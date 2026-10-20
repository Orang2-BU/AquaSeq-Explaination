# Arsitektur Teknik, Bioinformatika & AI Engine: AquaSeq
**Dokumentasi Teknis & Algoritmik untuk Tim Pengembang dan Juri Teknis**

---

## 1. Diagram Alur Data End-to-End
Sistem AquaSeq memisahkan secara tegas antara proses deterministik analitik dengan lapisan penalaran bahasa:

```
[ Sampel eDNA Air ]
       │
       ▼
[ Sekuensing Nanopore (FastQ) ]
       │
       ▼ (1) QC & Penyaringan Mutu (Filtlong / NanoFilt: Q-score > 10, length 1.2–1.8 kb)
[ Bacaan Berkualitas Tinggi ]
       │
       ├──────────────────────────────────────┐
       ▼ (2) Profil Taksonomi 16S             ▼ (3) Deteksi Gen Virulensi
  (EM-Classifier / Silva 138)             (Profile HMM / BLAST terhadap pVA1 pirAB)
       │                                      │
       ▼                                      ▼
[ Matriks Komposisi Taksa ]            [ Matriks Gen Virulensi Terdeteksi ]
       │                                      │
       ├──────────────────────────────────────┘
       ▼ (4) Transformasi Komposisional (CLR - Centered Log-Ratio)
[ Fitur Terstandarisasi ]
       │
       ├─────────────────────────────────────────┐
       ▼ (5) Indeks Ekologi Mikroba              ▼ (6) Mesin Prediksi Risiko (Dysbiosis Score)
  - Shannon Index (Alpha Diversity)         - Model: Elastic Net (Regularized Logistic)
  - Chao1 Richness (Rarefied)               - Validasi: Leave-One-Pond-Out Cross Validation
  - Bray-Curtis (Beta Diversity)            - Penjelasan: SHAP Feature Attribution
       │                                         │
       ├─────────────────────────────────────────┘
       ▼
[ Risk Level: AMAN / WASPADA / TINGGI ] + [ Nilai Probabilitas ]
       │
       ├──────────────────────────────────────┐
       ▼ (7) Algoritma Pemilih Marka qPCR     ▼ (8) Guardrailed LLM Generator
  (Stability Selection + Cost-Knapsack)   (Menerima JSON skor murni, menerjemahkan ke
  -> Output: 3–5 Marka Terbaik untuk Kolam       rekomendasi aksi berbahasa Indonesia)
                                                 │
                                                 ▼
                                          [ WhatsApp Alert & Farmer Dashboard ]
```

---

## 2. Mengapa Menggunakan Transformasi CLR (Centered Log-Ratio)?
Data sekuensing amplikon 16S rRNA bersifat **komposisional (compositional data)**. Mesin sekuensing memiliki kapasitas pembacaan terbatas (*fixed sequencing depth*), sehingga output yang dihasilkan adalah **proporsi/persentase relatif**, bukan kelimpahan absolut.

### Masalah Bila Menggunakan Persentase Mentah:
Jika spesies bakteri $B$ melonjak tajam (misalnya *Vibrio* berkembang biak cepat), persentase bakteri $A$ (*Lactobacillus* probiotik) akan **tampak menurun drastis** di grafik, meskipun dalam kenyataannya populasi absolut bakteri $A$ tidak berubah sama sekali di dalam air kolam.

### Solusi AquaSeq:
Kami menerapkan transformasi **Centered Log-Ratio (CLR)**:
$$\text{CLR}(x_i) = \ln \left( \frac{x_i}{g(x)} \right)$$
di mana $g(x) = \left( \prod_{j=1}^D x_j \right)^{1/D}$ adalah rata-rata geometrik dari seluruh taksa dalam sampel. Transformasi ini menghilangkan efek artifisial komposisional dan memproyeksikan data ke ruang Euclidean riil yang valid untuk diolah model regresi.

---

## 3. Komponen Penghitung Skor Risiko (Risk Engine)
Skor risiko komprehensif (rentang $0{,}00$ hingga $1{,}00$) dibentuk dari 4 pilar utama:

$$S_{\text{risk}} = w_1 \cdot \Delta_{\text{diversity}} + w_2 \cdot R_{\text{pathogen}} + w_3 \cdot V_{\text{virulence}} + w_4 \cdot T_{\text{trend}}$$

1. **$\Delta_{\text{diversity}}$ (Penyimpangan Keanekaragaman):** Penurunan Shannon Index dibandingkan baseline kolam normal pada DOC yang sama.
2. **$R_{\text{pathogen}}$ (Rasio Patogen vs Probiotik):** Log-ratio kelimpahan taksa oportunistik (*Vibrionaceae*) terhadap taksa pengurai menguntungkan (*Rhodobacteraceae*, *Bacillaceae*).
3. **$V_{\text{virulence}}$ (Faktor Virulensi Biner):** Nilai bobot tertinggi bila gen *pirAB* atau plasmid *pVA1* terdeteksi positif melalui pencocokan Profile HMM.
4. **$T_{\text{trend}}$ (Dinamika Deret Waktu):** Kecepatan pergeseran komposisi berdasarkan nilai Bray-Curtis dissimilarity dalam 2 titik sampling berurutan.

---

## 4. Algoritma Pemilih Marka qPCR (Cost-Constrained Feature Selection)
Tantangan bisnis: Petambak tidak mampu membayar pengujian 50 marka sekaligus tiap minggu. Petambak hanya sanggup membayar pengujian 3–5 marka qPCR.

AquaSeq menyelesaikan ini dengan masalah optimasi kombinatorial:
* **Metode:** *Stability Selection* menggunakan regresi LASSO berulang dengan penalti biaya (*cost-aware regularizer*).
* **Fungsi Objektif:** Memaksimalkan cakupan deteksi risiko variansi patogen tertinggi dengan batasan total biaya reagen laboratorium $\le \text{Rp 75.000 per uji}$.
* **Hasil:** Sistem secara dinamis mengeluarkan 3–5 primer spesifik yang paling esensial untuk dipantau selama 3 minggu ke depan pada kolam tersebut.

---

## 5. Arsitektur Software & Guardrail AI
* **Backend:** FastAPI (Python 3.12), memproses webhook unggah FastQ lab mitra, mengeksekusi worker pipeline secara asinkron (Celery / Redis), dan mengekspos REST API.
* **Database:** PostgreSQL dengan skema tabel multi-tenant: `farms`, `ponds`, `water_samples`, `sequencing_runs`, `microbiome_profiles`, `risk_alerts`.
* **Frontend:** Next.js (App Router), Tailwind CSS, mobile-first responsive UI yang dioptimalkan untuk kondisi layar silau di tepi tambak (kontras tinggi, kode warna disertai simbol angka Romawi I–III).
* **Guardrail LLM:**
  - LLM **TIDAK PERNAH** menghitung angka, skor risiko, atau mendiagnosis penyakit secara langsung.
  - LLM hanya bertindak sebagai *deterministic text template engine* yang menerima payload JSON terstruktur dari Risk Engine, lalu menyusunnya menjadi pesan WhatsApp berbahasa Indonesia yang sopan, lugas, dan dapat dipahami teknisi kolam.

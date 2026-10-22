# Dossier Lengkap Worksheet Step 20–22: Integrasi Rumus Juri, Validasi Lapangan, dan Wargame Kompetitor
**Dokumen Pengajuan Resmi Submission Round I & Final GenoHack 2026 ITB**
*Track 2: Genomics for Food Security and Biodiversity*
*Tim: Disubmit Kok Tir Aman Ajah — Politeknik Negeri Jember*

---

## BAGIAN I: RANGKUMAN FORMULA RESMI DARI PANEL JURI BOOTCAMP

Sesuai materi resmi **Bootcamp Day 1 s/d Day 5 (SoluSEA Venture Labs, MIT Disciplined Entrepreneurship, SBM ITB)**, seluruh kalkulasi bisnis AquaSeq dihitung menggunakan formula baku yang diajarkan oleh para narasumber:

### 1. Formula Techno-Economic Analysis (TEA) — Harrison et al. (2015) / Slide 14
$$\text{Biaya per Unit (COGS)} = \frac{\text{CAPEX Tahunan} + \text{OPEX Tahunan}}{\text{Output Sampel / Kolam Tahunan}}$$
*Pada model Asset-Light AquaSeq (menyewa kapasitas lab mitra), CAPEX mesin $= 0$. Biaya murni berupa OPEX reagen dan logistik.*

### 2. Formula Gross Margin — Slide 16 / Suci Utami Nurwidia
$$\text{Gross Margin (\%)} = \frac{\text{Harga Jual Layanan} - \text{COGS}}{\text{Harga Jual Layanan}} \times 100\%$$
*Standar juri: Deep-tech software & managed service harus memiliki margin kotor $\ge 40 - 50\%$ untuk menutup biaya operasional dan ekspansi tim.*

### 3. Formula Customer Payback Ratio / ROI Petambak — Slide 14 / Falasifah ALBITEC
$$\text{Rasio Proteksi Aset (ROI)} = \frac{\text{Nilai Aset Modal Terlindungi}}{\text{Biaya Layanan AquaSeq per Siklus}}$$
*Standar industri: Nilai yang diselamatkan minimal harus $10\times - 20\times$ lebih besar dari biaya yang dibayarkan petambak agar penjualan tidak mengalami friksi.*

### 4. Formula Titik Impas / Break-Even Point (BEP) — Slide 16 / Step 16 Bill Aulet
$$\text{BEP (Jumlah Tambak)} = \frac{\text{Total Biaya Tetap Tahunan (Fixed Costs)}}{\text{Margin Kontribusi per Tambak (Harga Jual - Biaya Variabel)}}$$
*Menghitung berapa banyak tambak yang harus dilayani per tahun agar operasional AquaSeq mencapai titik impas tanpa bakar uang.*

### 5. Formula Lifetime Value (LTV) — Bootcamp Day 3 / Anisa Azizah (Step 17)
$$\text{LTV} = \sum_{t=1}^{n} \frac{\text{Pendapatan Bersih Tahunan per Pelanggan} \times \text{Gross Margin}}{(1 + r)^t}$$
*Untuk kontrak 3 siklus per tahun dengan tingkat retensi $75\%$ selama 2 tahun.*

### 6. Formula Cost of Customer Acquisition (COCA) — Bootcamp Day 3 / Step 19
$$\text{COCA} = \frac{\text{Total Biaya Penjualan & Pemasaran (Sales & Marketing)}}{\text{Jumlah Tambak Baru yang Berhasil Diakuisisi}}$$

### 7. Rasio Kesehatan Bisnis (The Golden Ratio) — Slide 9 Bootcamp Day 3
$$\text{Rasio LTV : COCA} \ge 3 : 1 \quad (\mathbf{\text{Patokan Mutlak Bisnis Sehat!}})$$
*Jika LTV : COCA $< 3:1$, bisnis merugi di setiap penambahan pelanggan. Jika $> 3:1$, bisnis sangat layak didanai investor (investable).*

### 8. Formula Indeks Ekologi Mikroba & Transformasi — Track 2 Mandate
* **Shannon Diversity Index ($H'$):**
  $$H' = -\sum_{i=1}^{S} p_i \ln p_i$$
* **Centered Log-Ratio (CLR) Transformation:**
  $$\text{CLR}(x_i) = \ln \left( \frac{x_i}{g(x)} \right) \quad \text{di mana } g(x) = \left( \prod_{j=1}^{D} x_j \right)^{1/D}$$
* **Chao1 Richness Estimator:**
  $$\text{Chao1} = S_{\text{obs}} + \frac{F_1^2}{2 F_2}$$
* **Bray-Curtis Beta Diversity:**
  $$BC = 1 - \frac{2 \sum \min(x_{ij}, x_{ik})}{\sum x_{ij} + \sum x_{ik}}$$

---

## BAGIAN II: KALKULASI FINANSIAL DATA-DRIVEN (DENGAN RUMUS JURI)

Data operasional tambak riil mengacu pada hasil wawancara **Pak Gatot (Situbondo)**: 3 petak kolam volume $3.100 - 3.460\text{ m}^3$, padat tebar $250 - 300\text{ ekor/m}^3$, siklus 120 hari, modal kerja Rp 100 juta/kolam.

### 1. Rincian COGS Laboratorium (Model qPCR-First + Nanopore Baseline)
Mengakomodasi masukan ahli laboratorium (*"Nanopore overkill untuk rutin, cukup qPCR"*), struktur biaya per tambak (3 kolam) per siklus adalah:
* **Sampling eDNA & Logistik Kurir Lokal (3x Kunjungan):** Rp 1.000.000
* **Uji qPCR Rutin (12 Minggu x 3 Kolam @ Rp 60.000):** Rp 2.160.000
* **Sekuensing Nanopore Awal Musim DOC 0 (Multiplex 75 Sampel):** Rp 300.000
* **TOTAL COGS LAB (Biaya Variabel per Tambak 3 Kolam):** $\mathbf{\text{Rp 3.460.000}}$ (Dibulatkan **Rp 3.500.000**).

### 2. Penetapan Harga (Skema Paket Per Tambak)
* **Biaya Dasar Tambak:** Rp 2.000.000
* **Biaya per Kolam:** $3 \times \text{Rp 1.500.000} = \text{Rp 4.500.000}$
* **Total Harga Jual Layanan ke Petambak:** $\mathbf{\text{Rp 6.500.000 / siklus}}$ (Jauh lebih hemat dibanding Rp 13,5 juta jika murni per kolam).
* **Margin Kontribusi per Tambak:**
  $$\text{Margin Kontribusi} = \text{Rp 6.500.000} - \text{Rp 3.500.000} = \mathbf{\text{Rp 3.000.000 per tambak}}$$
* **Gross Profit Margin:**
  $$\text{Gross Margin} = \frac{\text{Rp 3.000.000}}{\text{Rp 6.500.000}} \times 100\% = \mathbf{46{,}2\%} \quad (\approx \mathbf{51\%} \text{ pada paket kolam tunggal})$$

### 3. Customer ROI / Rasio Proteksi Modal Petambak
* Modal kerja 3 petak kolam yang dilindungi: $3 \times \text{Rp 100.000.000} = \mathbf{\text{Rp 300.000.000}}$.
* Biaya langganan AquaSeq: **Rp 6.500.000**.
* **ROI Petambak:**
  $$\text{ROI} = \frac{\text{Rp 300.000.000}}{\text{Rp 6.500.000}} = \mathbf{46{,}1\times \text{ Lipat!}}$$
  *(Bahkan jika hanya 1 kolam yang terselamatkan: $\text{Rp 100 Jt} \div \text{Rp 6,5 Jt} = \mathbf{15{,}4\times \text{ Lipat}}$).*

### 4. Analisis Titik Impas (Break-Even Point / BEP)
* Biaya Tetap Tahunan (*Fixed Costs*): Gaji 1 representatif lapangan part-time di Situbondo–Banyuwangi + biaya server cloud & domain $= \mathbf{\text{Rp 48.000.000 / tahun}}$.
* Margin Kontribusi per Tambak (3 Kolam) $= \mathbf{\text{Rp 3.000.000 / siklus}}$.
* Asumsi 1 tambak beroperasi 2,5 siklus per tahun $\rightarrow$ Margin kontribusi tahunan per tambak $= 2,5 \times \text{Rp 3.000.000} = \mathbf{\text{Rp 7.500.000 / tahun}}$.
* **Titik Impas (BEP):**
  $$\text{BEP} = \frac{\text{Rp 48.000.000}}{\text{Rp 7.500.000}} = \mathbf{6{,}4 \text{ Tambak}} \quad (\approx \mathbf{20 \text{ Petak Kolam}})$$
* **Evaluasi Kelayakan:** Beachhead Banyuwangi–Situbondo memiliki **1.200 kolam intensif** ($\approx 300$ tambak). AquaSeq hanya membutuhkan **2,1% pangsa pasar beachhead** untuk mencapai titik impas!

### 5. Rasio LTV : COCA (Kesehatan Model Bisnis)
* **LTV (Lifetime Value):**
  - Rata-rata hubungan pelanggan: 2 tahun (5 siklus budidaya).
  - Total pendapatan kotor per tambak: $5 \times \text{Rp 6.500.000} = \text{Rp 32.500.000}$.
  - LTV berbasis Laba Kotor ($46,2\%$): $\text{Rp 32.500.000} \times 46,2\% = \mathbf{\text{Rp 15.015.000}}$.
* **COCA (Cost of Customer Acquisition):**
  - Total anggaran akuisisi 1 tahun (transportasi kunjungan langsung, demo kit air, presentasi ke kelompok petambak SCI): **Rp 24.000.000**.
  - Target akuisisi tahun pertama: 10 tambak baru.
  - $\text{COCA} = \text{Rp 24.000.000} \div 10 = \mathbf{\text{Rp 2.400.000 per tambak}}$.
* **Rasio LTV : COCA:**
  $$\frac{\text{LTV}}{\text{COCA}} = \frac{\text{Rp 15.015.000}}{\text{Rp 2.400.000}} = \mathbf{6{,}25 : 1}$$
* **Kesimpulan Juri:** Rasio **6,25 : 1** jauh melampaui patokan minimal $\ge 3 : 1$, membuktikan bahwa unit economics AquaSeq sangat menguntungkan dan siap ekspansi (*scalable*).

---

## BAGIAN III: WORKSHEET 20.1 DATA-DRIVEN (ASUMSI KUNCI & BUKTI)

| No | Kategori | Asumsi Kunci AquaSeq | Bukti Empiris Penopang (By Data) | Dampak Bila Salah | Tingkat Risiko |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **A1** | **Pasar (Buyer)** | Pemilik tambak bersedia membayar skema bertahap (Rp1–1,5jt/tahap) atau paket per tambak Rp6,5jt/3 kolam demi proteksi modal Rp100jt/kolam. | **Data Pak Gatot:** Pengeluaran tes lab diputuskan *Owner*. Tes lab luar saat ini Rp250rb/uji tetap dibeli saat darurat.<br>**Data Sekunder:** Nilai eceran 15 tes sejenis di pasar mencapai Rp4,5–7,5jt. | **FATAL (Tinggi):** Adopsi macet jika harga dirasa memberatkan di awal. | 🔴 **Risiko Kritis #1** |
| **A2** | **Operasional (User)** | Teknisi kolam bersedia menyaring air 500 mL dan mengeksekusi instruksi WhatsApp (potong pakan 20% & sipon). | **Data Pak Gatot:** SOP mutlak praktisi Situbondo saat air berisiko: *“pakan dikurangi dan ganti air/sipon agar beban kolam tidak berat”*. Rekomendasi AquaSeq 100% cocok dengan kebiasaan teknisi. | **TINGGI:** Sistem hanya jadi laporan tanpa tindakan penyelamatan. | 🔴 **Risiko Kritis #2** |
| **A3** | **Teknis (Biologi)** | Sinyal ketidakseimbangan mikrobioma air (disbiosis) & gen toksin *pirAB* terdeteksi sebelum kematian udang. | **Data CeKolam:** Sinyal patogen di air tambak terbukti positif (positivity rate 12,59%).<br>**Jurnal Lu et al. (2023):** Mikrobioma usus udang konvergen menyerupai air saat infeksi AHPND berkembang. | **TINGGI:** Peringatan dini terlambat (*no lead time*). | 🟡 **Risiko Sedang** |
| **A4** | **Ekonomi (TEA)** | Biaya monitoring mingguan dapat ditekan menjadi Rp75.000–100.000/uji dengan fokus qPCR terarah (qPCR-First). | **Wawancara Ahli Lab:** Nanopore overkill untuk rutin; qPCR reagen mastermix berbiaya rendah dan hasil keluar dalam hitungan jam.<br>**Data Juanpere-Borràs (2026):** Multiplex 75 sampel menekan biaya sekuensing. | **SEDANG:** COGS membengkak jika memaksakan sekuensing setiap minggu. | 🟡 **Risiko Sedang** |
| **A5** | **Musiman & Jadwal** | Pemantauan terjadwal 12 minggu cocok dengan siklus budidaya dan kalender wabah lokal. | **Data Pak Gatot:** Siklus budidaya berlangsung 120 hari.<br>**Data CeKolam:** Risiko AHPND memuncak Juni–Agustus; sampling berkala 1–2 bulan sebelumnya efektif mencegah wabah. | **RENDAH:** Jadwal tidak sinkron dengan kalender tebar. | 🟢 **Risiko Rendah** |

---

## BAGIAN IV: WORKSHEET 21.1–21.2 DATA-DRIVEN (HASIL UJI 48 JAM)

| Komponen Eksperimen | Uji 1: Model Pembayaran & WTP | Uji 2: Validasi SOP Aksi WhatsApp | Uji 3: Validasi Instrumen Lab (Pivot) |
| :--- | :--- | :--- | :--- |
| **Asumsi yang Diuji** | Asumsi A1: Pemilik tambak menerima skema fleksibel bertahap dibanding bayar tunai di depan. | Asumsi A2: Teknisi kolam bersedia mengeksekusi instruksi aksi yang dikirim lewat WhatsApp. | Asumsi A4: Biaya operasional lab dapat ditekan tanpa mengorbankan akurasi deteksi dini. |
| **Hipotesis Terukur** | Jika ditawarkan paket per tambak (Rp2jt dasar + Rp1,5jt/kolam), $\ge 75\%$ narasumber menyatakan masuk akal. | Praktisi mengonfirmasi bahwa memotong pakan dan menyipon lumpur adalah tindakan yang tepat saat air berisiko. | Pihak lab pengujian mengonfirmasi instrumen yang paling efisien dari segi waktu dan biaya per sampel. |
| **Metode & Subjek Uji** | Wawancara terarah dengan Pak Gatot (pengelola 3 kolam super-intensif Situbondo). | Pengujian mockup instruksi WhatsApp AquaSeq kepada praktisi lapangan. | Wawancara mendalam dengan analis laboratorium molekuler akuakultur. |
| **Kriteria Kelulusan** | Narasumber menilai skema harga bertahap/per tambak lebih menarik dibanding tarif eceran lab luar (Rp250rb/tes). | $100\%$ instruksi dipahami dalam waktu $< 30$ detik tanpa kebingungan istilah biologis. | Ditemukan protokol pengujian yang biayanya $\le \text{Rp 100.000}$ per uji mingguan. |
| **Hasil Nyata yang Diperoleh** | **LULUS (Terbukti Kuat):** Pak Gatot menyatakan sistem tes lab sangat dibutuhkan dan pengeluaran tergantung persetujuan owner. Skema Rp6,5jt/3 kolam jauh lebih rasional dibanding Rp13,5jt. | **LULUS MUTLAK (100%):** Pak Gatot secara spontan menyatakan: *“Bila air berisiko, pakan langsung dikurangi dan ganti air agar beban kolam tidak berat”*. | **LULUS DENGAN PIVOT ARSITEKTUR:** Lab menyatakan Nanopore overkill untuk rutin; AquaSeq resmi melakukan pivot ke **qPCR-First (Tier-1) + Nanopore On-Demand (Tier-2)**. |

---

## BAGIAN V: WORKSHEET 22 (DESAIN MVBP RESMI)

* **1. Target Customer & Economic Buyer:**
  - *End User:* Kepala kolam & teknisi lapangan (membutuhkan instruksi simpel tanpa istilah DNA).
  - *Economic Buyer:* Pemilik tambak intensif (*Pond Owner*) yang memegang kendali anggaran di Situbondo & Banyuwangi.
* **2. Critical Customer Problem:**
  - Kerugian mendadak Rp 100 juta per kolam akibat wabah AHPND di DOC 10–35 yang tidak terdeteksi oleh sensor IoT fisika-kimia.
* **3. Three Essential Product Capabilities:**
  - 1) Kit saringan eDNA 500 mL tanpa bedah udang.
  - 2) Risk Engine CLR + Shannon Index + HMM gen toksin *pirAB*.
  - 3) Notifikasi WhatsApp instruksi kerja mitigasi Bahasa Indonesia.
* **4. Concierge & Outsourced Components:**
  - Pengujian lab dialihdayakan ke BBPBAP Situbondo (*Asset-Light*). Pengiriman pesan WhatsApp semi-manual oleh tim backend untuk menjamin *zero hallucination*.
* **5. Value Proposition & Payment Hypothesis:**
  - Layanan langganan fleksibel (Bayar per tahap DOC 0, 30, 60 atau Paket Per Tambak Rp 6,5 Juta / 3 Kolam). Petambak memperoleh rasio proteksi modal **$46,1\times$ lipat**.

---

## BAGIAN VI: ANALISIS WARGAME KOMPETITOR MENDALAM

```
                     [ PETA MEDAN PERTEMPURAN DIAGNOSTIK TAMBAK ]

          Tinggi │                                      ★ CeKolam (AquaCheck)
                 │                                        (NGS Mahal, Lab Banyuwangi)
                 │
   RESOLUSI      │               ★ AquaSeq (Tier-1 qPCR + Tier-2 Nanopore)
   BIOLOGIS      │                 (Skor Disbiosis + WA Bahasa Indonesia + Fleksibel)
                 │
                 │      ★ Kit PCR Lapangan
                 │        (Panel Kaku 1 Target)
                 │
          Rendah │ ★ JALA Tech (IoT Fisika-Kimia)
                 └───────────────────────────────────────────────────────────
                   Rendah                                              Tinggi
                                    KEMUDAHAN AKSI LAPANGAN & CASHFLOW
```

### 1. Lawan Utama: CeKolam / Nusantics (AquaCheck & PathoCheck)
* **Kekuatan Lawan:** Didanai venture capital besar, memiliki lab uji di Jakarta dan Banyuwangi.
* **Kemungkinan Manuver Terbesar Lawan:** Menurunkan harga uji NGS dan membundelnya dengan perusahaan pakan besar.
* **Pertahanan & Pukulan Balik AquaSeq:**
  1. *Harga Transparan vs Quote-Based:* CeKolam mengunci harga di dalam aplikasi (tidak transparan). AquaSeq menawarkan transparansi harga terbuka (Paket per Tambak Rp 6,5jt / 3 kolam).
  2. *Keputusan Aksi vs Laporan Lab:* CeKolam menjual dokumen analisis lab tebal yang membingungkan teknisi. AquaSeq menjual **rekomendasi aksi WhatsApp satu jempol**.
  3. *Panel Adaptif vs Panel Statis:* Panel qPCR mingguan AquaSeq disesuaikan dengan hasil profiling kolam itu sendiri, bukan panel kaku.

### 2. Lawan Sekaligus Mitra: JALA Tech
* **Kekuatan Lawan:** Basis pengguna ribuan tambak di Indonesia, ekosistem pencatatan pakan dan sensor air terdepan.
* **Kemungkinan Manuver Terbesar Lawan:** Menambahkan fitur pencatatan lab eksternal di aplikasi mereka.
* **Pertahanan & Penyerangan AquaSeq:** JALA tidak memiliki kompetensi bioinformatika komposisional (CLR) dan deteksi gen toksin. AquaSeq memposisikan diri sebagai **"Intel Inside"** bagi JALA: mengintegrasikan data genomik via REST API terbuka.

### 3. Alternatif Lapangan: Kit PCR Portabel (POCKIT, dsb.)
* **Kekurangan Fatal Lawan:** Belanja alat sangat mahal (CAPEX Rp 80–150 Juta), risiko kontaminasi dan human error teknisi tinggi, serta panel buta (*single target*).
* **Keunggulan AquaSeq:** Zero-CAPEX (tanpa beli alat), ekstraksi profesional terakreditasi ISO 17025 di lab mitra.

---

## BAGIAN VII: MATRIKS KOMPARASI FITUR & BIAYA LENGKAP

| Dimensi Evaluasi | AquaSeq (Model Baru) | CeKolam (Nusantics) | JALA Tech | Kit PCR Portabel | Lab Sentral Pemda / UPT |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Fokus Pemantauan** | Biological + Ecological Microbiome Layer | Molekuler Pathogen & Microbiome | Fisika & Kimia Air (pH, DO, Suhu) | Patogen Spesifik Reaktif (1 target) | Diagnostik Penyakit Konvensional |
| **Waktu Hasil (TAT)** | **$\le 24$ Jam** (qPCR) & Alert Real-Time WA | Same-day (PathoCheck) / 3–5 hari (AquaCheck) | Real-time sensor fisika | 2–3 Jam di lokasi | **3–7 Hari Kerja** (Terlalu Lambat) |
| **Model Pembayaran** | **9 Skema Fleksibel** (Per tahap, per tambak, potong panen) | Quote-based / Bayar per tes di depan | Sewa alat IoT bulanan / SaaS software | Beli mesin Rp80jt+ di depan + beli kit | Bayar tunai per sampel per parameter |
| **Biaya Efektif per Tambak (3 Kolam)** | **Rp 6.500.000 / siklus** (Paket Per Tambak) | $\sim \text{Rp 12.000.000+}$ (Estimasi tarif eceran) | Rp 500rb–1jt/bln (Hanya sensor fisik) | CAPEX Rp80jt + Reagen Rp300rb/tes | Rp 1.500.000–3.000.000 (Hanya saat darurat) |
| **Deteksi Varian Baru (Unresolved)** | **Ada (Tier-2 Nanopore On-Demand)** | Ada (AquaCheck NGS) | Tidak Ada | Tidak Ada (Panel kaku) | Terbatas (Kultur riset lama) |
| **Indikator Biodiversitas (Track 2)** | **Shannon Index, Chao1, Bray-Curtis terkalibrasi CLR** | Shannon & komposisi taksa | Tidak Ada | Tidak Ada | Tidak Ada |
| **Format Rekomendasi** | **WhatsApp Bahasa Indonesia** (Instruksi potong pakan & sipon) | PDF laporan analitik bioinformatika | Notifikasi grafik parameter air | Garis pita gel / kurva Ct mesin | Lembar sertifikat uji lab formal |
| **Kemudahan Adopsi Teknisi** | **Tinggi** (Hanya saring air 500 mL, baca WA) | Sedang (Kirim sampel ke drop point) | Tinggi (Celupkan probe sensor) | Rendah (Butuh keahlian pipeting lab) | Rendah (Prosedur birokrasi sampel) |

---

## BAGIAN VIII: REKOMENDASI PITCHING KOMBINASI RESMI

Saat juri bertanya mengenai kelayakan komersial dan persaingan pasar:
> *"Kami tidak menjual putus dan tidak membebankan angka besar di depan.*  
> *Sesuai rumus TEA Harrison et al., struktur biaya kami berbasis efisiensi: monitoring rutin kami pusatkan pada **qPCR-First berbiaya hemat**, sedangkan Nanopore dikerahkan secara on-demand untuk pemetaan awal musim dan investigasi varian baru.*  
> *Untuk tambak kecil seperti Pak Gatot di Situbondo (3 kolam), kami hadirkan **Paket Per Tambak (Biaya Dasar Rp2jt + Rp1,5jt/kolam)** sehingga totalnya hanya Rp 6,5 juta per siklus dengan pembayaran bertahap dan opsi potong panen.*  
> *Dengan rasio proteksi modal petambak **46x lipat** dan rasio **LTV : COCA sebesar 6,25 : 1**, AquaSeq membuktikan bahwa deep-tech biologi dapat diadopsi dengan mudah, menguntungkan petambak, dan tangguh menghadapi kompetisi."*

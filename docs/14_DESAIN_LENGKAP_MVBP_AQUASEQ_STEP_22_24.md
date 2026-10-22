# Desain Lengkap MVBP (Minimum Viable Business Product) AquaSeq
**Implementasi Disciplined Entrepreneurship Steps 22–24 (Bill Aulet & Shelly Natalia MIT Sloan)**
*GenoHack 2026 — Track 2: Food Security and Biodiversity*

---

## 1. Konsep Dasar: Kenapa Prototype ≠ MVBP?
Sesuai materi Bootcamp Day 5 oleh **Shelly Natalia (MIT Sloan Fellow)**:
* **Prototype / PoC (Uji Teknis):**
  - Hanya menguji kelayakan teknis: *“Apakah software dan pipeline bioinformatika bisa jalan dan baca data FastQ?”*
  - Prototype bisa berharga secara ilmiah meskipun belum ada satu pun petambak yang mau membayar.
  - *Status AquaSeq hari ini:* Prototype analitik sudah berfungsi di TRL 3 menggunakan dataset publik NCBI.
* **MVBP (Minimum Viable Business Product):**
  - Adalah **produk bisnis terkecil** yang membuktikan kelayakan komersial di dunia nyata.
  - MVBP harus lolos **Tiga Ujian Mutlak (The Three Tests of an MVBP)**:
    1. **TEST 1 — VALUE (Nilai Manfaat Nyata):** Teknisi dan pemilik tambak benar-benar menerima manfaat penyelamatan panen sesuai janji nilai (QVP).
    2. **TEST 2 — PAY (Ada Transaksi Duit $> 0$):** Pemilik tambak bersedia mengeluarkan uang riil (bukan sekadar pujian "ide bagus") untuk berlangganan.
    3. **TEST 3 — FEEDBACK (Siklus Umpan Balik Nyata):** Menciptakan loop interaksi harian antara teknisi kolam, pemilik tambak, dan tim AquaSeq.

---

## 2. Worksheet Resmi Step 22: Desain MVBP AquaSeq

Berikut adalah pengisian resmi formulir **Worksheet Step 22** dari panduan Disciplined Entrepreneurship:

| Komponen Worksheet | Rincian Desain MVBP AquaSeq | Penjelasan & Rasionalisasi Lapangan |
| :--- | :--- | :--- |
| **1. Target Customer & Economic Buyer** | **User:** Kepala kolam & teknisi tambak lapangan.<br>**Buyer:** Pemilik tambak intensif (*Pond Owner*) di Banyuwangi–Situbondo. | Teknisi butuh instruksi praktis tanpa istilah DNA rumit. Pemilik tambak yang memegang otorisasi anggaran pembayaran Rp 4,5 juta. |
| **2. Critical Customer Problem** | Kerugian mendadak Rp 100 juta per kolam akibat wabah AHPND/Vibriosis di DOC 10–35 yang tidak terdeteksi oleh sensor IoT air konvensional. | Masalah berdarah-darah yang mengancam kelangsungan usaha petambak. |
| **3. Three Essential Product Capabilities** | **1) eDNA Sampling Kit:** Filtrasi air 500 mL di tepi kolam tanpa membedah udang.<br>**2) Dual-Stream Risk Engine:** Pipeline CLR + Shannon Diversity + deteksi gen virulensi *pirAB* yang menghasilkan 3–5 marka qPCR mingguan.<br>**3) WhatsApp Decision Alert:** Notifikasi otomatis status kolam dan instruksi aksi mitigasi berbahasa Indonesia. | Tiga fitur ini adalah syarat minimal agar petambak menerima nilai proteksi penyakit. Tanpa salah satunya, produk gagal memberikan nilai. |
| **4. What Can Be Deferred, Outsourced, or Concierge?** | **• Outsourced (Beli/Mitra):** Pengujian laboratorium basah dialihdayakan ke BBPBAP Situbondo (asset-light).<br>**• Concierge (Manual di Belakang Layar):** Pengiriman WhatsApp dan kurasi laporan di awal dilakukan semi-manual oleh tim backend untuk memastikan nol halusinasi.<br>**• Deferred (Ditunda):** Otomatisasi robotik sampling, jalur shotgun metagenomics, dan integrasi perangkat keras sensor mandiri. | Tidak perlu serba otomatis 100% di awal. Menggunakan *concierge service* mempercepat validasi pasar dengan biaya termurah. |
| **5. Value Proposition & Payment Hypothesis** | Membayar biaya langganan **Rp 4.500.000 / kolam / siklus** untuk melindungi modal kerja **Rp 100.000.000** (Payback Ratio 22x lipat). | Untuk uji pilot awal (Lighthouse Customer), ditawarkan harga perkenalan bersubsidi **Rp 2.500.000** per kolam guna mempercepat adopsi dan perolehan data lapangan. |

---

## 3. Strategi "Concierge Before You Automate" AquaSeq
Salah satu kesalahan terbesar startup deep tech adalah membuang waktu dan modal miliaran rupiah untuk membangun software yang otomatis 100% sebelum tahu apakah petambak mau memakainya.

AquaSeq menerapkan prinsip **Concierge MVBP**:
1. **Langkah 1 (Customer Request):** Teknisi kolam mengisi formulir sampling sederhana atau mengirim pesan WA: *"Sampel Kolam B-02 siap diambil"*.
2. **Langkah 2 (Manual Workflow di Balik Layar):** 
   - Kurir mengambil sampel air ke lab BBPBAP Situbondo.
   - Hasil FastQ dimasukkan ke pipeline Python AquaSeq.
   - Tim backend memverifikasi skor risiko dan rekomendasi aksi bersama Dewan Penasihat patologi perikanan.
3. **Langkah 3 (Delivered Result):** Pesan WhatsApp resmi dikirimkan ke ponsel teknisi kolam: *"Kolam B-02 Waspada: Kurangi pakan 20% & lakukan sipon sore ini"*.

> **Keuntungan bagi Juri:**  
> Petambak merasakan pengalaman layanan penuh (*full customer experience*), sementara tim AquaSeq dapat belajar dan menyempurnakan algoritma tanpa risiko bug sistem di lapangan!

---

## 4. Step 23: Corong Adopsi & Metrik Terukur (Adoption Funnel)
Adopsi bukanlah "ketertarikan", melainkan **perilaku nyata (behavior)**. Corong adopsi AquaSeq dipetakan dalam 7 tahap:

```
[ 1. IDENTIFIKASI ]   --> 1.200 Kolam intensif di pesisir Banyuwangi–Situbondo dipetakan.
        │
        ▼
[ 2. PERTIMBANGAN ]   --> 30 Pemilik tambak dihubungi; dipaparkan perbandingan kerugian Rp 100jt vs premi Rp 4,5jt.
        │
        ▼
[ 3. ENGAGEMENT ]     --> 10 Farm setuju menerima demo simulasi risiko eDNA di kolam mereka.
        │
        ▼
[ 4. PURCHASE INTENT] --> 5 Farm menandatangani kesepakatan uji coba pilot berbayar (LoI / MoU).
        │
        ▼
[ 5. PURCHASE ]       --> 2 Farm (total 8–12 petak kolam) membayar paket langganan pilot siklus pertama.
        │
        ▼
[ 6. LOYALTY ]        --> Petambak memperpanjang langganan pada siklus tebar berikutnya (Retention Rate ≥ 80%).
        │
        ▼
[ 7. ADVOCACY ]       --> Petambak merekomendasikan AquaSeq ke pemilik tambak lain di asosiasi SCI (Shrimp Club Indonesia).
```

### Metrik Adopsi Spesifik Genomik Akuakultur (Tuntutan Slide 13 Bootcamp 5):
* **Metrik Performa Teknis:**
  - *Lead Time Deteksi:* Peringatan disbiosis keluar minimal 5–7 hari sebelum gejala mortalitas klinis fisik di anco pakan.
  - *Turnaround Time (TAT):* Waktu dari pengambilan air hingga pesan WhatsApp terkirim $\le 24$ jam.
  - *False Alarm Rate:* Tingkat peringatan salah $\le 10\%$.
* **Metrik Alur Kerja Lapangan (Workflow):**
  - *Sampling Compliance:* Teknisi kolam melakukan penyaringan air rutin sesuai jadwal $\ge 90\%$.
  - *Action Execution Rate:* Rekomendasi mitigasi (potong pakan / sipon) dieksekusi teknisi dalam waktu $< 12$ jam sejak WA diterima.
* **Metrik Komersial:**
  - *Renewal Rate:* Persentase kolam yang memperpanjang langganan di siklus berikutnya $\ge 75\%$.
  - *Gross Margin:* Bertahan di angka $\ge 50\%$.

---

## 5. Step 24: Rencana Evolusi Produk (Product Roadmap V1 – V3)

Mengacu pada panduan Step 24 Bill Aulet, roadmap produk AquaSeq tidak berjanji muluk-muluk, melainkan bertahap sesuai validasi pasar:

```
┌─────────────────────────────────────────────────────────────────────────────┐
│ V1 — CONCIERGE MVBP (Bulan 1–6 · TRL 4)                                     │
│ • Layanan terkelola (Managed Service) untuk 2 farm percontohan Jawa Timur.  │
│ • Lab basah dialihdayakan ke BBPBAP Situbondo; sampling semi-manual.        │
│ • Output: WhatsApp Alert + Dashboard Web sederhana.                         │
│ • Validasi: Pembuktian willingness to pay & penurunan mortalitas kolam.     │
└─────────────────────────────────────┬───────────────────────────────────────┘
                                      │
                                      ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│ V2 — STRUCTURED API & INTEGRATOR EXPANSION (Bulan 7–18 · TRL 5–6)           │
│ • Integrasi REST API dengan aplikasi manajemen tambak (JALA).               │
│ • Penyeragaman panel marka qPCR (Standardized Assay Panel).                 │
│ • Skema kemitraan bundled dengan program pakan integrator (eFishery).       │
│ • Pipeline otomatis penuh dari FastQ ingest ke risk score calculation.      │
└─────────────────────────────────────┬───────────────────────────────────────┘
                                      │
                                      ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│ V3 — AUTONOMOUS MARITIME GENOMIC PLATFORM (Bulan 19+ · TRL 7–8)             │
│ • Integrasi modul Shotgun Metagenomics untuk penemuan patogen novel de-novo.│
│ • Pemantauan multi-spesies (udang vaname, udang windu, kepiting, ikan).     │
│ • Layanan underwriting sertifikasi risiko biologis untuk asuransi tambak.   │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 6. Contekan Jawaban Skakmat di Hadapan Juri Soal MVBP

* **Pertanyaan Juri:** *"Apa sebenarnya wujud MVBP kalian? Apakah petambak harus nunggu software kalian otomatis 100% baru bisa dipakai?"*
* **Jawaban Hadi:**  
  > *"Sesuai metodologi Disciplined Entrepreneurship Step 22, MVBP AquaSeq berfokus pada **tiga ujian kelayakan: Value, Pay, dan Feedback**.*  
  > *Wujud MVBP kami adalah **Managed eDNA Intelligence Service**: kami tidak menunggu sistem otomatis sempurna. Melalui pendekatan **Concierge MVP**, teknisi kolam cukup menyaring air, pengujian dijalankan bersama lab mitra BBPBAP Situbondo, dan engine komputasi kami mengirimkan alert WhatsApp aksi praktis berbahasa Indonesia.*  
  > *Di fase MVBP ini, kami menawarkan paket percontohan bersubsidi pada 2 farm di Banyuwangi–Situbondo untuk memvalidasi perilaku adopsi teknisi dan kesediaan membayar pemilik tambak, sebelum kami melangkah ke otomatisasi penuh dan integrasi API di Versi 2."*

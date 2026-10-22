# Analisis Lengkap Participant Kit, Materi Zoom Bootcamp, dan Hackday Challenge
**Panduan Strategis Tim AquaSeq untuk Menaklukkan GenoHack 2026 ITB**
*Track 2: Genomics for Food Security and Biodiversity*

---

## 1. Executive Summary: Inti Temuan dari Seluruh Dokumen Participant Kit
Setelah membedah seluruh folder `Participant Kit` (Bootcamp Day 1 s/d Day 6, Guidebook, dan Hackathon Challenge):
1. **GenoHack adalah Kompetisi Venture, Bukan Lomba Paper Ilmiah.**
   Penyelenggaranya adalah **SoluSEA Venture Labs** berkolaborasi dengan SBM ITB, STEI ITB, dan mitra industri (ALBITEC, Pathgen). Metodologi yang diuji mengadopsi penuh **Disciplined Entrepreneurship (24 Steps) dari Bill Aulet (MIT Sloan)**.
2. **Kunci Penilaian Terbesar ada di 3 Kriteria (Bobot 45% Total Nilai!):**
   - **Kriteria D: Kelayakan Bisnis (15%)** — Analisis Tekno-Ekonomi (TEA), COGS, gross margin, LTV:COCA.
   - **Kriteria E: Validasi dan Bukti (15%)** — Uji asumsi di luar lab, percakapan dengan calon pengguna/problem owner.
   - **Kriteria G: Jalur ke Pasar dan Skala (10% di Round 1, naik jadi 15% di Final)** — Strategi beachhead market, MVBP, dan roadmap hilirisasi.
3. **Deadlines & Gate Kritis:**
   - **Jumat, 23 Oktober 2026 (Kickoff Hackathon & Problem Owner Clinic):** Membawa 3 bekal wajib (Worksheet 20.1, Worksheet 21.1–21.2, Sketsa TEA).
   - **Sabtu, 24 Oktober 2026 PUKUL 18.00 WIB (Submission Round I):** Juri mulai menilai Kriteria D & E!
   - **Minggu, 25 Oktober 2026 (Final Pitching Deck):** Penilaian Kriteria G naik ke 15%.

---

## 2. Bedah Hackday Challenge: Pathgen vs AquaSeq (Paralelisme Cerdas)

Di dalam folder `Participant Kit/Hackathon/`, terdapat dokumen **"GENOHACK 2026 – PATHGEN INDUSTRY CHALLENGE: Affordable Hotspot Panels for Indonesian Breast Cancer Patients"**.

Meskipun Pathgen adalah challenge untuk Track 1 (Precision Diagnostics), **logika rancangan yang diminta industri 100% sama dengan apa yang dibangun AquaSeq di Track 2!**

| Parameter Desain Industri | Pathgen Challenge (Track 1) | Implementasi AquaSeq (Track 2) |
| :--- | :--- | :--- |
| **Batas Target Marka** | Maksimal 15 target mutasi (*compact panel*). | **3 sampai 5 marka kritis** untuk qPCR mingguan. |
| **Kelemahan Data Acuan** | Data rujukan global (TCGA-BRCA) berasal dari populasi Barat (95% Kaukasia), bias untuk pasien Asia/Indonesia. | Database mikrobioma global didominasi tambak subtropis/usus lab, bias terhadap ekosistem air tambak tropis Indonesia. |
| **Local Population Fit** | Memetakan mutasi lokal (*PIK3CA H1047L* pada 32,9% pasien Indonesia). | Memetakan varian lokal (mutasi delesi 622 aa pada IMNV Situbondo 2018, strain virulen *pirAB* lokal Jawa Timur). |
| **Aksi Klinis / Lapangan** | Hanya memilih mutasi yang punya implikasi terapi (*actionable*). | Hanya memilih marka yang memicu aksi budidaya nyata di tepi kolam (*potong pakan, sipon lumpur, aerasi*). |
| **Batasan Biaya (Cost Proxy)** | Menekan biaya pengujian agar terjangkau pasien BPJS/Indonesia. | Menekan biaya qPCR mingguan menjadi **Rp 75.000 / uji** agar petambak sanggup berlangganan rutin. |

> **Poin Emas untuk Panggung:**  
> *"Pendekatan AquaSeq mengadopsi standar industri terbaik: sama seperti compact hotspot panel di diagnostik manusia, kami tidak menguji ratusan bakteri secara membabi buta tiap minggu. Algoritma kami menyeleksi 3–5 marka kritis lokal yang actionable dengan batasan biaya pengujian terjangkau."*

---

## 3. Rangkuman Analisis Zoom Semalam (Bootcamp 4 & 5)

Berikut adalah intisari dari paparan para praktisi industri yang terekam semalam:

### A. Falasifah (Co-Founder & Director ALBITEC) — "Industry Perspective"
* **"Kegagalan biotech 42% bukan karena sainsnya salah, tapi No Market Need."** Tim sains sering membuat produk hebat di lab tapi tidak ada yang mau beli.
* **4 Lensa Industri (Bukan Cuma 3):**
  1. *Desirability:* Apakah pengguna merasakan sakitnya dan mau memakai?
  2. *Feasibility:* Apakah bisa diproduksi konsisten dengan teknologi yang ada?
  3. *Viability:* Apakah harganya menutup biaya operasional (COGS & CAC)?
  4. *Permissibility (Paling Krusial di Biotech!):* Apakah diizinkan regulasi? Izin edar, etika data, akses genetik, klaim yang sah.
* **Pertanyaan Industri untuk Track 2 (Food Security & Biodiversity):**
  - *Outcome lapangan:* Bukti nyata di kolam.
  - *Adopsi petani:* Siapa yang memakai di kolam (teknisi) vs siapa yang bayar (pemilik tambak).
  - *Supply chain:* Logistik rantai dingin dan waktu tunggu hasil.

### B. apt. Suci Utami Nurwidia, MSc (SoluSEA Venture Labs) — "Test Before You Build"
* **Aturan Eksperimen yang Jujur (Step 21):**
  - Satu asumsi, satu uji.
  - **Kriteria lulus ditulis LEBIH DULU sebelum uji dijalankan.** (Tanpa kriteria di awal, hasil apa pun akan dicocok-cocokkan seolah berhasil).
  - Uji termurah dan tercepat dulu (telepon petambak, cek harga reagen vendor).
  - Ukur perilaku nyata, bukan opini sopan ("Idenya bagus mas" $\rightarrow$ tidak bernilai).
* **Techno-Economic Analysis (TEA) Track 2:**
  - Rumus biaya unit: $(\text{CAPEX} + \text{OPEX}) \div \text{Output Sampel}$.
  - 4 penggerak biaya terbesar di Track 2: Sampling rantai dingin, utilisasi sampel per run sekuensing, frekuensi uji per siklus, dan biaya reagen di lokasi.
  - **Uji Sensitivitas $\pm 20\%$:** Buktikan margin tetap sehat saat biaya reagen naik 20%.

### C. Shelly Natalia (MIT Sloan Fellow) — "MVBP, Adoption & Scaling"
* **Prototype $\neq$ MVBP:**
  - *Prototype* hanya menguji kelayakan teknis (*apakah software/pipeline berjalan?*).
  - *Minimum Viable Business Product (MVBP)* menguji 3 hal: **Value** (pengguna dapat manfaat), **Pay** (ada yang membayar $> 0$), dan **Feedback Loop** (pengguna memberi masukan nyata).
* **Konsep "Concierge MVP":** Di awal tidak perlu serba otomatis 100%. Langkah lab manual dan pesan WhatsApp semi-manual sangat sah sebagai MVBP untuk memvalidasi nilai pasar sebelum membangun sistem otomatisasi mahal.

---

## 4. Tiga Artefak Wajib Bawa ke Hackathon (Jumat, 23 Oktober)

Sesuai Slide 23 Bootcamp, tiga dokumen ini dinilai langsung oleh juri mulai Submission Round I:

### 1. WORKSHEET 20.1: Matriks Asumsi Kunci AquaSeq (Terurut Risiko)

| No | Kategori | Asumsi Kunci | Dampak Bila Salah | Bukti yang Ada Hari Ini | Tingkat Risiko |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1** | **Pasar (Buyer)** | Pemilik tambak intensif mau membayar Rp 4,5 juta/kolam/siklus sebagai premi asuransi perlindungan modal Rp 100 juta. | **FATAL (Tinggi):** Model bisnis langganan gagal total. | Tipis (Sedang divalidasi via wawancara 4 petambak Jatim). | 🔴 **Risiko Kritis #1** |
| **2** | **Operasional (User)** | Teknisi tambak mau menyaring air 500 mL dan mengeksekusi instruksi aksi (potong pakan, sipon) dari WhatsApp. | **TINGGI:** Sistem tidak menghasilkan aksi nyata di kolam. | Sedang (Desain WhatsApp dibuat ramah satu jempol). | 🔴 **Risiko Kritis #2** |
| **3** | **Ekonomi (TEA)** | Biaya sekuensing Nanopore bisa ditekan ke Rp 300.000/sampel lewat multiplexing 75 sampel per flowcell. | **TINGGI:** COGS membengkak, margin tergerus di bawah 30%. | Kuat (Protokol Juanpere-Borràs et al., 2026 telah divalidasi). | 🟡 **Risiko Sedang** |
| **4** | **Teknis (Biologi)** | Pergeseran mikrobioma air kolam (disbiosis) mendahului gejala klinis mortalitas AHPND di udang. | **TINGGI:** Peringatan dini tidak memiliki *lead time*. | Kuat (Didukung jurnal Lu et al. 2023 & Xiong et al. 2024). | 🟢 **Risiko Rendah** |
| **5** | **Regulasi** | Layanan interpretasi bioinformatika software berbasis eDNA tidak memerlukan izin edar IVD alat kesehatan manusia. | **SEDANG:** Hambatan perizinan masuk pasar. | Kuat (Regulasi KKP/Kementan untuk diagnostik akuakultur non-obat). | 🟢 **Risiko Rendah** |

---

### 2. WORKSHEET 21.1–21.2: Rencana Uji Validasi Kilat 48 Jam (3 Asumsi Teratas)

* **Uji 1 (Asumsi Pembayar Rp 4,5 Juta):**
  - *Metode:* Menghubungi 4 pengelola tambak intensif di Banyuwangi–Situbondo via telepon/WA.
  - *Kriteria Lulus:* $\ge 3$ dari 4 pengelola menyatakan Rp 4,5 juta masuk akal dibandingkan risiko kehilangan modal Rp 100 juta.
* **Uji 2 (Asumsi Alur Kerja Teknisi WhatsApp):**
  - *Metode:* Menunjukkan mockup pesan WhatsApp AquaSeq kepada 3 teknisi kolam saat Problem Owner Clinic (Jumat 23 Okt).
  - *Kriteria Lulus:* $100\%$ teknisi memahami instruksi kerja dalam waktu $< 30$ detik tanpa bertanya istilah biologi.
* **Uji 3 (Asumsi Biaya Lab & Vendor):**
  - *Metode:* Konfirmasi ketersediaan flowcell MinION R10.4.1 dan reagen Native Barcoding ke vendor/lab mitra terdekat di Jatim.
  - *Kriteria Lulus:* Harga reagen per reaksi sesuai asumsi baseline TEA ($\pm 15\%$).

---

### 3. SKETSA TECHNO-ECONOMIC ANALYSIS (TEA) RESMI
* **Biaya per Unit (COGS 1 Kolam 100 Hari):** **Rp 2.200.000**
  - 3x Sekuensing Nanopore (Multiplex 75): **Rp 900.000**
  - 12x Uji qPCR Mingguan (3–5 Marka): **Rp 900.000**
  - 15x Filter Kit eDNA & Kurir Rantai Dingin: **Rp 400.000**
* **Harga Jual Paket Layanan:** **Rp 4.500.000**
* **Gross Profit Margin:** **51,1%**
* **Customer Payback Ratio (ROI):** **22,2x Lipat** ($\text{Rp 100 Juta} \div \text{Rp 4,5 Juta}$)
* **Uji Sensitivitas Reagen (+20%):** COGS naik jadi Rp 2,56 Juta $\rightarrow$ Margin tetap tebal di **43,1%**.

---

## 5. Strategi Meraih Skor Maksimal di Rubrik Penilaian Juri

### Target Kriteria E (Validasi & Bukti - Bobot 15%):
* Jangan mentok di **Skor 2** (hanya diskusi internal tim/mentor).
* Capai **Skor 3 atau 4** di Submission Round I (Sabtu 24 Okt 18.00):
  1. Catat nama 3–5 praktisi yang diwawancarai (atau mentor di Problem Owner Clinic).
  2. Tampilkan satu slide khusus di pitch deck: **"Field Validation & What We Learned"**.
  3. Masukkan 1 kutipan langsung petambak nyata:  
     *“Di tambak kami, kalau udang sudah berhenti makan di anco pakan, 48 jam kemudian biasanya kolam sudah habis. Kami butuh sinyal sebelum udang berhenti makan.” — [Nama Pengelola Tambak]*

### Target Kriteria D (Kelayakan Bisnis - Bobot 15%):
* Tampilkan tabel TEA per unit kolam yang detail (jangan cuma angka gelondongan).
* Tegaskan bahwa AquaSeq adalah model **Asset-Light Managed Service**: tidak perlu belanja modal (CAPEX) mesin sekuensing miliaran rupiah di awal; memanfaatkan kapasitas lab pengujian mitra.

### Target Kriteria G (Jalur ke Pasar & Skala - Naik jadi 15% di Final):
* **Beachhead:** 1.200 kolam intensif Banyuwangi–Situbondo (radius terjangkau dari Politeknik Negeri Jember).
* **Adjacency Growth (Mengikuti Konsep Step 14 Aulet):**
  - Pasar 1 (Beachhead): Tambak intensif mandiri di Jatim.
  - Pasar 2 (Same Product, New Channel): Kolam plasma binaan pabrik pakan / eFishery.
  - Pasar 3 (Same Customer, New Product): Sertifikasi mikrobioma untuk pembenihan (*hatchery*) dan klaim asuransi tambak.

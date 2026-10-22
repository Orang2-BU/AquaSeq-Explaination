# Skema Pembayaran Fleksibel, Pivot Lab qPCR-First, dan Data Sekunder
**Strategi Monetisasi Lapangan, Respons Feedback Lab, dan Triangulasi Data Pasar**
*AquaSeq — GenoHack 2026 ITB*

---

## 1. Pivot Kritis Berdasarkan Masukan Lab: "Nanopore Overkill untuk Rutin, Cukup qPCR!"

### Apa Kata Ahli Laboratorium?
Dalam wawancara validasi ke pihak laboratorium pengujian, terungkap masukan teknis krusial:
> *"Untuk mendeteksi penyakit udang secara rutin mingguan, penggunaan sekuensing Nanopore itu **terlalu overkill (berlebihan)** dari segi biaya dan waktu. Cukup menggunakan **qPCR** saja yang cepat, spesifik, dan murah!"*

### Bagaimana Respons & Pivot Cerdas AquaSeq? (Skor 4 Kriteria E)
Di hadapan juri venture, temuan ini **BUKAN KELEMAHAN**, melainkan bukti bahwa AquaSeq melakukan **Pivot / Penyesuaian Nyata Berdasarkan Masukan Ahli Lapangan** (persis seperti yang dicari juri di Kriteria E Skor 4: *“Asumsi diuji dengan bukti tertulis; ada pivot berdasarkan hasil”*).

#### Arsitektur Baru: "qPCR-First for Routine Surveillance + Nanopore On-Demand"
1. **Tier 1 — Monitoring Rutin Mingguan (100% qPCR-First):**
   - Untuk deteksi penyakit rutin (AHPND, WSSV, EHP, WFD), sistem mengandalkan **qPCR bertarget**.
   - Cepat (hasil 2–4 jam), biaya sangat murah (**Rp 75.000 – Rp 150.000 / tes**), dan akurat.
   - Tidak overkill, langsung menyelesaikan masalah petambak harian.
2. **Tier 2 — Profiling Komunitas & Investigasi Anomali (Nanopore On-Demand):**
   - Nanopore **TIDAK DIHAPUS**, melainkan ditempatkan pada fungsi aslinya yang paling bernilai:
     * **Awal Musim / Tebar (DOC 0):** Pemetaan awal keanekaragaman mikrobioma perairan kolam (memenuhi mandat *Track 2 Biodiversity* & baseline Shannon Index).
     * **Kasus Anomali (Unresolved Outbreak):** Jika udang menunjukkan gejala sakit/mati tapi semua tes qPCR negatif (artinya ada mutasi varian baru seperti kasus IMNV delesi 622 aa Situbondo 2018), Nanopore dikerahkan sebagai *deep investigative sequencing*.
3. **Dampak Finansial Positif:**
   - Menurunkan beban modal rutin petambak.
   - Memungkinkan hadirnya **Paket Panel qPCR** yang jauh lebih murah dan cepat diadopsi petambak kecil!

---

## 2. Bedah 9 Skema Pembayaran Fleksibel (Solusi Cash-Flow Petambak)

Petambak udang memiliki pola arus kas musiman: uang baru cair setelah panen (DOC 100–120). Menuntut bayar penuh di depan Rp 4,5 juta sering kali menjadi friksi penjualan.

Berikut adalah 9 skema pembayaran adaptif yang dirancang AquaSeq:

### 1. Bayar Per Tahap (Milestone-Based — Skema Standar Default)
* Petambak membayar setiap kali hasil analisis keluar, bukan di muka:
  - **Paket Panel (qPCR Focus):** $3 \times \text{Rp 1.000.000}$ (ditagih setelah hasil DOC 0, DOC 30, DOC 60).
  - **Paket Lengkap (qPCR + Nanopore):** $3 \times \text{Rp 1.500.000}$ (ditagih setelah hasil DOC 0, DOC 30, DOC 60).
* **Fitur Ramah Petani:** Petambak boleh berhenti di tengah jalan dan hanya membayar tahap yang hasilnya sudah diterima. Batas pelunasan 7 hari kerja setelah laporan diterima.

### 2. Paket Per Tambak: Biaya Dasar + Biaya Per Kolam (Khusus Tambak 2–4 Kolam)
* Biaya operasional kurir dan preparasi lab bersifat tetap per lokasi tambak. Maka harga dibuat fleksibel:
  - **Biaya Dasar Tambak:** **Rp 2.000.000 / siklus** (menutup 3x kunjungan sampling + preparasi lab).
  - **Biaya Tambahan Per Kolam:** **Rp 1.500.000 / kolam**.
* **Simulasi Perbandingan (Tambak Pak Gatot - 3 Kolam):**
  - *Jika murni per kolam:* $3 \times \text{Rp 4.500.000} = \mathbf{\text{Rp 13.500.000}}$ (terasa berat).
  - *Dengan Paket Per Tambak:* $\text{Rp 2.000.000} + (3 \times \text{Rp 1.500.000}) = \mathbf{\text{Rp 6.500.000 / siklus}}$!
  - Jauh lebih terjangkau bagi petambak mandiri, sementara margin AquaSeq tetap aman karena biaya kurirnya digabung.

### 3. Bayar Panen / Potong Panen (Harvest Deducted)
* **DP 20% di DOC 0:** Rp 600.000 (Panel) / Rp 900.000 (Lengkap) per kolam untuk menutup biaya reagen awal.
* **Pelunasan 80%:** Dilunasi saat panen melalui pemotongan hasil penjualan udang oleh offtaker, koperasi, atau agen pakan mitra.
* *Prinsip Keamanan:* AquaSeq **TIDAK** memberi piutang langsung ke petambak perorangan; transaksi dijamin oleh mitra yang memegang uang panen.

### 4. Cicilan Lewat Mitra Pembiayaan (Fintech / Pakan)
* AquaSeq dibayar lunas di depan oleh mitra pembiayaan (misalnya koperasi tambak, distributor pakan, atau program *eFishery Kabayan*).
* Petambak mencicil pembayaran ke mitra dengan mekanisme yang sudah biasa mereka gunakan untuk pembelian pakan dan benur.
* AquaSeq fokus pada analitik software, bukan menjadi agen penagih kredit.

### 5. Success Fee (Bayar Penuh Bila Panen Sukses)
* **Paket Panel:** Biaya dasar Rp 1.500.000 + Success fee Rp 1.500.000 bila panen tercapai tanpa mortalitas massal berat.
* **Paket Lengkap:** Biaya dasar Rp 2.000.000 + Success fee Rp 2.500.000 bila panen sukses.
* Skema terbaik untuk mengakuisisi 2 tambak percontohan pertama (*Lighthouse Customer*), membuktikan bahwa AquaSeq berani berbagi risiko dengan petambak.

### 6. Dibayar Pihak Ketiga (B2B2C Sponsorship / Bundling)
* **Perusahaan Pakan / Hatchery:** Layanan AquaSeq dibundel gratis ke dalam pembelian benur atau pakan volume tertentu. Petambak merasa gratis, AquaSeq ditagih ke pabrik pakan.
* **Eksportir / Pabrik Pengolahan:** Membiayai tes kolam plasma demi mengamankan kepastian pasokan udang bebas residu antibiotik.

### 7. Kontrak Tahunan Multi-Siklus (Annual Subscription)
* Kontrak berlangganan 3 siklus berturut-turut (1 tahun penuh) dengan harga terkunci.
* Diberikan diskon retensi 10% (misal Paket Lengkap 3 siklus $= \text{Rp 12.150.000}$ per kolam).
* Memberikan pendapatan berulang yang terprediksi (*predictable recurring revenue*) bagi AquaSeq.

### 8. Uji Coba Berbayar (Paid Trial — Bukan Gratisan)
* Dimulai dari 1–2 kolam percontohan dulu dalam 1 siklus dengan harga Paket Panel.
* Pengambilan sampel digabung dengan jadwal tambak tetangga agar hemat transportasi.
* Begitu petambak melihat manfaatnya, mereka menaikkan langganan ke seluruh kolam di siklus berikutnya.

### 9. Garansi Layanan (SLA Service Guarantee)
* Jika hasil pengujian terlambat melebihi waktu yang dijanjikan dalam SLA (misalnya $> 24$ jam untuk qPCR), biaya tahap tersebut didiskon 50% atau digratiskan.
* Membangun kepercayaan mutlak bagi petambak baru dengan risiko finansial yang sangat kecil bagi AquaSeq.

---

## 3. Triangulasi Data Sekunder & Validasi Pasar Nasional

Data eksternal resmi untuk memperkuat argumen di depan juri investor:

1. **Urgensi Kegagalan Panen Nyata di Indonesia:**
   - Studi komunitas petambak di Langnga, Pinrang membuktikan **hampir 100% petambak mengalami gagal panen akibat penyakit** sebelum udang berumur 1 bulan. Petambak kehabisan cara dan penyuluh tidak mampu memberi solusi dini.
2. **Data Sinyal Patogen Air Tambak (Riset CeKolam / Nusantics):**
   - Dari survei tambak nasional Indonesia, positivity rate elemen tambak: Pakan 43,26%, Udang 34,22%, Lumpur 24,46%, dan **Air Tambak 12,59%**.
   - *Jawaban ke Juri:* Air memang memiliki positivity rate lebih rendah dari pakan/lumpur, namun air adalah **medium bersama tanpa bedah udang (non-invasif)** yang mampu mendeteksi pergeseran stabilitas komunitas mikroba (disbiosis) sebelum udang mati.
3. **Kalender Musiman Penyakit Udang Indonesia:**
   - **EHP:** Puncak di bulan Januari & November.
   - **AHPND:** Puncak di bulan Juni – Agustus.
   - **IMNV:** Puncak di bulan Februari – Mei.
   - *Nilai Jual AquaSeq:* Kalender monitoring mingguan AquaSeq disesuaikan dengan pola musiman risiko penyakit setempat.
4. **Benchmark Harga Pengujian DNA Pasar:**
   - Biaya uji PCR resmi pemerintah (PMK 85/2023 BVet Banjarbaru): **Rp 500.000 / sampel**.
   - Tarif PCR lab komersial: **Rp 800.000 / sampel**.
   - Biaya qPCR lapangan percontohan Pak Gatot: **Rp 200.000 – Rp 250.000 / tes**.
   - *Kesimpulan:* Paket monitoring mingguan AquaSeq seharga **Rp 75.000 – Rp 100.000 / tes** berada jauh di bawah tarif eceran pasar berkat efisiensi pooling batch!

---

## 4. Kalimat Emas Pitching (Rekomendasi Kombinasi)

Saat juri bertanya: *"Petambak kecil mana mau bayar tunai di depan Rp 4,5 juta?"*

> *"Pak Juri, kami tidak pernah menjual putus dan tidak membebani petambak dengan biaya besar di depan.*  
> *Standar layanan kami berbasis **pembayaran bertahap (milestone-based)** setiap kali hasil tes keluar. Untuk petambak kecil 2–4 kolam, kami menghadirkan **Paket Per Tambak (Biaya Dasar + Per Kolam)** sehingga tambak 3 kolam hanya membayar Rp 6,5 juta, bukan Rp 13,5 juta.*  
> *Pelunasan dapat dilakukan melalui sistem **potong panen** lewat integrator atau koperasi mitra yang membiayai cicilannya. Dan berdasarkan masukan ahli lab, pemantauan rutin kami fokuskan pada **qPCR berbiaya hemat**, sementara Nanopore difokuskan on-demand untuk pemetaan awal musim dan investigasi varian baru. Dengan cara ini, risiko terbagi secara adil dan adopsi petambak terjamin lancar."*

# Kamus Hacker: Biologi Molekuler Diterjemahkan ke Konsep Komputer
**Buku Pegangan Hadi (Mahasiswa IT / Backend) untuk Memahami & Memakai Bahasa Saintifik di GenoHack 2026**

---

## 1. Mindset Utama: Kenapa Anak IT Justru Diuntungkan?
Biologi molekuler modern itu **sebenarnya adalah sistem komputasi**.
- DNA itu kode biner (cuma bedanya punya 4 huruf: A, T, C, G, alias 2-bit per karakter).
- Sel itu komputer biologis (CPU-nya ribosom, RAM-nya sitoplasma, ROM-nya genom).
- Penyakit itu seperti *malware* atau *DDoS attack*.

Saat lo pitch di depan juri, lo gak perlu sok-sokan jadi dokter hewan atau profesor biologi basah. Lo berdiri sebagai **Software & AI Architect** yang mengolah data genomik menjadi keputusan praktis petambak.

---

## 2. Tabel Translasi: Bahasa Biologi vs Bahasa Anak IT

| Istilah Saintifik / Biologi | Konsep di Dunia Komputer (IT) | Penjelasan Teknis & Contoh Kasus |
| :--- | :--- | :--- |
| **DNA / Genom** | **Source Code / Base Code / Biner** | Seluruh baris kode program dari satu makhluk hidup yang menentukan fungsi tubuhnya. |
| **Gen (Gene)** | **Fungsi / Method / Subroutine** | Satu potongan baris kode tertentu yang punya tugas spesifik (contoh: fungsi buat bikin racun). |
| **Plasmid (misal: pVA1)** | **Plugin Eksternal / DLL File / Payload USB** | Cincin DNA kecil di luar sistem operasi utama bakteri. Bakteri bisa mengunduh *plugin* ini dari luar. Jika plasmid pVA1 diunduh, bakteri ketambahan fungsi baru: memproduksi racun *pirAB*. |
| **Konjugasi (T4SS)** | **P2P File Sharing / Lateral Movement Malware** | Cara bakteri mentransfer file plasmid ke bakteri sebelahnya lewat koneksi langsung, mirip *worm* yang nyebar payload ke server tetangga di jaringan lokal. |
| **eDNA (Environmental DNA)** | **Log Telemetri / Server Dump di Jaringan** | Rekaman jejak yang ditinggalkan makhluk hidup di air. Lo gak perlu SSH masuk ke dalam tubuh udang; cukup baca dump log yang keluar di air kolam. |
| **16S rRNA Gene** | **MAC Address / SHA-256 Fingerprint Server** | Kode pengenal standar yang dimiliki semua bakteri. Ada kode vendor (bagian konstan) dan serial unik per spesies (daerah variabel V1–V9). |
| **Sekuensing Nanopore (MinION)** | **Wireshark Packet Sniffer (Promiscuous Mode)** | Alat yang menyadap dan membaca SEMUA paket data (urutan DNA) yang lewat di jaringan air kolam secara lengkap. |
| **qPCR (Quantitative PCR)** | **Grep Regex + Packet Counter Cepat** | Skrip regex yang cuma mencari 1 kata kunci spesifik dan menghitung berapa kali kata itu muncul dalam hitungan detik. Murah dan cepat. |
| **Data Komposisional (16S)** | **Grafik CPU Usage Persentase (Sum = 100%)** | Data yang cuma menunjukkan proporsi relatif. Kalau Proses B makan 90% CPU, Proses A otomatis tampak turun ke 10% di monitor, padahal beban kerja Proses A sebenarnya konstan. |
| **Transformasi CLR (Centered Log-Ratio)** | **Normalisasi Logaritmik / Standarisasi Skala** | Rumus matematika untuk menormalisasi data persentase relatif menjadi nilai absolut riil agar model machine learning tidak tertipu. |
| **Shannon Diversity Index ($H'$)** | **Shannon Entropy (Teori Informasi)** | Rumus yang persis sama dengan entropi kriptografi ($-\sum p \log p$). Mengukur seberapa acak dan beragamnya bit/spesies dalam satu sistem. |
| **Disbiosis (Dysbiosis)** | **Degraded State / Pre-Crash Anomaly di Server** | Kondisi server overload sebelum benar-benar tumbang (503 Service Unavailable). Udang belum mati, tapi sistem sudah mulai pincang. |
| **Profile HMM (Hidden Markov Model)** | **Fuzzy Regex / Signature Engine Antivirus** | Algoritma pencocokan pola probabilitas untuk menemukan varian racun mutasi yang urutan hurufnya sedikit berbeda dari aslinya. |
| **Stability Selection (Knapsack)** | **Greedy Knapsack Algorithm (Optimasi Biaya)** | Algoritma memilih 3–5 fitur marka terbaik yang memberi informasi terbanyak dengan batasan budget lab $\le \text{Rp 75.000}$. |
| **Ground Truth** | **Label Data Valid / Golden Dataset** | Kebenaran acuan mutlak di dunia nyata (contoh: konfirmasi udang benar-benar mati atau terbukti sakit lewat histopatologi lab). |

---

## 3. Cara Menggunakan Bahasa Saintifik di Depan Juri (Biar Gak Kaku)

### Skenario 1: Saat Menjelaskan Cara Kerja Produk (Slide 4)
* **Gaya Awam (Kurang Keren):** *"Kita ambil air, terus dicek bakterinya pakai alat, nanti keluar angka risikonya."* ❌
* **Gaya Hacker Profesional (Keren & Tepat Data):** 
  > *"Kami mengambil sampel **eDNA air kolam**, lalu melakukan pembacaan komunitas mikroba menggunakan **sekuensing Nanopore 16S amplikon**. Engine bioinformatika kami menerapkan **transformasi Centered Log-Ratio (CLR)** untuk mengeliminasi bias komposisional, mendeteksi gen virulensi **pirAB** melalui **Profile HMM**, lalu menghitung **Shannon Diversity Index** untuk memantau stabilitas ekosistem perairan."* ✔️

---

### Skenario 2: Saat Ditanya Kenapa Pakai Dua Alat (Nanopore + qPCR)
* **Gaya Awam:** *"Nanopore kan mahal kak, jadi kita campur sama qPCR yang murah."* ❌
* **Gaya Hacker Profesional:**
  > *"Secara arsitektur, Nanopore berfungsi sebagai **Discovery Layer** secara periodik untuk memetakan seluruh varian baru yang berpotensi lolos dari primer biasa. Setelah peta komunitas didapat, algoritma optimasi kami memilih 3 sampai 5 marka kritis untuk dipantau secara mingguan menggunakan **qPCR sebagai Monitoring Layer berbiaya rendah**."* ✔️

---

### Skenario 3: Saat Juri Menguji Latar Belakang IT Kalian
* **Pertanyaan Juri:** *"Kalian kan anak IT semua, kok berani-beraninya bikin platform diagnostik biologis?"*
* **Jawaban Skakmat Hadi:**
  > *"Justru di era modern ini, bottleneck terbesar genomik bukan lagi pada alat basahnya, melainkan pada **data interpretation dan pipeline komputasi**. Laboratorium basah sudah banyak di Jawa Timur, tapi mereka menghasilkan berkas FastQ mentah yang tidak dipahami petambak.*  
  > *Posisi tim kami adalah **software and intelligence layer**: mengotomatisasi QC, normalisasi CLR, scoring risiko terkalibrasi, hingga pengiriman rekomendasi aksi berbahasa Indonesia.*  
  > *Untuk protokol basah, kami mengadopsi model **asset-light** bermitra dengan BBPBAP Situbondo, dan validasi biologis didampingi oleh Dewan Penasihat praktisi patologi akuakultur."* ✔️

---

## 4. Tiga Istilah yang Sering Bikin Anak IT Kepleset & Solusinya

1. **Vibrio vs pirAB:**
   - *Jangan bilang:* "Bakteri Vibrio itu racun." (Salah, Vibrio itu nama bakteri, pirAB itu nama racunnya).
   - *Katakan:* "Bakteri *Vibrio parahaemolyticus* yang membawa gen racun *pirAB*."
2. **16S rRNA vs Virus:**
   - *Jangan bilang:* "Sekuensing 16S kami membaca virus IMNV dan White Spot." (Salah total, virus gak punya gen 16S).
   - *Katakan:* "16S membaca profil bakteri perairan, sedangkan target virus kami tangani menggunakan amplikon spesifik."
3. **Persentase vs Kuantitas Absolut:**
   - *Jangan bilang:* "Hasil qPCR kami menunjukkan Vibrio 12%." (Salah, persentase itu output sekuensing, qPCR menghasilkan angka salinan absolut/Ct).
   - *Katakan:* "Sekuensing memberi rasio kelimpahan relatif, sedangkan qPCR mengukur kuantitas absolut penanda terpilih."

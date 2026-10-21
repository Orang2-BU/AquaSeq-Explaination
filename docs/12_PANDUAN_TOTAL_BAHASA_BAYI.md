# Kitab Suci AquaSeq: Versi Bahasa Bayi (Literally Semuanya!)
**Ditulis Khusus Buat Hadi — Mahasiswa IT / Backend yang Pengen Paham 100% Tanpa Pusing Biologi**

---

## 1. Cerita Awalnya: "Masalah Apa Sih yang Mau Kita Selesain?"

Bayangin ada seorang bapak petambak udang di Banyuwangi atau Situbondo:
* Dia punya 1 petak kolam udang vaname (ukuran lapangan bola voli, isi 125.000 ekor anak udang/benur).
* Modal yang dia keluarin buat beli bibit, pakan karungan, listrik kincir air, dan obat-obatan selama 100 hari itu gede banget: **Rp 100 JUTA RUPIAH per kolam**!
* Kalau udangnya selamat sampai panen di hari ke-100, dia bisa jual udangnya seharga **Rp 180 Juta**. Untung bersih Rp 80 juta. Mantap kan?

**TAPI ADA SATU MIMPI BURUK PALING NGERI:**
Tiba-tiba di **hari ke-25**, udangnya kena penyakit bernama **AHPND** (atau nama beken petaninya: **EMS**).
* Penyakit ini ganasnya minta ampun: cuma butuh waktu 2 sampai 3 hari, **100% SEMUA UDANG DI KOLAM MATI MENGAMBANG!**
* Modal Rp 100 juta yang baru dikeluarin si bapak langsung **HANGUS JADI NOL RUPIAH** dalam semalam! Si bapak bisa bangkrut dan nangis darah.

---

## 2. Kenapa Udang Bisa Mati? (Biologi AHPND Versi Kartun)

* **Pelakunya siapa?** Bakteri bernama *Vibrio*.
* **Apakah semua bakteri Vibrio jahat?** GAK! Jutaan Vibrio itu bakteri biasa yang suka nongkrong di air payau. Gak bikin udang mati.
* **Terus kenapa bisa bikin mati?** 
  Karena ada sebagian Vibrio yang **bawa tas berisi pistol racun**!
  - Tas ranselnya namanya: **Plasmid pVA1**.
  - Pistol racun di dalem tasnya namanya: **pirA dan pirB** (disingkat **pirAB**).
* **Gimana cara racunnya bunuh udang?**
  Udang lagi berenang, gak sengaja nelen air yang ada bakteri bawa pistol tadi.
  Di dalem dada udang, ada organ pencernaan penting namanya **Hepatopankreas** (ini kayak gabungan lambung + hati + pankreas).
  Racun pirAB ini nembak dan **ngebolongin dinding hepatopankreas** udang kayak peluru! 
  Organ pencernaannya bolong-bolong, membusuk, udangnya gak bisa makan, lemas, terus mati massal.

---

## 3. Kenapa Alat Sensor Keren yang Ada Sekarang (Kayak JALA) Gagal Nyegah?

Petambak jaman sekarang udah pada beli sensor IoT canggih (contohnya merek **JALA**):
* Sensor JALA itu kayak **termometer dan tensimeter**. Dia cuma bisa ngecek: airnya panas gak? pH-nya asam gak? Oksigennya cukup gak?
* **Celah butanya:** Bakteri pembawa racun pirAB itu **GAK BIKIN AIR JADI PANAS ATAU ASAM!**
* Jadi di layar HP petambak, aplikasi JALA nampilin warna **HIJAU / NORMAL**. Air kelihatan jernih. Tapi di bawah air, bakterinya lagi pesta pora nembakin perut udang!
* Pas petambak sadar udangnya mati mengambang, itu udah terlambat. Gak bisa diobatin lagi.

---

## 4. Terus Solusi AquaSeq Itu Ngapain? (Motto 3 Jurus)

Motto kita: **"Sequencing to discover, qPCR to monitor, Bahasa Indonesia to act."**

Kita gak minta petani nangkap atau bedah udang (bikin udang stres). Kita cuma minta **saring 1 botol air kolam**:

1. **Jurus 1: Sequencing to Discover (CCTV 360 Derajat di Awal Bulan)**
   - Pas awal tebar (Hari ke-1, 30, 60), air kolam dicek pakai mesin sekuensing **Nanopore** di lab mitra.
   - Mesin ini kayak CCTV mall: dia ngedata SEMUA jenis bakteri yang ada di kolam.
   - Dari ratusan bakteri, sistem komputer AquaSeq milih: *"Oh, di kolam ini yang paling bahaya ada 3 sampai 5 bakteri buronan ini nih!"*
2. **Jurus 2: qPCR to Monitor (Metal Detector Murah Tiap Minggu)**
   - Nah, di minggu-minggu berikutnya (12 minggu berturut-turut), kita **GAK PERLU** sekuensing mahal lagi.
   - Kita cuma ngecek **3 sampai 5 bakteri buronan** tadi pakai tes **qPCR**.
   - qPCR ini kayak metal detector di pintu mall: cepet, presisi, dan murah banget (cuma Rp 75 ribu sekali tes).
3. **Jurus 3: Bahasa Indonesia to Act (Instruksi WhatsApp Siap Eksekusi)**
   - Kalau kondisi air mulai gak beres (disbiosis), sistem komputer kita gak ngirim laporan bahasa Inggris yang bikin pusing.
   - Sistem kita langsung nge-WA teknisi kolam pakai Bahasa Indonesia lugas:
     > *"Halo Pak Slamet, Kolam B-02 waspada Vibrio racun! Tolong kurangi pakan 20% dan sedot lumpur dasar sore ini!"*
   - Teknisi langsung ngerti dan bertindak hari itu juga. Udang selamat, panen aman!

---

## 5. Kamus Bahasa Bayi: Istilah Keren Jadi Bahasa Tongkrongan

| Istilah Keren | Apa Artinya Sebenarnya? | Bahasa Bayi / Analogi Gampang |
| :--- | :--- | :--- |
| **eDNA (Environmental DNA)** | DNA yang rontok ke air kolam. | **Remah biskuit di kasur / sidik jari di TKP.** Gak perlu bedah udang, cukup periksa airnya. |
| **16S rRNA** | Bagian DNA yang ada di semua bakteri. | **Plat nomor polisi / KTP bakteri.** Buat tahu siapa aja warga bakteri di kolam. |
| **Nanopore Sequencing** | Mesin baca urutan DNA lengkap. | **CCTV 360 derajat Full-HD.** Rekam semua orang yang lewat tanpa milih. |
| **qPCR** | Tes cepat penghitung target khusus. | **Metal detector di pintu mall.** Cuma bunyi kalau ada pistol spesifik. Murah & cepat. |
| **pirAB** | Gen racun penyebab AHPND. | **Pistol rakitan di kantong penjahat.** |
| **Disbiosis (Dysbiosis)** | Komposisi bakteri air mulai gak seimbang. | **Situasi komplek sebelum tawuran.** Warga baik ngurung diri, preman liar mulai ngumpul. |
| **Shannon Index** | Angka keragaman mikroba air kolam. | **Skor keseimbangan warga kota.** Kalau nilainya tinggi berarti warganya rukun & beragam. Kalau anjlok, berarti dikuasai preman. |
| **TEA (Techno-Economic Analysis)** | Analisis kelayakan biaya vs keuntungan. | **Hitungan modal vs untung jualan es teh.** Modal bahan berapa, dijual berapa, sisa untung berapa. |
| **Unit Economics** | Hitungan untung-rugi per satu kolam. | **Hitungan per porsi makanan.** Modal lab 2,2 juta, kita jual 4,5 juta, untung 2,3 juta per kolam. |

---

## 6. Hitung-Hitungan Duitnya (Kenapa Rp 4,5 Juta Bisa Tes 12 Minggu?)

Banyak orang bingung: *"Hah? Katanya qPCR ngetes tiap minggu, kok cuma bayar Rp 4,5 juta sekali di awal?"*

**Jawabannya:**
Petani **BUKAN BELI ECERAN**, tapi beli **PAKET KATERING ALL-YOU-CAN-EAT 100 HARI** seharga **Rp 4.500.000**.
Semua biaya lab selama 100 hari itu udah ditanggung di dalam modal kita (**COGS Rp 2.200.000**):

* **Biaya Nanopore (3x seumur hidup udang):** Rp 900.000  
  *(Alat aslinya mahal, tapi kita patungan bareng 75 kolam sekali jalan! Jadi per kolam cuma kena Rp 300rb × 3 = Rp 900rb).*
* **Biaya qPCR Mingguan (12 minggu berturut-turut):** Rp 900.000  
  *(Karena tiap minggu cuma ngecek 3–5 bakteri buronan, biaya cairannya cuma Rp 75rb per minggu. 12 × Rp 75rb = Rp 900rb).*
* **Biaya Saringan eDNA & Kurir Bensin:** Rp 400.000  
  *(15 saringan steril + ongkos kurir motor anter jemput air di Situbondo/Banyuwangi).*

**TOTAL MODAL KITA KE LAB = Rp 2.200.000.**  
**KITA JUAL KE PETANI = Rp 4.500.000.**  
**UNTUNG BERSIH KITA = Rp 2.300.000 (Margin 51% Cuan Tebal!).**

**Kenapa Petani Mau Beli?**  
Karena petani mikir gini: *"Gua keluar Rp 4,5 juta buat nyelamatin duit gua Rp 100 juta biar gak musnah. Itu untung 22 kali lipat!"*

---

## 7. Hubungan Kita sama JALA dan eFishery (Kawan atau Lawan?)

Kita **BUKAN LAWAN** mereka, kita adalah **TEMAN DUET MEREKA**:

* **Sama JALA:**
  - JALA itu **tensimeter** (ngukur suhu, pH, oksigen).
  - AquaSeq itu **tes lab darah** (ngukur bakteri racun di air).
  - Keduanya saling melengkapi! Data AquaSeq nanti ditempel ke aplikasi JALA lewat API.
* **Sama eFishery:**
  - eFishery itu jualan **mesin pelempar pakan otomatis** biar pakan gak boros.
  - eFishery juga punya program **Kabayan** (ngutangin pakan ke petani puluhan juta, bayarnya pas panen).
  - **Mimpi buruk eFishery:** Kalau udang petaninya mati kena AHPND, petaninya bangkrut dan **utang pakannya gak bisa dibayar!**
  - **AquaSeq jadi penyelamat:** eFishery bilang ke petani: *"Boleh ngutang pakan, asalkan kolamnya dijagain pakai AquaSeq biar udangnya gak mati dan utang lunas!"*

---

## 8. Kenapa Kita Anak IT Bisa Menang Walau Gak Ada Anak Biologi?

Kalau juri nanya: *"Kalian berenam kan anak komputer semua, kok berani bikin ginian?"*

**Jawaban Santai tapi Skakmat:**
> *"Pak Juri, di jaman sekarang, lab biologi basah itu udah banyak banget di Jawa Timur. Tapi masalahnya: lab itu cuma ngeluarin file data mentah huruf DNA yang tebel dan bikin petani pusing.*  
> *Peran tim kami adalah **bikin otaknya (Software & AI-nya)**: komputer kami yang nyaring data, ngitung skor bahayanya, milih bakteri mana yang harus dicek, dan ngirim WhatsApp bahasa Indonesia ke petani.*  
> *Urusan nyuntik dan ngetes di lab basah, kita tinggal kerja sama sama Balai Perikanan Situbondo (asset-light). Dan buat mastiin teorinya bener, kita dibimbing langsung sama Dewan Penasihat dokter hewan/pakar penyakit ikan!"*

---

## 9. Naskah Pitching 3 Menit Versi Super Lancar

1. **Detik 0–30 (Masalah):**  
   "Petambak udang di Jatim keluar modal 100 juta per kolam. Tapi dalam 25 hari, duit itu bisa ludes 100% jadi nol gara-gara wabah AHPND. Sensor IoT yang ada cuma ngecek suhu dan pH, gak bisa liat bakteri racun."
2. **Detik 30–90 (Solusi):**  
   "Kenalkan AquaSeq: Sistem pelengkap cerdas berbasis DNA air. Cukup saring air kolam. Di awal kita petakan semua bakteri pakai Nanopore, terus tiap minggu kita pantau 3-5 bakteri paling bahaya pakai qPCR murah. Kalau bahaya, langsung kirim WA bahasa Indonesia ke teknisi buat kurangi pakan dan sedot lumpur."
3. **Detik 90–140 (Biodiversitas & Bisnis):**  
   "Sesuai Track 2, kita juga pantau keragaman hayati mikroba air pakai Shannon Index biar ekosistem laut gak rusak kena antibiotik liar. Bisnisnya: Petani langganan 4,5 juta per siklus, modal lab kita cuma 2,2 juta karena patungan 75 sampel. Kita dapet margin 51%, petani dapet proteksi aset 22x lipat."
4. **Detik 140–180 (Roadmap & Penutup):**  
   "Prototipe kita udah jalan di TRL 3 pakai dataset publik NCBI air tambak vaname. 12 bulan ke depan kita uji pilot di 2 tambak Jatim bareng Balai Situbondo. Bersama AquaSeq, kita amankan panen udang dan devisa pangan maritim Indonesia. Terima kasih!"

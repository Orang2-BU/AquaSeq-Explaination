# Kamus Istilah AquaSeq: Bahasa Manusia & Analogi Tongkrongan
**GenoHack 2026 — Dibuat untuk Software Engineers yang Masih Awam Biologi**

Dokumen ini adalah "kamus sakti" buat lo. Saat juri melontarkan istilah-istilah ilmiah rumit, lo gak bakal bengong karena lo udah paham analogi dan esensinya.

---

## DAFTAR ISTILAH BIOLOGI & GENOMIK

### 1. eDNA (Environmental DNA)
* **Apa artinya di lab?** DNA yang tertinggal dan melayang bebas di air, tanah, atau udara yang rontok dari organisme hidup lewat feses, lendir, sel kulit, atau jasad renik.
* **Analogi Sehari-hari:** 🍪 **Remah biskuit di sofa atau sidik jari maling di gagang pintu.** Lo gak perlu gerebek malingnya di tempat buat tahu dia pernah masuk rumah; cukup periksa sidik jari yang dia tinggalin.
* **Kenapa AquaSeq pakai ini?** Karena kita gak perlu nangkep atau bedah udang satu-satu. Cukup ambil 1 liter air kolam, saring, dan periksa DNA-nya. Non-invasif dan ramah udang.

### 2. Gen 16S rRNA
* **Apa artinya di lab?** Gen penyandi RNA ribosom subunit kecil yang ada pada SEMUA bakteri dan arkea. Memiliki bagian konstan (sama pada semua bakteri) dan daerah variabel V1–V9 (berbeda pada tiap spesies).
* **Analogi Sehari-hari:** 🪪 **Plat nomor polisi atau KTP bakteri.** Huruf depannya kode wilayah (bagian konstan), nomor tengahnya identitas unik pemiliknya (daerah variabel).
* **PENTING (Jebakan Juri!):** Virus (seperti IMNV atau WSSV) **TIDAK PUNYA** gen 16S rRNA karena virus bukan makhluk bersel dan gak punya ribosom. Kalau juri nanya *"16S kalian bisa deteksi virus white spot?"*, jawab tegas: *"Tidak bisa, 16S khusus bakteri. Untuk virus kami pakai amplikon primer target khusus."*

### 3. pirAB & Plasmid pVA1
* **Apa artinya di lab?** Gen pembawa racun biner (*PirA* dan *PirB*) penyebab nekrosis hepatopankreas akut (AHPND). Gen ini terletak di cincin DNA ekstra-kromosomal bernama plasmid pVA1.
* **Analogi Sehari-hari:** 💣 **Senjata api rakitan di saku.** Bakteri *Vibrio* biasa itu kayak orang nongkrong biasa. Tapi kalau dia nemu pistol (plasmid pVA1 dengan gen pirAB), dia berubah jadi penembak jitu mematikan.
* **Kenapa Penting?** Menghitung nama bakteri doang gak cukup. Jutaan bakteri Vibrio bisa jadi gak berbahaya kalau gak punya gen pirAB. AquaSeq fokus mendeteksi gen senjatanya!

### 4. Dysbiosis (Disbiosis)
* **Apa artinya di lab?** Kondisi ketidakseimbangan komunitas mikrobioma normal, ditandai dengan penurunan bakteri probiotik alami dan lonjakan bakteri patogen oportunistik.
* **Analogi Sehari-hari:** ⚖️ **Situasi komplek perumahan sebelum tawuran.** Warga baik-baik mendadak ngurung diri, preman liar mulai berkerumun di gang. Belum ada rumah yang dibakar, tapi tanda-tanda bencana sudah jelas.
* **Kenapa Disebut Peringatan Dini?** Disbiosis terjadi **beberapa hari sebelum udang mati**. Di fase ini petambak masih bisa bertindak (ganti air, kurangi pakan, tambah aerasi).

### 5. Mikrobioma (Microbiome)
* **Apa artinya di lab?** Seluruh kumpulan mikroorganisme (bakteri, virus, jamur, protozoa) beserta materi genetiknya yang hidup di satu ekosistem tertentu (usus udang atau air tambak).
* **Analogi Sehari-hari:** 🏙️ **Seluruh populasi warga di satu kota metropolitan.** Ada polisi (probiotik), pedagang biasa (bakteri komensal pengurai), dan kriminal (patogen).

---

## DAFTAR ISTILAH TEKNOLOGI & LAB

### 6. Nanopore Sequencing (Oxford Nanopore Technologies / MinION)
* **Apa artinya di lab?** Teknologi pembacaan sekuens DNA untai tunggal generasi ketiga melalui pori protein mikroskopis (nanopori). Perubahan arus listrik diterjemahkan menjadi huruf A, T, C, G.
* **Analogi Sehari-hari:** 📹 **CCTV 360 derajat Full-HD di seluruh penjuru kota.** Dia merekam siapa saja yang lewat tanpa milih-milih.
* **Peran di AquaSeq:** Dipakai secara berkala (tiap 2–4 minggu) untuk **"Discover"** (menemukan varian atau ancaman baru yang belum terdaftar di tes biasa). Biaya ditekan murah lewat multiplexing 75 sampel per flowcell.

### 7. qPCR (Quantitative / Real-Time PCR)
* **Apa artinya di lab?** Teknik penggandaan DNA secara eksponensial dengan penanda fluoresen, mengukur konsentrasi absolut target spesifik secara cepat dalam hitungan jam.
* **Analogi Sehari-hari:** 🚨 **Metal detector khusus di pintu mall.** Alat ini gak peduli lo bawa baju apa, dia cuma berbunyi kalau ada logam tertentu. Murah, cepat, akurat.
* **Peran di AquaSeq:** Dipakai mingguan untuk **"Monitor"** 3–5 marka kritis hasil rekomendasi Nanopore.

### 8. Multiplexing & Barcode DNA
* **Apa artinya di lab?** Menempelkan label urutan basa pendek unik (barcode) pada tiap sampel, sehingga puluhan sampel dari tambak berbeda bisa dimasukkan dan dibaca bersamaan dalam 1 alat flowcell sekuensing.
* **Analogi Sehari-hari:** 🏷️ **Nomor resi paket JNE dalam satu truk kontainer.** Satu truk bawa ratusan paket dari orang berbeda, tapi pas dibongkar gak bakal tertukar karena punya resi masing-masing. Ini rahasia kenapa biaya sekuensing AquaSeq bisa sangat murah!

---

## DAFTAR METRIK BIODIVERSITAS (KARTU TRUF TRACK 2)

### 9. Shannon Diversity Index ($H'$)
* **Apa artinya?** Indeks yang mengukur keanekaragaman dan kemerataan spesies mikroba. Semakin tinggi nilainya, semakin seimbang dan tahan banting ekosistemnya.
* **Analogi:** Kelas sekolah di mana 30 muridnya punya hobi berbeda-beda secara merata ($H'$ tinggi). Kalau 29 anak hobinya main game dan cuma 1 yang belajar, nilainya anjlok ($H'$ rendah).
* **Kapan Dibahas?** Ketika juri Track 2 nanya: *"Mana aspek biodiversity-nya?"* Lo jawab: *"Kami memantau Shannon Index air kolam. Keruntuhan indeks ini adalah sinyal awal stres ekologis."*

### 10. Chao1 Richness Estimator
* **Apa artinya?** Estimasi kekayaan total jenis mikroba di suatu tempat, termasuk spesies langka yang belum sempat terbaca oleh mesin.
* **Analogi:** Menaksir berapa total spesies burung di hutan lebat berdasarkan jumlah burung yang cuma terlihat 1 kali atau 2 kali oleh peneliti.

### 11. Bray-Curtis Dissimilarity
* **Apa artinya?** Metrik *beta diversity* untuk menghitung seberapa jauh perbedaan komposisi komunitas mikroba antara Kolam A vs Kolam B, atau Kolam A Minggu ke-1 vs Minggu ke-4.
* **Skala Nilai:** 0 artinya identik persis, 1 artinya berbeda 100% tanpa satupun mikroba yang sama.

---

## DAFTAR ISTILAH BISNIS & VENTURE

### 12. TEA (Techno-Economic Analysis)
* **Apa artinya?** Analisis gabungan antara kelayakan proses rekayasa sains dengan neraca keuangan (CAPEX, OPEX, COGS, harga jual, payback period).
* **Analogi:** Hitung-hitungan pedagang martabak: Berapa harga terigu, telur, gas elpiji per loyang, dijual berapa, dan berapa lama sampai gerobaknya lunas.

### 13. COGS (Cost of Goods Sold) / HPP
* **Apa artinya?** Total biaya langsung untuk memproduksi 1 unit layanan. Di AquaSeq: Biaya reagen Nanopore + reagen qPCR + membran filter eDNA + ongkos kurir per kolam.
* **Angka AquaSeq:** **Rp 2.200.000 per kolam per siklus**.

### 14. Gross Margin
* **Rumus:** $(Harga Jual - COGS) \div Harga Jual \times 100\%$
* **Angka AquaSeq:** $(Rp 4,5 jt - Rp 2,2 jt) \div Rp 4,5 jt = \mathbf{51\%}$.
* **Arti bagi Juri Investor:** Bisnis ini sehat dan punya ruang keuntungan tebal untuk ekspansi tim dan teknologi.

### 15. Moat (Parit Pertahanan Bisnis)
* **Apa artinya?** Keunggulan unik yang membuat produk lo sangat sulit ditiru oleh raksasa seperti JALA atau laboratorium kampus.
* **Moat AquaSeq:**
  1. *Dynamic Marker Optimization Algorithm:* Algoritma pemilihan 3–5 penanda paling hemat biaya.
  2. *Proprietary Microbial Pond Baseline:* Database profil normal air tambak pesisir Indonesia berdasarkan umur tebar (DOC).

# Killer Q&A Defense: Menjawab Pertanyaan Paling Berbahaya Juri
**Bocoran Pertanyaan Panel Juri GenoHack 2026 & Jawaban Skakmat Berintegritas Tinggi**

---

### Q1: "Sampel air kolam kan berbeda dari usus udang. Bagaimana kalian bisa yakin eDNA air mencerminkan kondisi riil di dalam tubuh udang?"
* **Kenapa juri nanya ini?** Karena proposal riset sebelumnya banyak meneliti sampel isi usus (*gut microbiome*), bukan air bebas. Juri ingin tahu apakah kalian cuma berhalusinasi atau baca jurnal terkini.
* **Jawaban Mantap:**
  > *"Pertanyaan yang sangat krusial, dewan juri. Dasar pemikiran kami merujuk pada temuan Lu et al. (2023) dalam Applied Microbiology and Biotechnology, yang menunjukkan bahwa seiring berkembangnya penyakit AHPND, struktur mikrobioma usus udang mengalami keruntuhan dan konvergen—yaitu komposisinya menjadi sangat mirip dengan mikrobioma air kolam pemeliharaan.*
  > *Namun kami sangat jujur: acuan kebenaran akhir (ground truth) kami bukanlah isi usus, melainkan angka mortalitas dan konfirmasi penyakit di kolam nyata. Menguji tingkat korelasi sensitivitas antara eDNA air dan mortalitas lapangan adalah kriteria sukses eksplisit pada fase validasi retrospektif dan pilot TRL 4–5 kami."*

---

### Q2: "Kenapa tidak pakai Deep Learning mutakhir (Transformer/LLM) untuk mesin prediksi risikonya?"
* **Kenapa juri nanya ini?** Juri teknis sering menguji apakah kalian cuma "ikut tren AI" atau paham karakteristik data biologi.
* **Jawaban Mantap:**
  > *"Untuk tahap saat ini, data mikrobioma air tambak berlabel dengan luaran penyakit yang jelas masih berjumlah terbatas (skala puluhan hingga ratusan sampel). Memaksakan arsitektur deep learning justru kontraproduktif karena akan mengalami overfitting parah dan bertindak sebagai kotak hitam (black box).*
  > *AquaSeq dirancang sebagai alat pendukung keputusan yang harus dipercaya petambak. Oleh karena itu kami memilih model ter-regularisasi (Elastic Net) dan Profile HMM untuk gen virulensi: model ini terbukti tangguh pada data komposisional kecil, koefisien fiturnya dapat diinterpretasikan secara transparan (explainable AI), serta divalidasi dengan metode leave-one-pond-out untuk mencegah kebocoran data.*
  > *Deep learning baru akan kami kaji setelah bank data dari fase pilot terkumpul dalam volume ribuan sampel."*

---

### Q3: "Sekuensing itu mahal. Petambak kecil di desa mana sanggup bayar 4,5 juta rupiah?"
* **Kenapa juri nanya ini?** Juri venture ingin memastikan kalian punya pemahaman pasar nyata (*market reality*), bukan cuma mimpi idealis di atas kertas.
* **Jawaban Mantap:**
  > *"Tepat sekali, itulah mengapa strategi Go-To-Market kami terbagi menjadi dua tahap.*
  > *Pelanggan awal (beachhead) kami bukanlah petambak tradisional berskala kecil, melainkan tambak intensif dan korporasi integrator (seperti pabrik pakan dan pembenihan hatchery) yang mengelola modal ratusan juta hingga miliaran rupiah per siklus. Bagi mereka, biaya 4,5 juta adalah premi asuransi yang sangat rasional untuk melindungi modal 100 juta rupiah.*
  > *Untuk petambak kecil, jalur penetrasinya adalah melalui program kemitraan integrator pakan atau koperasi perikanan, di mana pemantauan eDNA dilakukan secara kolektif (pooled sampling) pada saluran pasok air bersama, sehingga beban biaya per petani turun drastis menjadi hanya ratusan ribu rupiah."*

---

### Q4: "Semua anggota tim kalian berlatar belakang komputasi/software. Siapa yang menangani uji laboratorium basah (wet-lab)?"
* **Kenapa juri nanya ini?** Proposal kalian menunjukkan 6 mahasiswa/dosen IT. Juri meragukan eksekusi biologinya.
* **Jawaban Mantap:**
  > *"Core value AquaSeq berakar pada software layer: engine analitik, seleksi marka dinamis, dan sistem penerjemah peringatan berbahasa Indonesia. Kami secara sengaja mengadopsi model kemitraan asset-light: proses ekstraksi sampel, sekuensing Nanopore, dan uji qPCR dialihdayakan ke laboratorium mitra pengujian terakreditasi di Jawa Timur, seperti Balai Perikanan Budidaya Air Payau (BBPBAP) Situbondo dan laboratorium mikrobiologi perguruan tinggi terdekat.*
  > *Selain itu, untuk menjamin validitas protokol biologi dan rekomendasi tindakan budidaya, kami menggandeng praktisi patologi perikanan sebagai Dewan Penasihat (Advisory Board) tim kami, yang sekaligus memastikan tim inti kami tetap patuh pada batas aturan 6 anggota lomba."*

---

### Q5: "Apakah sistem kalian bisa menemukan varian virus baru yang bermutasi?"
* **Kenapa juri nanya ini?** Proposal awal kalian menyebut "discover emerging pathogens", padahal 16S amplikon punya batas ilmiah.
* **Jawaban Mantap:**
  > *"Kami ingin mengklarifikasi batasan ilmiah prototipe kami secara jujur: sekuensing 16S amplikon bertarget difokuskan untuk mendeteksi dan memetakan bakteri serta marka virulensi yang sudah dirancang primernya (seperti gen racun pirAB). 16S tidak menangkap virus RNA/DNA.*
  > *Untuk varian gen bakteri yang menyimpang, kami menggunakan Profile HMM. Namun untuk penemuan patogen baru yang belum pernah terpetakan sama sekali (novel pathogens), dibutuhkan alur shotgun metagenomics tanpa amplikon. Jalur shotgun ini telah kami rancang dalam peta arsitektur jangka panjang pada roadmap TRL 6."*

---

### Q6: "Apa bedanya kalian dengan JALA yang aplikasinya sudah dipakai ribuan petambak?"
* **Kenapa juri nanya ini?** JALA adalah raksasa farm-management di Indonesia. Juri ingin tahu apakah kalian mau bunuh diri melawan mereka.
* **Jawaban Mantap:**
  > *"JALA adalah pionir luar biasa dalam digitalisasi operasional tambak di Indonesia. Namun fokus JALA berada pada parameter fisika-kimia air (pH, salinitas, oksigen) serta manajemen logistik pakan. JALA tidak memiliki lapisan biological/genomic monitoring.*
  > *Oleh karena itu, posisi AquaSeq bukan sebagai kompetitor, melainkan mitra sinergis. Visi komersial kami adalah mengintegrasikan AquaSeq Engine ke dalam aplikasi JALA melalui API terbuka, sehingga petambak pengguna JALA dapat mengaktifkan modul 'Genomic Disease Surveillance' sebagai layanan bernilai tambah."*

---

### Q7: "Nilai Shannon Index kolam turun dari 2,5 jadi 1,4. Apakah kolam itu PASTI terkena wabah penyakit?"
* **Kenapa juri nanya ini?** Menguji apakah kalian paham ekologi mikroba atau cuma menganggap Shannon sebagai "skor biner".
* **Jawaban Mantap:**
  > *"Tentu tidak otomatis berarti penyakit, dewan juri. Keanekaragaman mikroba secara alami dapat berfluktuasi akibat umur budidaya (DOC), perubahan salinitas air, cuaca hujan, maupun aplikasi probiotik rutin.*
  > *Itulah sebabnya sistem AquaSeq tidak membaca Shannon Index secara terisolasi. Penurunan keragaman diperlakukan sebagai sinyal peringatan awal yang harus dikonfirmasi silang dengan Bray-Curtis Beta Diversity untuk melihat arah pergeseran komunitas, rasio logaritmik bakteri penyeimbang vs oportunis, serta keberadaan marka spesifik seperti pirAB. Ini adalah sistem pendukung keputusan holistik, bukan kesimpulan sepihak."*

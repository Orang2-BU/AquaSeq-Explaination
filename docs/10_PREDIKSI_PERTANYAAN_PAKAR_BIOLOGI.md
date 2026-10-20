# Prediksi Pertanyaan Kritis Pakar Biologi & Genomik (Track 2)
**Simulasi Serangan Dosen / Peneliti Senior di GenoHack 2026 & Format Jawaban Skakmat**

---

## Profil & Sudut Pandang Juri Biologi Track 2
Sebagai pakar biologi molekuler, patologi akuakultur, dan ekologi mikroba, juri ini **tidak bisa dibodohi dengan istilah keren AI**. Dia tahu persis bahwa:
1. Air kolam dan perut udang itu ekosistem yang berbeda.
2. 16S rRNA punya batasan resolusi dan tidak bisa membaca virus.
3. Data sekuensing itu relatif (komposisional), bukan angka absolut.
4. Air tambak payau penuh lumpur inhibitor yang bisa menggagalkan PCR.

Di bawah ini adalah **8 pertanyaan terganas yang pasti dilontarkan juri biologi**, lengkap dengan anatomi serangannya, jebakan maut, dan **Format Jawaban Skakmat (Metode PREP: Point - Reason - Evidence - Plan)**.

---

### SERANGAN 1: Air Kolam vs Usus Udang (The Core Biological Gap)
* **Pertanyaan Juri:**  
  *"Kalian mengambil sampel eDNA dari air kolam. Tapi AHPND itu menginfeksi dan merusak organ hepatopankreas di dalam tubuh udang, bukan di air. Penelitian Rajonhson et al. (2024) di Thailand membuktikan bahwa niche sampel (usus vs air vs sedimen) menjelaskan 56% variasi mikrobioma—artinya mikrobioma usus dan air itu sangat berbeda! Bagaimana kalian bisa yakin eDNA air bisa mendeteksi AHPND sebelum udangnya mati, bukan setelah bangkainya membusuk dan mencemari air?"*
* **Anatomi Serangan:** Juri ingin tahu apakah kalian paham perbedaan biologis organ inang vs air lingkungan, atau cuma berhalusinasi menyamakan keduanya.
* **Jebakan Maut (JANGAN JAWAB INI):** ❌ *"Air dan usus udang itu sama aja kok pak, kan udang hidup di air."* (Juri langsung memberi nilai 1 untuk pemahaman biologis).
* **Format Jawaban Skakmat Hadi (PREP):**
  - **Point:** *"Kami sepenuhnya sepakat bahwa pada kondisi kolam normal yang sehat, mikrobioma usus udang dan air kolam memiliki struktur taksa yang berbeda signifikan."*
  - **Reason:** *"Namun, hipotesis peringatan dini kami bersandar pada fenomena biologis saat infeksi mulai terjadi: permeabilitas membran hepatopankreas rusak, udang mengalami regurgitasi, shedding sel bakteri, dan pelepasan DNA lingkungan meningkat ke kolom air."*
  - **Evidence:** *"Hal ini didukung oleh temuan Lu et al. (2023) dalam Applied Microbiology and Biotechnology, yang membuktikan bahwa seiring progresivitas AHPND, komunitas mikrobioma usus udang mengalami keruntuhan dan konvergen—yaitu strukturnya makin menyerupai komunitas air pemeliharaan."*
  - **Plan (Batasan Jujur):** *"Namun kami tidak mengasumsikan korelasi ini mutlak. Ground truth kami bukanlah usus, melainkan kejadian mortalitas klinis kolam. Menguji sensitivitas eDNA air terhadap kejadian mortalitas nyata adalah target utama uji retrospektif dan pilot lapangan TRL 4–5 kami."*

---

### SERANGAN 2: Batasan 16S rRNA terhadap Virus RNA/DNA & Resolusi Spesies
* **Pertanyaan Juri:**  
  *"Kalian mengutip kasus wabah IMNV di Situbondo 2018 dengan mutasi delesi 622 asam amino sebagai latar belakang. Tapi IMNV itu virus RNA dan WSSV itu virus DNA, keduanya TIDAK punya gen 16S rRNA ribosom! Selain itu, 16S V3-V4 sering kali hanya mampu mengidentifikasi sampai tingkat genus (Vibrio sp.), tidak bisa membedakan V. parahaemolyticus dengan Vibrio non-patogen lainnya. Bagaimana sistem kalian membuktikan ini bukan false discovery?"*
* **Anatomi Serangan:** Menguji apakah kalian paham taksonomi dasar: bakteri punya ribosom (punya 16S), virus tidak punya ribosom (tidak punya 16S).
* **Jebakan Maut:** ❌ *"Pipeline 16S kami sudah dilatih mendeteksi semua virus udang."* (Blunder memalukan; kalian akan ditertawakan panel juri).
* **Format Jawaban Skakmat Hadi (PREP):**
  - **Point:** *"Tepat sekali dewan juri, gen 16S rRNA secara biologis eksklusif hanya ada pada bakteri dan arkea, sehingga 16S mustahil mendeteksi virus seperti IMNV atau WSSV."*
  - **Reason:** *"Itulah alasan mengapa desain alur kerja AquaSeq tidak mengandalkan 16S tunggal, melainkan menggabungkan 16S untuk memetakan komunitas bakteri DENGAN panel amplikon primer bertarget khusus untuk gen virulensi dan penanda virus RNA/DNA."*
  - **Evidence:** *"Terkait resolusi spesies Vibrio, literatur Waiho et al. (2023) membuktikan 16S pendek memang terbatas di tingkat genus. Oleh karena itu, AquaSeq menyertakan primer amplikon gen virulensi toksin pirAB. Jadi kami tidak mendiagnosis penyakit berdasarkan genus Vibrio saja, melainkan keberadaan gen racun spesifiknya."*
  - **Plan:** *"Untuk deteksi varian virus baru secara de-novo tanpa amplikon, kami telah memetakan jalur shotgun metagenomics pada roadmap jangka panjang TRL 6."*

---

### SERANGAN 3: DNA Hidup vs DNA Bebas (Free-Floating eDNA dari Sel Mati)
* **Pertanyaan Juri:**  
  *"Air tambak intensif sering diberi perlakuan klorinasi atau hidrogen peroksida saat persiapan air, yang membunuh jutaan bakteri tapi meninggalkan sisa DNA bebas (free-floating eDNA) yang stabil berminggu-minggu di air payau. Bagaimana kalian bisa yakin eDNA pirAB yang kalian deteksi berasal dari bakteri hidup aktif yang mengancam udang, bukan DNA rontokan bakteri mati?"*
* **Anatomi Serangan:** Menyerang kelemahan klasik eDNA: mendeteksi DNA tidak sama dengan mendeteksi organisme hidup (*viable cells*).
* **Jebakan Maut:** ❌ *"eDNA kami pasti dari bakteri hidup karena airnya segar."*
* **Format Jawaban Skakmat Hadi (PREP):**
  - **Point:** *"Pertanyaan yang sangat tajam. eDNA memang mencerminkan keberadaan materi genetik, baik dari sel utuh maupun DNA bebas."*
  - **Reason:** *"Untuk membedakan sinyal pasif dari ancaman aktif, AquaSeq tidak menggunakan satu titik sampling tunggal, melainkan membaca dinamika deret waktu (time-series slope) dan rasio komposit."*
  - **Evidence:** *"DNA bebas dari organisme mati mengalami degradasi eksponensial di air payau tropis bersuhu 29–31°C akibat aktivitas enzim nuklease alami dan sinar UV matahari. Jika pirAB berasal dari residu mati, sinyalnya akan meluruh menurun. Sebaliknya, infeksi aktif ditandai oleh peningkatan salinan pirAB pada qPCR mingguan beruntun yang berkorelasi dengan penurunan Shannon Diversity Index."*
  - **Plan:** *"Pada protokol lab basah TRL 4, kami juga mengevaluasi penambahan perlakuan Propidium Monoazide (PMAxx) sebelum lisis untuk mengikat DNA bebas sel mati agar tidak teramplifikasi."*

---

### SERANGAN 4: Fluktuasi Alami Shannon Index vs Stres Disbiosis
* **Pertanyaan Juri:**  
  *"Kalian memasukkan Shannon Index dan Chao1 untuk memenuhi syarat Track 2 Biodiversity. Tapi studi Puspitasari et al. (2025) di Indramayu yang kalian kutip sendiri menunjukkan bahwa mikrobioma kolam bergeser secara alami di minggu ke-6 karena faktor salinitas dan akumulasi pakan. Bagaimana kalian membedakan pergeseran ekologi alami menurut umur tebar (DOC) dengan disbiosis akibat serangan penyakit?"*
* **Anatomi Serangan:** Juri ingin memastikan kalian tidak menganggap penurunan Shannon Index sebagai "tombol vonis mati udang".
* **Jebakan Maut:** ❌ *"Pokoknya kalau Shannon turun di bawah 2, kolam pasti kena AHPND."*
* **Format Jawaban Skakmat Hadi (PREP):**
  - **Point:** *"Kami sepenuhnya sadar bahwa keragaman mikrobioma air tambak dinamis dan berubah mengikuti umur budidaya (DOC), salinitas, dan aplikasi probiotik."*
  - **Reason:** *"Oleh karena itu, AquaSeq tidak menggunakan ambang batas Shannon statis tunggal untuk seluruh umur kolam. Sistem kami membandingkan metrik keragaman terhadap Baseline Kolam Lokal pada DOC yang sama."*
  - **Evidence:** *"Penurunan Shannon diperlakukan sebagai sinyal awal (early flag) yang wajib dikonfirmasi silang dengan: (1) Bray-Curtis Beta Diversity untuk melihat arah pergeseran taksa, (2) Log-ratio taksa menguntungkan seperti Rhodobacteraceae vs Vibrionaceae, dan (3) Ada tidaknya konfirmasi gen toksin pirAB."*
  - **Plan:** *"Dengan pendekatan multi-layer ini, perubahan alami akibat pakan tidak akan memicu alarm palsu (false positive) bagi petambak."*

---

### SERANGAN 5: Read Error Nanopore & Pembengkakan Palsu Chao1
* **Pertanyaan Juri:**  
  *"Estimator Chao1 sangat sensitif terhadap singletons (F1) dan doubletons (F2)—yaitu taksa yang hanya terbaca 1 atau 2 kali. Oxford Nanopore terkenal memiliki raw read error rate yang lebih tinggi dibanding Illumina (meski sudah pakai kimia V14). Error sekuensing ini bisa menciptakan OTU palsu sehingga Chao1 membengkak liar. Bagaimana pipeline komputasi kalian menangani ini?"*
* **Anatomi Serangan:** Menguji pemahaman bioinformatika statistik kalian di balik metrik keanekaragaman hayati.
* **Jebakan Maut:** ❌ *"Nanopore sekarang sudah 100% akurat tanpa error."*
* **Format Jawaban Skakmat Hadi (PREP):**
  - **Point:** *"Tepat sekali, estimasi Chao1 mentah pada data Nanopore tanpa kurasi akan menghasilkan inflasi kekayaan taksa semu akibat artefak pembacaan."*
  - **Reason:** *"Untuk mengatasi hal ini, pipeline bioinformatika AquaSeq menerapkan tiga lapis penyaringan ketat sebelum indeks dihitung."*
  - **Evidence:** *"Pertama, penyaringan mutu Filtlong dengan ambang batas Q-score $\ge 10$ dan panjang bacaan 1.200–1.800 bp. Kedua, penerapan clustering berbasis kesamaan 97–99% untuk mereduksi varian error. Ketiga, normalisasi kedalaman pembacaan melalui proses rarefaction pada kedalaman seragam (misal 50.000 reads per sampel) sebelum menghitung Chao1, serta membuang singleton yang tidak terkonfirmasi pada kedua untai barcode."*
  - **Plan:** *"Dengan metode ini, Chao1 mencerminkan kekayaan taksa ekologis riil, bukan noise instrumen."*

---

### SERANGAN 6: Inkonsistensi Satuan (Persentase 16S vs Absolute qPCR)
* **Pertanyaan Juri:**  
  *"Di draf awal proposal kalian, ada grafik yang mencampuradukkan persentase Vibrio dengan label hasil qPCR mingguan. Data 16S itu bersifat komposisional (relatif), sedangkan qPCR menghasilkan Cycle threshold (Ct) atau jumlah kopi absolut. Bagaimana arsitektur kalian memastikan data komposisional tidak merusak seleksi marka qPCR?"*
* **Anatomi Serangan:** Menyerang kesalahan umum pemula yang menyamakan persentase sekuensing dengan angka absolut qPCR.
* **Jebakan Maut:** ❌ *"qPCR kan juga bisa ngeluarin persentase bakteri."*
* **Format Jawaban Skakmat Hadi (PREP):**
  - **Point:** *"Terima kasih atas koreksinya. Kami telah memisahkan secara tegas antara data komposisional relatif dari sekuensing dengan data kuantifikasi absolut dari qPCR."*
  - **Reason:** *"Data 16S bersifat proporsi relatif tertutup (sum = 100%). Jika satu taksa melonjak, taksa lain tampak turun secara artifisial. Untuk mengatasi bias ini, pipeline komputasi kami menerapkan transformasi Centered Log-Ratio (CLR) pada matriks kelimpahan taksa."*
  - **Evidence:** *"Transformasi CLR memproyeksikan data ke ruang log-ratio terhadap rata-rata geometrik sampel, sehingga seleksi marka qPCR menggunakan Stability Selection berbasis pada variansi dinamika riil, bukan distorsi persentase."*
  - **Plan:** *"Pada dashboard teknisi kolam, hasil qPCR mingguan ditampilkan dalam bentuk satuan delta perlipatan salinan (fold-change relative to baseline), bukan persentase semu."*

---

### SERANGAN 7: Masalah Inhibitor Air Payau & Volume Filtrasi eDNA
* **Pertanyaan Juri:**  
  *"Air tambak udang intensif sangat keruh, pekat suspensi alga, pakan sisa, dan senyawa humik yang merupakan inhibitor polimerase paling ganas untuk reaksi PCR. Membran filter 0.22 um sering mampet hanya dalam 50–100 mL air. Berapa volume filtrasi riil kalian dan bagaimana protokol mengatasi inhibitor air payau?"*
* **Anatomi Serangan:** Menguji apakah kalian pernah turun ke tepi kolam melihat air tambak yang seperti 'jus hijau pekat'.
* **Jebakan Maut:** ❌ *"Kami saring 10 liter air kolam pakai filter kopi."*
* **Format Jawaban Skakmat Hadi (PREP):**
  - **Point:** *"Kondisi air tambak intensif memang memiliki beban padatan tersuspensi dan asam humik yang sangat tinggi."*
  - **Reason:** *"Kami tidak memaksakan volume besar yang justru memicu penyumbatan membran dan konsentrasi inhibitor berlebih. Untuk air tambak dengan densitas plankton tinggi, volume filtrasi optimal berkisar antara 250 hingga 500 mL."*
  - **Evidence:** *"Kami menggunakan filter kapsul tertutup (Sterivex / syringe filter PES) dengan pre-filter bertingkat untuk menyaring debris kasar sebelum mencapai membran 0.22 μm. Pada tahap ekstraksi DNA, kami mensyaratkan kit ekstraksi yang dilengkapi kolom pembersih inhibitor polifenol/humik (misalnya Zymo OneStep PCR Inhibitor Removal atau kit DNeasy PowerWater)."*
  - **Plan:** *"Keberhasilan penghilangan inhibitor diverifikasi melalui Internal Amplification Control (IAC) pada setiap batch reaksi qPCR."*

---

### SERANGAN 8: Validasi Data Sintetis vs Bukti Lapangan (Kriteria E)
* **Pertanyaan Juri:**  
  *"Kalian membangun prototipe 3 hari ini di atas data publik NCBI dan skenario wabah sintetis. Menguji akurasi model pada data buatan sendiri itu sirkular dan bias. Bukti apa yang kalian punya hari ini bahwa petambak mau mempercayai peringatan WhatsApp kalian?"*
* **Anatomi Serangan:** Menyerang langsung Kriteria E (Validasi & Bukti) dari slide juri (Slide 19).
* **Jebakan Maut:** ❌ *"Model kami sudah 99% akurat dan petambak pasti percaya."*
* **Format Jawaban Skakmat Hadi (PREP):**
  - **Point:** *"Kami mengakui secara transparan dan berintegritas: prototipe hackathon saat ini berada di TRL 3, di mana skenario sintetis difokuskan untuk memvalidasi throughput pipa komputasi end-to-end, bukan pembuktian validasi akurasi klinis akhir."*
  - **Reason:** *"Sesuai dengan Tangga Bukti (Ladder of Evidence) pada materi bootcamp, kami tidak melompati tahapan hilirisasi. Asumsi risiko tertinggi kami saat ini adalah kemauan teknisi mengambil tindakan berdasarkan alert WhatsApp."*
  - **Evidence:** *"Untuk memvalidasi ini, kami telah menyusun panduan wawancara pada Appendix B proposal untuk mewawancarai 5–6 kepala tambak dan teknisi di koridor Banyuwangi–Situbondo guna menguji antarmuka, bahasa peringatan, dan batas toleransi false-alarm."*
  - **Plan:** *"Validasi ilmiah retrospektif akan dieksekusi pada Fase 2 (Nov 2026–Jan 2027) menggunakan data mikrobioma tambak terpublikasi dengan riwayat mortalitas terverifikasi, sebelum kami turun ke uji lapangan 2 farm di TRL 5."*

---

## Rangkuman Kata Kunci Emas untuk Diingat Hadi:
1. **Lu et al. (2023):** Bukti mikrobioma usus konvergen menyerupai air saat udang sakit.
2. **Wang et al. (2022):** Bukti plasmid pVA1 pembawa pirAB berpindah via konjugasi T4SS.
3. **Juanpere-Borràs et al. (2026):** Bukti efisiensi multiplexing 75 sampel per run Nanopore.
4. **Centered Log-Ratio (CLR):** Solusi matematika untuk bias data komposisional 16S.
5. **Elastic Net + Profile HMM:** Pilihan model yang bisa dijelaskan (explainable), bukan deep learning black box.
6. **Asset-Light Lab Partnership:** Solusi ketiadaan alat basah sendiri (bekerja sama dengan BBPBAP Situbondo).

# AquaSeq: Panduan Pembelajaran, Bisnis & Pitching Portal
**GenoHack 2026 Track 2: Genomics for Food Security and Biodiversity**  
*Tim: Disubmit Kok Tir Aman Ajah — Politeknik Negeri Jember*

---

> **Motto Produk:**  
> *"Sequencing to discover, qPCR to monitor, Bahasa Indonesia to act."*

> **Prinsip Posisi Produk:**  
> **Sistem Pelengkap Cerdas (The Missing Biological Layer), BUKAN Pengganti.**  
> AquaSeq tidak meminta petambak mengganti sensor IoT (seperti JALA) atau alat pemantau fisik kolam. Petambak tetap memakai sensor pH, suhu, dan oksigen (DO), lalu AquaSeq melengkapinya dengan mengolah **dua aliran data laboratorium** (sekuensing Nanopore berkala + qPCR mingguan) untuk mendeteksi ledakan mikroba patogen dan gen racun *pirAB* sebelum udang mati.

Repositori ini memuat seluruh materi pembelajaran komprehensif, arsitektur teknis, kalkulator bisnis interaktif, dan simulator presentasi (*pitch deck*) 3 menit untuk persiapan kompetisi **GenoHack 2026** di ITB Ganesha Bandung.

---

## 🚀 Cara Menggunakan Repositori Ini (Langsung Buka di Browser)
Cukup unduh / clone repositori ini, lalu **double-click** file [`index.html`](index.html) untuk membuka portal utama di Google Chrome, Microsoft Edge, atau browser lainnya.

---

## ⚡ Suite Dashboard Interaktif (Folder `dashboards/`)

| Dashboard | File | Deskripsi & Kegunaan |
| :--- | :--- | :--- |
| **⭐ Kitab Suci Versi Bahasa Bayi (Literally Semuanya!)** | [`dashboards/panduan-bahasa-bayi.html`](dashboards/panduan-bahasa-bayi.html) | Panduan visual interaktif lengkap: masalah Rp 100 juta petambak, biologi AHPND, celah JALA, 3 jurus AquaSeq, bedah modal Rp 2,2 juta, vs eFishery, plus kuis kilat! |
| **1. Pitch Deck 3 Menit** | [`dashboards/pitch-deck-interactive.html`](dashboards/pitch-deck-interactive.html) | Mode presentasi 10 slide interaktif dengan stopwatch latihan 180 detik, naskah santai Hadi, poin wajib juri, dan pantangan panggung. |
| **2. Simulator Bisnis & TEA** | [`dashboards/business-simulator.html`](dashboards/business-simulator.html) | Kalkulator Techno-Economic Analysis (TEA) dengan slider jumlah kolam, modal kerja, margin 51%, dan uji sensitivitas biaya reagen $\pm 20\%$. |
| **3. Pipeline AI & Genomik** | [`dashboards/genomics-pipeline.html`](dashboards/genomics-pipeline.html) | Visualisasi alur data dari air kolam (eDNA) → sekuensing Nanopore → QC Filtlong & CLR → pelacakan toksin pirAB → skor disbiosis → WhatsApp alert. |
| **4. Radar Kompetisi & Moat** | [`dashboards/competitive-moat.html`](dashboards/competitive-moat.html) | Radar multi-dimensi membandingkan AquaSeq vs JALA vs Kit PCR Lapangan vs Lab Sentral. Menjelaskan kenapa JALA adalah mitra API kita. |
| **5. Flashcard Killer Q&A** | [`dashboards/qa-simulator.html`](dashboards/qa-simulator.html) | Simulasi latihan menjawab 8 pertanyaan paling mematikan dari juri venture capital dan profesor biologi dengan kartu bolak-balik interaktif. |
| **6. Biodiversity Explorer** | [`dashboards/biodiversity-engine.html`](dashboards/biodiversity-engine.html) | Eksplorasi keanekaragaman hayati mikrobioma air tambak (Shannon Index $H'$, Chao1, Bray-Curtis) untuk penilaian mandat Track 2. |
| **7. Bahasa Bayi: Unit Economics & eFishery** | [`dashboards/unit-economics-efishery.html`](dashboards/unit-economics-efishery.html) | Pembedahan santai tanpa jargon: kenapa Rp 4,5 juta bisa tes 12 minggu, bedah modal Rp 2,2 juta, dan perbandingan langsung dengan raksasa eFishery. |
| **8. Hackday Challenge Masterclass** | [`dashboards/hackday-challenge-guide.html`](dashboards/hackday-challenge-guide.html) | Bedah materi Participant Kit D1–D6, tantangan industri Pathgen vs AquaSeq, 3 artefak wajib bawa ke Hackathon (Worksheet 20.1, 21.1, TEA), 4 lensa industri ALBITEC, dan rubrik Kriteria E. |
| **9. Worksheet Generator & Simulator 9 Skema Bayar** | [`dashboards/worksheet-generator.html`](dashboards/worksheet-generator.html) | Generator interaktif formulir resmi Worksheet 20.1, 21.1–21.2, dan 22. Lengkap dengan bukti validasi Pak Gatot (Situbondo), simulasi 9 skema pembayaran, dan tombol cetak laporan resmi! |

---

## 📚 Panduan Dokumen Mendalam (Folder `docs/`)
Bagi yang ingin membaca secara mendalam dalam format teks Markdown:

1. **[`01_RINGKASAN_EKSEKUTIF_AQUASEQ.md`](docs/01_RINGKASAN_EKSEKUTIF_AQUASEQ.md)**: Gambaran besar latar belakang masalah, urgensi ketahanan pangan udang nasional, dan inovasi AquaSeq.
2. **[`02_KAMUS_LENGKAP_ZERO_JARGON.md`](docs/02_KAMUS_LENGKAP_ZERO_JARGON.md)**: Kamus istilah lab (eDNA, 16S, pirAB, Nanopore, qPCR, Shannon) yang diterjemahkan ke analogi bahasa tongkrongan.
3. **[`03_BUSINESS_PLAN_DAN_TEA.md`](docs/03_BUSINESS_PLAN_DAN_TEA.md)**: Rencana bisnis venture, segmentasi pengguna vs pembayar, rincian COGS Rp 2,2 juta, pasar beachhead 1.200 kolam, dan Go-To-Market.
4. **[`04_PANDUAN_PITCHING_DAN_SCRIPT.md`](docs/04_PANDUAN_PITCHING_DAN_SCRIPT.md)**: Naskah lengkap presentasi 180 detik (detik demi detik), aturan panggung, dan tips percaya diri.
5. **[`05_KILLER_QA_DEFENSE_JURI.md`](docs/05_KILLER_QA_DEFENSE_JURI.md)**: Kumpulan 8 pertanyaan tersulit juri beserta contekan jawaban skakmat dan referensi jurnal resminya.
6. **[`06_ARSITEKTUR_TEKNIK_DAN_AI.md`](docs/06_ARSITEKTUR_TEKNIK_DAN_AI.md)**: Arsitektur software (FastAPI, Next.js, PostgreSQL), alasan menggunakan model Elastic Net dan transformasi CLR, serta guardrail LLM.
7. **[`07_AUDIT_DATA_DAN_SITASI_RESMI.md`](docs/07_AUDIT_DATA_DAN_SITASI_RESMI.md)**: Audit validitas 100% data, rujukan DOI jurnal peer-reviewed, kalkulasi riil modal tambak Jatim, dan batasan ilmiah anti-blunder.
8. **[`08_BEDAH_LENGKAP_WABAH_AHPND.md`](docs/08_BEDAH_LENGKAP_WABAH_AHPND.md)**: Bedah biologi penyakit AHPND/EMS, plasmid pVA1, gen racun pirAB, mekanisme kerusakan organ hepatopankreas, dan tindakan intervensi petambak.
9. **[`09_KAMUS_HACKER_BIOLOGI_UNTUK_ANAK_IT.md`](docs/09_KAMUS_HACKER_BIOLOGI_UNTUK_ANAK_IT.md)**: Kamus translasi istilah biologi saintifik ke analogi komputer (Wireshark, Regex, MAC address, Entropy, Knapsack) khusus buat mahasiswa IT.
10. **[`10_PREDIKSI_PERTANYAAN_PAKAR_BIOLOGI.md`](docs/10_PREDIKSI_PERTANYAAN_PAKAR_BIOLOGI.md)**: 8 Prediksi pertanyaan terganas pakar biologi/dosen mikrobiologi molekuler Track 2 beserta anatomi serangan, jebakan maut, dan format jawaban skakmat (metode PREP).
11. **[`11_KURASI_DATASET_PUBLIK_DAN_ALUR_UJI.md`](docs/11_KURASI_DATASET_PUBLIK_DAN_ALUR_UJI.md)**: Kurasi dataset publik terverifikasi (NCBI BioProject PRJNA1087723 & PRJNA947186) dan alur pemrosesan data FastQ Nanopore + Ct qPCR di prototipe.
12. **[`12_PANDUAN_TOTAL_BAHASA_BAYI.md`](docs/12_PANDUAN_TOTAL_BAHASA_BAYI.md)**: Kitab suci AquaSeq versi bahasa bayi (literally semuanya tanpa istilah biologi rumit).
13. **[`13_ANALISIS_PARTICIPANT_KIT_DAN_HACKDAY_CHALLENGE.md`](docs/13_ANALISIS_PARTICIPANT_KIT_DAN_HACKDAY_CHALLENGE.md)**: Analisis komprehensif seluruh dokumen Participant Kit, materi Zoom Bootcamp Day 1–6, pembedahan Hackday Challenge, 3 artefak wajib Jumat 23 Okt, dan strategi Kriteria D, E, G.
14. **[`14_DESAIN_LENGKAP_MVBP_AQUASEQ_STEP_22_24.md`](docs/14_DESAIN_LENGKAP_MVBP_AQUASEQ_STEP_22_24.md)**: Desain resmi MVBP (Minimum Viable Business Product) mengacu pada Disciplined Entrepreneurship Step 22–24 (Shelly Natalia MIT Sloan), 3 ujian kelayakan (Value, Pay, Feedback), strategi Concierge MVP, corong adopsi 7 tahap, dan roadmap produk V1–V3.
15. **[`15_VALIDASI_LAPANGAN_WAWANCARA_PAK_GATOT_SITUBONDO.md`](docs/15_VALIDASI_LAPANGAN_WAWANCARA_PAK_GATOT_SITUBONDO.md)**: Transkrip & analisis 18 poin wawancara praktisi tambak super-intensif Situbondo (Pak Gatot) yang mengunci Skor 4 pada Kriteria E.
16. **[`16_SKEMA_PEMBAYARAN_DAN_PIVOT_LAB_QPCR_VS_NANOPORE.md`](docs/16_SKEMA_PEMBAYARAN_DAN_PIVOT_LAB_QPCR_VS_NANOPORE.md)**: 9 Skema pembayaran fleksibel (bayar per tahap, paket per tambak dasar+kolam, potong panen), pivot lab qPCR-First vs Nanopore on-demand, dan triangulasi data sekunder pasar.

---

## 🧬 Dataset Publik Terverifikasi (Bahan Uji Prototipe Hackathon)
Untuk memastikan validitas ilmiah 100% dan bebas fabrikasi, prototipe komputasi AquaSeq diuji pada dataset publik resmi dunia:
* **NCBI BioProject PRJNA1087723** (*Rajonhson et al., 2024, Microbiology Spectrum*): Sekuensing Oxford Nanopore 16S full-length & Illumina pada **air tambak (*pond water*)** dan usus udang vaname.
* **NCBI BioProject PRJNA1445501** (*Khanh et al., 2024*): Runtut waktu 16S mikrobioma air tambak selama 10 minggu masa pemeliharaan (DOC).
* **NCBI BioProject PRJNA947186** (*Heliyon / Cell Press, 2024*): Profil komparatif mikrobioma udang sehat vs terinfeksi AHPND.
* **NCBI GenBank KM067908.1**: Sekuens referensi plasmid pVA1 pembawa gen racun *pirA* dan *pirB*.

---

## 💡 Ringkasan Finansial & Bisnis (Pegang Ini Saat Pitching!)
* **Aset Terancam:** Petambak intensif keluar modal **Rp 100.000.000 / kolam / siklus**. Serangan AHPND/Vibriosis mematikan udang 100% dalam DOC 10–35.
* **Harga Paket AquaSeq:** **Rp 4.500.000 / kolam / siklus** (3x Nanopore + 12x qPCR mingguan + Alert WhatsApp).
* **Beban Pokok (COGS Lab):** **Rp 2.200.000** (efisiensi multiplex 75 sampel per run).
* **Gross Profit Margin:** **51%** (Rp 2.300.000 per kolam).
* **Nilai Tambah Petambak:** **ROI 22x Lipat** dari satu siklus panen yang diselamatkan.
* **Pasar Awal (Beachhead):** 1.200 petak kolam tambak intensif di kawasan pesisir Banyuwangi–Situbondo, Jawa Timur.

---

## 👥 Tim Pengembang (Politeknik Negeri Jember)
* **Aji Seto Arifianto, S.ST., M.T.** — Team Leader & Academic Supervisor
* **Aditya Fadni Athaullah** — AI & Bioinformatics Lead
* **Muchamad Lucky Ramadhan** — Business & Research Lead
* **Krisna Panca Dewa** — Frontend & UI/UX Engineer
* **Hadi Akram Ramadhan** — Backend Engineer
* **Mohammad Yassir Thoriq Fathirurrizqy** — Data & Infrastructure Engineer
* *Dewan Penasihat (Advisory Board):* Praktisi Patologi Akuakultur & Mitra Balai Perikanan Budidaya Air Payau (BBPBAP) Situbondo.

# AquaSeq: Panduan Pembelajaran, Bisnis & Pitching Portal
**GenoHack 2026 Track 2: Genomics for Food Security and Biodiversity**  
*Tim: Disubmit Kok Tir Aman Ajah — Politeknik Negeri Jember*

---

> **Motto Produk:**  
> *"Sequencing to discover, qPCR to monitor, Bahasa Indonesia to act."*

Repositori ini memuat seluruh materi pembelajaran komprehensif, arsitektur teknis, kalkulator bisnis interaktif, dan simulator presentasi (*pitch deck*) 3 menit untuk persiapan kompetisi **GenoHack 2026** di ITB Ganesha Bandung.

---

## 🚀 Cara Menggunakan Repositori Ini (Langsung Buka di Browser)
Cukup unduh / clone repositori ini, lalu **double-click** file [`index.html`](index.html) untuk membuka portal utama di Google Chrome, Microsoft Edge, atau browser lainnya.

---

## ⚡ Suite Dashboard Interaktif (Folder `dashboards/`)

| Dashboard | File | Deskripsi & Kegunaan |
| :--- | :--- | :--- |
| **1. Pitch Deck 3 Menit** | [`dashboards/pitch-deck-interactive.html`](dashboards/pitch-deck-interactive.html) | Mode presentasi 10 slide interaktif dengan stopwatch latihan 180 detik, naskah santai Hadi, poin wajib juri, dan pantangan panggung. |
| **2. Simulator Bisnis & TEA** | [`dashboards/business-simulator.html`](dashboards/business-simulator.html) | Kalkulator Techno-Economic Analysis (TEA) dengan slider jumlah kolam, modal kerja, margin 51%, dan uji sensitivitas biaya reagen $\pm 20\%$. |
| **3. Pipeline AI & Genomik** | [`dashboards/genomics-pipeline.html`](dashboards/genomics-pipeline.html) | Visualisasi alur data dari air kolam (eDNA) → sekuensing Nanopore → QC Filtlong & CLR → pelacakan toksin pirAB → skor disbiosis → WhatsApp alert. |
| **4. Radar Kompetisi & Moat** | [`dashboards/competitive-moat.html`](dashboards/competitive-moat.html) | Radar multi-dimensi membandingkan AquaSeq vs JALA vs Kit PCR Lapangan vs Lab Sentral. Menjelaskan kenapa JALA adalah mitra API kita. |
| **5. Flashcard Killer Q&A** | [`dashboards/qa-simulator.html`](dashboards/qa-simulator.html) | Simulasi latihan menjawab 8 pertanyaan paling mematikan dari juri venture capital dan profesor biologi dengan kartu bolak-balik interaktif. |
| **6. Biodiversity Explorer** | [`dashboards/biodiversity-engine.html`](dashboards/biodiversity-engine.html) | Eksplorasi keanekaragaman hayati mikrobioma air tambak (Shannon Index $H'$, Chao1, Bray-Curtis) untuk penilaian mandat Track 2. |

---

## 📚 Panduan Dokumen Mendalam (Folder `docs/`)
Bagi yang ingin membaca secara mendalam dalam format teks Markdown:

1. **[`01_RINGKASAN_EKSEKUTIF_AQUASEQ.md`](docs/01_RINGKASAN_EKSEKUTIF_AQUASEQ.md)**: Gambaran besar latar belakang masalah, urgensi ketahanan pangan udang nasional, dan inovasi AquaSeq.
2. **[`02_KAMUS_LENGKAP_ZERO_JARGON.md`](docs/02_KAMUS_LENGKAP_ZERO_JARGON.md)**: Kamus istilah lab (eDNA, 16S, pirAB, Nanopore, qPCR, Shannon) yang diterjemahkan ke analogi bahasa tongkrongan.
3. **[`03_BUSINESS_PLAN_DAN_TEA.md`](docs/03_BUSINESS_PLAN_DAN_TEA.md)**: Rencana bisnis venture, segmentasi pengguna vs pembayar, rincian COGS Rp 2,2 juta, pasar beachhead 1.200 kolam, dan Go-To-Market.
4. **[`04_PANDUAN_PITCHING_DAN_SCRIPT.md`](docs/04_PANDUAN_PITCHING_DAN_SCRIPT.md)**: Naskah lengkap presentasi 180 detik (detik demi detik), aturan panggung, dan tips percaya diri.
5. **[`05_KILLER_QA_DEFENSE_JURI.md`](docs/05_KILLER_QA_DEFENSE_JURI.md)**: Kumpulan 8 pertanyaan tersulit juri beserta contekan jawaban skakmat dan referensi jurnal resminya.
6. **[`06_ARSITEKTUR_TEKNIK_DAN_AI.md`](docs/06_ARSITEKTUR_TEKNIK_DAN_AI.md)**: Arsitektur software (FastAPI, Next.js, PostgreSQL), alasan menggunakan model Elastic Net dan transformasi CLR, serta guardrail LLM.

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

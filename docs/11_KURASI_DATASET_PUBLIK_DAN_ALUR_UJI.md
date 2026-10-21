# Kurasi Dataset Publik & Alur Pengujian Prototipe AquaSeq
**Dokumentasi Dataset Resmi (NCBI BioProject & SRA) untuk Pipeline Hackathon GenoHack 2026**

---

## 1. Sumber Data Nyata: Tidak Mengarang, 100% Data Publik Terbuka
Untuk membangun prototipe selama 3 hari hackathon (23–25 Oktober) tanpa melanggar etika dan aturan GenoHack, tim menggunakan dataset publik yang telah dipublikasikan di repositori genomik dunia (**NCBI Sequence Read Archive / BioProject**).

Data mentah ini merekam kondisi nyata air kolam tambak (*pond water*) dan usus udang vaname (*Litopenaeus vannamei*), mencakup sekuensing **Oxford Nanopore (long-read)** dan **qPCR / amplikon**.

---

## 2. Tabel Master Dataset Publik yang Digunakan

| No | BioProject ID / SRA Accession | Sumber Literatur Resmi | Tipe Data & Platform | Kompartemen Sampel | Kegunaan Spesifik di AquaSeq Engine |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1** | **PRJNA1087723** | Rajonhson et al. (2024), *Microbiology Spectrum* | **Oxford Nanopore MinION** (Full-Length 16S V1–V9) & Illumina V3–V4 | **Air Tambak (Pond Water)**, Usus Udang, Sedimen | **DATASET INTI NANOPORE:** Menguji pipeline pembacaan Nanopore langsung pada sampel air tambak vaname. Memvalidasi kestabilan indeks keragaman (Shannon/Chao1) antara bacaan panjang vs pendek. |
| **2** | **PRJNA1445501** | Khanh et al. (2024), *NCBI SRA / GitHub Repository* | Illumina 16S rRNA Amplikon Time-Series | **Air Kolam Tambak**, Usus, Sedimen (10 Minggu Budidaya) | **BASELINE DINAMIKA AIR (DOC):** Memetakan pergeseran mikrobioma air kolam normal dari minggu ke minggu selama siklus budidaya 10 minggu untuk baseline kolam sehat. |
| **3** | **PRJNA947186** | Heliyon (2024) / Cell Press | Illumina V3–V4 (Primer 341F/806R) | Lambung & Usus Udang (Sehat vs **Terinfeksi AHPND**) | **LABEL STATUS PENYAKIT AHPND:** Menyediakan 53 profil tanda mikrobioma pembeda antara udang sehat vs udang terinfeksi AHPND untuk melatih dan menguji model regresi Elastic Net. |
| **4** | **PRJNA645513** (SRR12199297, SRR12199298) | Food Science & Nutrition (2021) | 16S rRNA Metabarcoding Time-Course (0, 6, 12 hpi) | Udang Uji Tantang *Vibrio parahaemolyticus* AHPND | **UJI RESPON AWAL DISBIOSIS:** Data runtut waktu infeksi AHPND jam ke-6 dan jam ke-12 untuk membuktikan sinyal pergeseran mikrobioma mendahului mortalitas. |
| **5** | **GenBank KM067908.1** | Wang et al. / Han et al. (NCBI GenBank) | Sekuens Nukleotida Lengkap (Plasmid DNA) | Plasmid pVA1 *Vibrio parahaemolyticus* strain 3HP | **DATABASE REFERENSI TOKSIN pirAB:** Sekuens rujukan gen *pirA* dan *pirB* untuk membangun Profile HMM dan acuan pencocokan gen virulensi di pipeline. |

---

## 3. Alur Pengolahan Data di Sistem AquaSeq (Wet-to-Dry)

Sistem AquaSeq bertindak sebagai **software intelligence layer** yang memproses dua aliran data laboratorium mitra:

```
[ ALUR LABORATORIUM MITRA ]                [ SISTEM ANALITIK AQUASEQ ]
-----------------------------------------------------------------------------------------
1. eDNA Air (Tiap 2-4 Minggu)
   └─> Sekuensing Nanopore 16S  ─────> (A) FASTQ Mentah Masuk via API/Upload
                                             │
                                             ▼
                                       (B) Filtlong QC (Q-score ≥ 10, length 1.2-1.8 kb)
                                             │
                                             ▼
                                       (C) Profiling Taksonomi (Silva 138 Classifier)
                                             │
                                             ▼
                                       (D) Normalisasi CLR (Hapus Bias Komposisional)
                                             │
                                             ▼
                                       (E) Hitung Shannon Index & Bray-Curtis vs Baseline
                                             │
                                             ▼
                                       (F) Profile HMM Scan (Pencarian Gen Toksin pirAB)
                                             │
                                             ▼
                                       (G) Scoring Risiko Disbiosis (Elastic Net Model)
                                             │
                                             ▼
                                       (H) Stability Selection (Pilih 3–5 Marka Terbaik)
                                             │
                                             ├─────────────────────────────────────────┐
                                             ▼                                         ▼
2. Monitoring Mingguan                 [ Dashboard Teknis Kolam ]            [ Rekomendasi qPCR ]
   └─> qPCR Kit (3–5 Marka) ─────────> (I) Input Nilai Ct / Salinan          (Kirim ke Lab Mitra)
                                             │
                                             ▼
                                       (J) Evaluasi Delta Kuantitatif
                                             │
                                             ▼
                                  [ ALERTA WHATSAPP PETAMBAK ]
                                  "Kolam B-02: Waspada Vibrio.
                                   Kurangi pakan 20% & sipon."
```

---

## 4. Format Payload Data untuk Uji Hackathon (Mock & Real Ingestion)

Pada prototipe hackathon, data dari BioProject di atas diekstraksi ke format file JSON terstruktur yang menjadi input backend FastAPI:

```json
{
  "sample_metadata": {
    "sample_id": "LOT-STB-20261020-B02",
    "bioproject_ref": "PRJNA1087723",
    "compartment": "pond_water",
    "farm_location": "Situbondo, Jawa Timur",
    "day_of_culture": 28,
    "temperature_c": 29.5,
    "salinity_ppt": 22.0
  },
  "nanopore_metrics": {
    "raw_reads": 182400,
    "qc_passed_reads": 168910,
    "shannon_index": 2.14,
    "chao1_richness": 42.0,
    "bray_curtis_shift": 0.38,
    "pirab_virulence_detected": true,
    "pirab_reads_count": 18
  },
  "qpcr_weekly_inputs": [
    { "marker": "V. parahaemolyticus gyrB", "ct_value": 24.2, "fold_change": 3.8 },
    { "marker": "pirA/pirB toxin plasmid", "ct_value": 28.5, "fold_change": 4.2 },
    { "marker": "Rhodobacteraceae 16S", "ct_value": 31.0, "fold_change": 0.7 }
  ],
  "engine_outputs": {
    "dysbiosis_risk_score": 0.58,
    "risk_band": "WASPADA (BAND II)",
    "recommended_actions": [
      "Kurangi pakan 15-20% untuk membatasi akumulasi nutrien organik.",
      "Lakukan penyiponan endapan lumpur dasar kolam sore ini.",
      "Tingkatkan durasi operasional kincir aerasi pada malam hari."
    ]
  }
}
```

---

## 5. Cara Menjelaskan Penggunaan Data ke Juri (Anti-Skakmat)

> *"Pak Juri, prototipe komputasi kami di hackathon ini dibangun dan diuji menggunakan dataset publik terverifikasi dari NCBI BioProject: secara khusus **PRJNA1087723** untuk data sekuensing Nanopore 16S air tambak vaname, dan **PRJNA947186** untuk profil pembeda AHPND.*  
> *Sistem kami menerima input berkas FastQ Nanopore berkala dan nilai kuantifikasi qPCR mingguan, menormalkannya dengan transformasi CLR, menghitung Shannon Index, dan menerjemahkan angka biologis tersebut menjadi instruksi praktis yang melengkapi dashboard sensor IoT yang sudah dimiliki petambak."*

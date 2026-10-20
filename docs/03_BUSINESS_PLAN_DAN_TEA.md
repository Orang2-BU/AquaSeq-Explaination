# Techno-Economic Analysis (TEA) & Business Plan: AquaSeq
**Kriteria D (Kelayakan Bisnis 15%) & Kriteria G (Jalur ke Pasar dan Skala 15%)**

---

## 1. Executive Summary & Customer Value Proposition
AquaSeq adalah platform early-warning berbasis biologi molekuler untuk tambak udang intensif dengan model bisnis **B2B SaaS + Diagnostic Service Subscription**.

### The Unfair Value Proposition
* **Customer Pain:** Petambak intensif menginvestasikan Rp 80.000.000 – Rp 120.000.000 per kolam per siklus (100 hari). Kematian massal akibat AHPND/Vibriosis memusnahkan seluruh modal dalam hitungan 48 jam.
* **AquaSeq Offer:** Asuransi deteksi dini berbasis genomik seharga **Rp 4.500.000 per kolam per siklus**.
* **Petambak ROI:** 
  $$\text{Payback Ratio} = \frac{\text{Aset Terselamatkan}}{\text{Biaya AquaSeq}} = \frac{\text{Rp 100.000.000}}{\text{Rp 4.500.000}} = \mathbf{22{,}2\times}$$

---

## 2. Customer Segmentation: Pengguna vs Pembayar
Mengacu pada Slide 20 Bootcamp GenoHack (*"Siapa pengguna, siapa yang benar-benar membayar?"*):

| Segmen | Peran | Alasan Membeli / Pakai |
| :--- | :--- | :--- |
| **Kepala Kolam & Teknisi Lapangan** | **User (Pengguna)** | Butuh panduan praktis yang bisa dibaca satu jempol di tepi kolam tanpa istilah DNA bahasa Inggris. Mengurangi beban kerja dan risiko kena semprot pemilik tambak saat udang mati. |
| **Pond Owner (Pemilik Tambak Intensif)** | **Buyer (Pembeli)** | Melindungi modal kerja Rp 100 juta per kolam. Menjamin stabilitas panen dan kelayakan kredit bank. |
| **Feed Mill & Hatchery Integrator (CP Prima, Japfa, dll.)** | **Enterprise Buyer** | Menjamin pasokan benur dan pakan terserap optimal. Mengurangi gagal bayar petambak plasma binaan. |

---

## 3. Techno-Economic Analysis (TEA) & Unit Economics
Mengacu pada Slide 14–15 Bootcamp GenoHack:
$$\text{Biaya Per Unit} = \frac{\text{CAPEX Tahunan} + \text{OPEX Tahunan}}{\text{Output Sampel Tahunan}}$$

### Rincian Beban Pokok Pendapatan (COGS) Per Kolam Per Siklus (100 Hari)
AquaSeq mengadopsi model *asset-light* (tanpa membeli mesin sekuensing sendiri di awal; memanfaatkan kapasitas berlebih laboratorium mitra terakreditasi):

| Komponen Biaya | Frekuensi / Spesifikasi | Biaya per Unit | Total per Kolam/Siklus |
| :--- | :--- | :--- | :--- |
| **Sekuensing Nanopore 16S + Marka** | 3 kali uji (DOC 1 tebar, DOC 30, DOC 60). Multiplexing 75 sampel per flowcell | Rp 300.000 / uji | Rp 900.000 |
| **Uji qPCR Mingguan (3–5 Marka)** | 12 minggu masa budidaya | Rp 75.000 / uji | Rp 900.000 |
| **Kit Pengambilan Sampel eDNA** | 15 membran filter sterilisasi, spuit, buffer lisis | Rp 15.000 / kit | Rp 225.000 |
| **Logistik Rantai Dingin Lokal** | Kurir berpendingin wilayah Banyuwangi–Situbondo–Jember | Rp 15.000 / pengiriman | Rp 175.000 |
| **Total COGS (HPP)** | | | **Rp 2.200.000** |

### Penetapan Harga & Margin Keuntungan
* **Harga Jual Paket Layanan:** **Rp 4.500.000 per kolam per siklus**.
* **Gross Profit per Kolam:** $\text{Rp 4.500.000} - \text{Rp 2.200.000} = \mathbf{\text{Rp 2.300.000}}$.
* **Gross Margin:** 
  $$\text{Gross Margin} = \frac{\text{Rp 2.300.000}}{\text{Rp 4.500.000}} \times 100\% = \mathbf{51{,}1\%}$$

---

## 4. Analisis Sensitivitas Tekno-Ekonomi (Tuntutan Slide 15)
Slide juri mensyaratkan: *"Uji sensitivitas: ubah tiap parameter $\pm 20\%$ dan lihat mana yang paling mengubah biaya per unit."*

| Skenario | Parameter yang Berubah | Dampak pada COGS | Margin Kotor Baru | Evaluasi Risiko |
| :--- | :--- | :--- | :--- | :--- |
| **Baseline** | Semua asumsi normal | Rp 2.200.000 | **51,1%** | Target operasi sehat |
| **Skenario A (+20% Biaya Reagen)** | Kurs USD naik, biaya flowcell & reagen naik 20% | Rp 2.560.000 | **43,1%** | Masih sangat menguntungkan (>40%) |
| **Skenario B (-20% Utilisasi Batch)** | Hanya terisi 60 sampel per flowcell (bukan 75) | Rp 2.425.000 | **46,1%** | Aman, lab partner menampung batch regional |
| **Skenario C (+20% Efisiensi Skala)** | Volume naik >200 kolam, diskon reagen grosir | Rp 1.840.000 | **59,1%** | Keuntungan melonjak seiring ekspansi |

*Kesimpulan Sensitivitas:* Parameter paling sensitif adalah **utilisasi sampel per batch (flowcell multiplexing)**. Kuncinya adalah mengumpulkan sampel secara terpusat di kawasan klaster tambak Banyuwangi–Situbondo.

---

## 5. Ukuran Pasar (Market Sizing: TAM, SAM, SOM)
* **TAM (Total Addressable Market):** 
  - Produksi udang budidaya Indonesia: $\sim 7,3$ juta ton dunia; Indonesia $\sim 1$ juta ton.
  - $\sim 70.000$ petak kolam tambak intensif di seluruh Indonesia.
  - Nilai Pasar: $70.000 \times \text{Rp 4,5 jt} \times 3 \text{ siklus/th} = \mathbf{\text{Rp 945 Miliar / tahun}}$.
* **SAM (Serviceable Available Market):** 
  - Wilayah pesisir Jawa Timur (Banyuwangi, Situbondo, Tuban, Probolinggo).
  - Sekitar 12.000 kolam intensif.
  - Nilai Pasar: $12.000 \times \text{Rp 4,5 jt} \times 3 = \mathbf{\text{Rp 162 Miliar / tahun}}$.
* **SOM (Serviceable Obtainable Market - Beachhead 2 Tahun Pertama):** 
  - 1.200 kolam intensif di koridor pesisir Banyuwangi–Situbondo (radius operasional lab Politeknik Negeri Jember / Balai Situbondo).
  - Target adopsi 10% (120 kolam pada Tahun ke-2).
  - Pendapatan Tahunan: $120 \times \text{Rp 4,5 jt} \times 3 = \mathbf{\text{Rp 1,62 Miliar / tahun}}$.

---

## 6. Strategi Go-To-Market (GTM) & Saluran Distribusi
1. **Fase 1: Direct Pilot B2B (Bulan 1–6)**
   - 2 Farm mitra di Banyuwangi (masing-masing 4–6 petak kolam).
   - Menghasilkan bukti tertulis (*Letter of Intent / LoI*) dan pembuktian akurasi lapangan (skor Kriteria E = 5).
2. **Fase 2: Integrator & Feed Mill Partnership (Bulan 7–18)**
   - Menggandeng perusahaan pakan udang besar. AquaSeq dijadikan paket *bundled premium* untuk pembeli pakan dalam volume tertentu.
3. **Fase 3: API Integration dengan Platform Manajemen Tambak (Bulan 19+)**
   - Menghubungkan AquaSeq Engine ke aplikasi **JALA** via REST API, menjadi add-on berbayar bagi puluhan ribu pengguna JALA yang butuh deteksi patogen biologis.

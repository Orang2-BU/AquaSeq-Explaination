# AquaSeq · Ringkasan Eksekutif & Peta Strategis
**GenoHack 2026 — Track 2: Genomics for Food Security and Biodiversity**
*Tim: Disubmit Kok Tir Aman Ajah — Politeknik Negeri Jember*

---

## 1. Fondasi Masalah: "Kenapa AquaSeq Harus Ada?"
Budidaya udang vaname (*Penaeus vannamei*) di Indonesia adalah penopang devisa ekspor perikanan nomor satu nasional. Namun, industri ini dihantui satu momok mematikan: **wabah penyakit mendadak**, khususnya:
1. **AHPND (Acute Hepatopancreatic Necrosis Disease) / EMS**: Menyebabkan kematian hingga 100% dalam 10–35 hari setelah tebar benur (DOC 10–35). Kerugian global mencapai lebih dari USD 7 miliar per tahun.
2. **IMNV (Infectious Myonecrosis Virus)**: Menghancurkan jaringan otot udang. Wabah Situbondo 2018 memunculkan varian baru dengan delesi 622 asam amino yang lolos dari tes biasa.
3. **Vibriosis & WSSV (White Spot Syndrome Virus)**: Menyebabkan kerugian tahunan hingga miliaran dolar.

### Mengapa Solusi Saat Ini Gagal?
* **Sensor IoT Fisika-Kimia (seperti JALA):** Hanya memantau pH, suhu, salinitas, dan oksigen terlarut (DO). Air kolam bisa tampak jernih dan bernilai normal di dashboard, sementara populasi bakteri patogen di dalamnya sudah berlipat ganda menuju tingkat mematikan.
* **Kit PCR Konvensional di Lapangan:** Bersifat reaktif dan sempit. Hanya mencari 1 atau 2 target yang dicurigai setelah udang tampak lesu. Padahal penyakit udang bersifat **polimikroba** (kombinasi beberapa mikroba) dan dinamis.
* **Hasil Tes Lab Lambat:** Petambak mengirim sampel ke lab luar dan menunggu 3–7 hari. Sementara AHPND bisa memusnahkan kolam dalam 48 jam.

---

## 2. Solusi: "Sequencing to Discover, qPCR to Monitor, Bahasa Indonesia to Act"
AquaSeq menghadirkan jembatan cerdas antara teknologi genomik tingkat tinggi dengan keputusan praktis di tepi kolam:

```
[ Air Kolam ] (eDNA filter berkala)
      │
      ▼
[ Nanopore Sequencing ] (Membaca komunitas bakteri 16S + gen virulensi pirAB)
      │
      ▼
[ AquaSeq Engine ] (Menghitung Indeks Keragaman Shannon + Skor Risiko Dysbiosis)
      │
      ├──> [ Pemilih Marka qPCR ] (Memilih 3-5 marka paling kritis untuk kolam itu)
      │          │
      │          ▼
      │    [ Monitoring Mingguan qPCR Murah ] (Tracking mingguan cepat & hemat)
      │
      ▼
[ Decision Layer ] (Dashboard Web Mobile & Notifikasi Otomatis WhatsApp)
      │
      ▼
[ Petambak Bertindak ] ("Kolam B-02 Waspada Vibrio: Kurangi pakan 20%, sipon dasar hari ini")
```

---

## 3. Kesesuaian Sempurna dengan Track 2: Food Security & Biodiversity
Lomba GenoHack Track 2 menuntut dua aspek utama:
1. **Food Security (Ketahanan Pangan):** Menyelamatkan pasokan udang nasional dari gagal panen massal, menjaga devisa ekspor, dan melindungi mata pencaharian petambak.
2. **Aquatic Biodiversity (Keanekaragaman Hayati Perairan):**
   - AquaSeq tidak sekadar membasmi bakteri, melainkan memantau kesehatan ekosistem perairan menggunakan metrik ekologi standar: **Shannon Diversity Index**, **Chao1 Richness**, dan **Bray-Curtis Beta Diversity**.
   - Mencegah penggunaan antibiotik membabi-buta yang selama ini merusak mikrobioma alami perairan pesisir Indonesia.

---

## 4. Logika Bisnis & Kelayakan Ekonomi (Venture Ready)
* **Pasar Awal (Beachhead):** 1.200 kolam intensif di segitiga emas akuakultur Jawa Timur (Banyuwangi – Situbondo – Jember).
* **Nilai Finansial:**
  - Modal kerja petambak per kolam intensif: **Rp 80 – 120 Juta per siklus**.
  - Harga Paket Layanan AquaSeq: **Rp 4.500.000 per kolam per siklus**.
  - Beban Pokok Pendapatan (COGS): **Rp 2.200.000 per kolam per siklus** (karena efisiensi multiplexing 75 sampel per run).
  - **Gross Margin:** **51%**.
  - **ROI bagi Petambak:** **22x Lipat** pengembalian modal dari 1 siklus panen yang berhasil diselamatkan dari gagal panen.

---

## 5. Posisi Kematangan Teknologi (TRL)
* **Saat Ini (Hackathon GenoHack): TRL 3** (Analytical pipeline working on public & synthetic datasets).
* **6 Bulan (Retrospective Validation): TRL 4** (Validasi pada data retrospektif dengan hasil klinis terkonfirmasi).
* **12 Bulan (Field Pilot): TRL 5** (Pilot lapangan di 2 tambak intensif Jawa Timur bekerja sama dengan Balai Perikanan Situbondo).

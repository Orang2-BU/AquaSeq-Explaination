# Bedah Lengkap Wabah AHPND (Acute Hepatopancreatic Necrosis Disease)
**Panduan Penguasaan Materi Biologi Penyakit untuk Hadi — GenoHack 2026**

---

## 1. Apa Itu AHPND Sebenarnya? (Singkatan & Sejarah)
* **Kepanjangan:** **A**cute **H**epatopancreatic **N**ecrosis **D**isease.
* **Nama Lama:** Dulu petambak menyebutnya **EMS (Early Mortality Syndrome)** karena udang mati massal di awal-awal tebar.
* **Kapan Menyerang?** Biasanya menyerang di **DOC 10 – 35** (Day of Culture: hari ke-10 sampai ke-35 setelah benur ditebar ke kolam).
* **Tingkat Kematian:** Hingga **100% kematian massal** dalam hitungan hari (*Sen et al., 2026, Vaccine*).

---

## 2. Siapa Pelaku Utamanya? (Bakteri + Senjata Beracun)
Penyakit ini **bukan disebabkan oleh virus**, melainkan oleh **bakteri**:

1. **Nama Bakterinya:** *Vibrio parahaemolyticus* (bakteri Gram-negatif berbentuk batang melengkung yang hidup alami di air payau dan laut).
2. **Kuncinya (JANGAN SALAH!):** 
   - **TIDAK SEMUA** *Vibrio parahaemolyticus* itu jahat! Jutaan *Vibrio* biasa hidup damai di kolam tanpa bikin udang mati.
   - *Vibrio* baru berubah jadi pembunuh mematikan **HANYA JIKA** dia membawa cincin DNA ekstra bernama **Plasmid pVA1**.
   - Di dalam plasmid pVA1 ini terdapat sepasang gen racun mematikan bernama **pirA dan pirB** (*Photorhabdus insect-related toxins*).

### Analogi Tongkrongan:
> *Vibrio biasa itu kayak pemuda yang lagi nongkrong di pos ronda. Gak berbahaya.*  
> *Tapi kalau ada satu orang bawa pistol rakitan (Plasmid pVA1 + gen racun pirAB), dia berubah jadi teroris mematikan.*  
> *Hebatnya lagi, riset Wang dkk. (2022) membuktikan bakteri pembawa plasmid ini bisa 'nularin senjata' ke bakteri lain lewat jembatan konjugasi (T4SS). Makanya wabahnya bisa meledak sangat cepat!*

---

## 3. Apa yang Terjadi di Tubuh Udang? (Kenapa Udang Bisa Mati?)
1. **Organ yang Diserang: Hepatopankreas (HP)**
   - Hepatopankreas adalah organ vital udang yang terletak di bagian kepala/dada.
   - Fungsinya gabungan antara lambung, hati, dan pankreas: buat mencerna makanan sekaligus menyimpan cadangan energi.
2. **Mekanisme Racun PirAB:**
   - Udang menelan air atau sedimen yang mengandung *Vibrio* beracun.
   - Bakteri memproduksi racun protein biner **PirA + PirB**.
   - Racun ini bertindak seperti peluru yang **menembus dan melubangi membran sel** tubulus hepatopankreas (*pore-forming toxin*).
   - Sel-sel hepatopankreas pecah, rontok (*sloughing*), dan jaringannya membusuk/mati (*nekrosis*).
3. **Ciri Fisik Udang yang Kena AHPND di Kolam:**
   - **Hepatopankreas mengecil dan pucat:** Organ di kepala yang tadinya cokelat/kehitaman berubah jadi putih pucat atau mengecil kisut.
   - **Usus kosong:** Udang berhenti makan (*anoreksia*), saluran usus tampak bening tanpa kotoran pakan.
   - **Cangkang lembek dan udang lemas:** Udang berenang tidak terarah di tepi kolam lalu tenggelam mati ke dasar.

---

## 4. Kenapa Solusi Lain Gagal Menghadapi AHPND?

| Metode Pemantauan Lain | Kenapa Gagal / Terlambat Menangani AHPND? |
| :--- | :--- |
| **Sensor IoT Air (JALA / pH / DO / Suhu)** | Bakteri *Vibrio* dan racun *pirAB* **tidak mengubah pH atau suhu air secara drastis**. Di layar aplikasi sensor, air terbaca hijau/normal, padahal di dalam air racun sudah diproduksi massal. |
| **Uji Cawan Agar TCBS Laboratorium** | Cawan TCBS hanya menumbuhkan koloni hijau/kuning *Vibrio*. Uji ini **tidak bisa membedakan** mana *Vibrio* biasa dan mana *Vibrio* pembawa gen racun *pirAB*. Hasilnya sering salah sangka (*false alarm*). |
| **Melihat Anco Pakan Manual** | Teknisi kolam baru sadar saat pakan di anco tidak habis dan udang mulai mati mengambang. Saat hepatopankreas sudah rusak dan membusuk, udang **sudah tidak bisa diobati lagi**. |

---

## 5. Bagaimana AquaSeq Menghentikan AHPND?

1. **Mendeteksi Sinyal Disbiosis Sebelum Kematian:**
   Sebelum wabah meledak, ekosistem mikrobioma air kolam mengalami guncangan (*Shannon Index turun, rasio bakteri baik drop*). AquaSeq menangkap sinyal pergeseran ekologis ini dari eDNA air.
2. **Melacak Keberadaan Gen Toksin pirAB:**
   Engine bioinformatika AquaSeq secara spesifik melacak urutan gen *pirA* dan *pirB* menggunakan Profile HMM, bukan sekadar menghitung bakteri *Vibrio*.
3. **Peringatan & Tindakan Cepat di WhatsApp:**
   Ketika terdeteksi sinyal waspada di DOC 20 (sebelum kematian massal terjadi), teknisi langsung diinstruksikan:
   - *Kurangi pakan 20%:* Mengurangi pakan memotong suplai nutrisi organik yang disukai bakteri *Vibrio*.
   - *Sipon dasar kolam:* Mengeluarkan bangkai mikroba dan kotoran amonia di titik mati kolam.
   - *Aplikasikan probiotik kompetitif:* Menambahkan bakteri penyeimbang untuk merebut kembali relung ekosistem.

---

## 6. Contekan Jawaban 10 Detik di Panggung

> *"Pak Juri, AHPND atau EMS adalah pembunuh nomor satu udang vaname di umur 10 sampai 35 hari tebar dengan kematian hingga 100%.*  
> *Penyebabnya bukan sekadar bakteri Vibrio, melainkan gen racun pirAB pada plasmid pVA1 yang melubangi organ pencernaan hepatopankreas udang hingga membusuk.*  
> *Sensor pH tidak bisa melihat racun ini, dan melihat bangkai di kolam sudah terlambat. AquaSeq mendeteksi gen racun pirAB dan pergeseran mikrobioma air melalui eDNA sebelum udang mulai mati."*

## Optimizing Market Demand: Architectural Typology and Revenue Performance in Bangkok’s Airbnb

*Executive Summary*

Analisis ini mengevaluasi performa 12.574 properti aktif di Bangkok untuk memetakan variabel arsitektural dan lokasi yang paling berpengaruh terhadap pendapatan. Temuan kunci menunjukkan bahwa aksesibilitas transportasi (jalur BTS/MRT) dan fungsionalitas interior (Dapur & Ruang Kerja) memberikan premi harga yang jauh lebih tinggi dibandingkan fasilitas gedung standar seperti kolam renang atau gym.
​Secara arsitektural, penelitian ini menemukan adanya "Privacy Premium" yang signifikan; unit dengan rasio maksimal 3 tamu per 1 kamar mandi mencatatkan efisiensi pendapatan tertinggi. Investor disarankan untuk beralih dari strategi "maksimalisasi kapasitas tempat tidur" menuju "optimalisasi rasio privasi dan fungsionalitas unit" guna mengamankan yield yang kompetitif di pasar menengah Bangkok (rentang harga ฿122 - ฿3.752).

Proyek ini menganalisis listing Airbnb di Bangkok untuk mengungkap strategi investasi berbasis data. Dengan menggabungkan intelijen lokasi, atribut properti, dan estimasi pendapatan, proyek ini memberikan wawasan yang dapat ditindaklanjuti bagi investor real estat yang mencari aset berkinerja tinggi.

## Tujuan
Mengidentifikasi tipe properti, lokasi, dan fitur arsitektural yang paling menguntungkan untuk investasi sewa jangka pendek di Bangkok.

## Dataset
* **Sumber:** Inside Airbnb (Bangkok)
* 28.806 listing awal dengan 79 fitur.
* Dibersihkan menjadi **12.574** listing aktif melalui filter ulasan terbaru dan validasi harga.

## Metodologi
1. **Pembersihan Data:** Mem-parsing harga dan fasilitas; menetapkan batas harga minimal **฿100** untuk validitas operasional; menghapus outlier harga menggunakan metode IQR (**Rentang Akhir: ฿122 - ฿3.752**).
2. **Rekayasa Fitur:** Membuat variabel biner untuk fasilitas kunci (AC, Dapur, Pool, Gym, Workspace) dan menghitung rasio tamu-per-kamar mandi.
3. **Estimasi Pendapatan:** Menggunakan "model kewajaran" (tingkat ulasan 50%, rata-rata menginap 3 malam) untuk estimasi bulanan.
4. **Analisis Eksploratif:** Peta panas lokasi, box plot tipe properti, dan analisis korelasi privasi (kamar mandi).

## Temuan Utama
* **Lokasi:** Konsentrasi pendapatan tinggi mengikuti jalur BTS/MRT, melintasi batas administratif distrik.
* **Tipe Properti:** Seluruh rumah/townhouse menghasilkan pendapatan tertinggi dibandingkan kamar privat.
* **Nilai Arsitektural:** Dapur dan ruang kerja memberikan premi harga tertinggi; sementara AC (86%) telah menjadi fasilitas standar pasar.
* **Keseimbangan Privasi:** Penambahan kamar mandi kedua adalah *price driver* krusial. Pendapatan menurun signifikan saat rasio melebihi 3 tamu per 1 kamar mandi.

## Rekomendasi
* **Target Investasi:** Prioritaskan unit dengan dapur lengkap dan rasio minimal **1 kamar mandi untuk setiap 3 tamu**.
* **Strategi Aset:** Untuk kapasitas >4 tamu, pastikan tersedia minimal 2 kamar mandi guna menjaga harga sewa premium.
* **Lokasi:** Fokus pada area dalam radius jalan kaki dari stasiun transportasi utama.

## Tools & Libraries
* Python (pandas, numpy, matplotlib, seaborn)
* Folium (Geospatial mapping)
* Jupyter Notebook / Quarto


> **[📊 Lihat Laporan Interaktif Lengkap (HTML)](https://s-hidayat.github.io/Bangkok-Airbnb-analysis/)**


## Author
**Samsur Hidayat** – Real Estate Data Analyst

---

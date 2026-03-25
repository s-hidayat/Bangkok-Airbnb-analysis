# Optimizing Market Demand: Architectural Typology and Revenue Performance in Bangkok’s Airbnb

Proyek ini menganalisis listing Airbnb di Bangkok untuk mengungkap strategi investasi berbasis data. Dengan menggabungkan intelijen lokasi, atribut properti, dan estimasi pendapatan, proyek ini memberikan wawasan yang dapat ditindaklanjuti bagi investor real estat yang mencari aset berkinerja tinggi.

## Tujuan
Mengidentifikasi tipe properti, lokasi, dan fitur arsitektural yang paling menguntungkan untuk investasi sewa jangka pendek di Bangkok.

## Dataset
* **Sumber:** Inside Airbnb (Bangkok)
* 28.806 listing dengan 79 fitur
* Dibersihkan dan disaring menjadi 12.574 listing aktif dengan ulasan terbaru

## Metodologi
1.  **Pembersihan Data:** Mem-parsing harga, kamar mandi, dan fasilitas; menangani nilai kosong; menghapus pencilan (IQR).
2.  **Rekayasa Fitur:** Membuat indikator biner untuk fasilitas kunci dan menghitung rasio tamu-per-kamar mandi.
3.  **Estimasi Pendapatan:** Menggunakan "model kewajaran" (tingkat ulasan 50%, rata-rata menginap 3 malam) untuk memperkirakan pendapatan bulanan.
4.  **Analisis Eksploratif:**
    * Titik panas lokasi melalui peta panas.
    * Kinerja tipe properti (box plot).
    * Dampak fasilitas terhadap pendapatan.
    * **Analisis privasi: Hubungan antara jumlah kamar mandi, rasio tamu, dan efisiensi pendapatan.**

## Temuan Utama
* **Lokasi:** Konsentrasi pendapatan tinggi mengikuti jalur BTS/MRT, bukan batas administratif distrik.
* **Tipe Properti:** Seluruh rumah/townhouse menghasilkan pendapatan tertinggi; kamar privat berkinerja rendah.
* **Nilai Arsitektural:** Dapur (+37%) dan ruang kerja (+26%) memberikan premi harga tertinggi.
* **Efisiensi Ruang:** Pendapatan per tamu optimal pada kapasitas 5 dan 9 tamu.
* **Keseimbangan Privasi:** Penambahan kamar mandi ke-2 adalah *price driver* krusial untuk segmen grup. Pendapatan menurun drastis saat rasio melebihi 3 tamu per 1 kamar mandi.

## Rekomendasi
* **Fokus Fasilitas:** Prioritaskan unit dengan dapur lengkap dan ruang kerja khusus.
* **Strategi Arsitektural:** Targetkan properti dengan **rasio minimal 1 kamar mandi untuk setiap 3 tamu**.
* **Investasi Aset:** Untuk target pasar keluarga/grup (kapasitas >4), prioritaskan unit dengan minimal 2 kamar mandi guna menjaga daya tawar harga premium.
* **Lokasi:** Fokus pada area dalam radius jalan kaki dari stasiun transportasi utama.

## Tools & Libraries
* Python (pandas, numpy, matplotlib, seaborn)
* Folium untuk peta panas interaktif
* Jupyter Notebook / Quarto



> **[📊 Lihat Laporan Interaktif Lengkap (HTML)](https://s-hidayat.github.io/Bangkok-Airbnb-analysis/)**


## Author
**Samsur Hidayat** – Real Estate Data Analyst

---

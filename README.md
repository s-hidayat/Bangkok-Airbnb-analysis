# Optimizing Market Demand: Architectural Typology and Revenue Performance in Bangkok’s Airbnb

Proyek ini menganalisis listing Airbnb di Bangkok untuk mengungkap strategi investasi berbasis data. Dengan menggabungkan intelijen lokasi, atribut properti, dan estimasi pendapatan, proyek ini memberikan wawasan yang dapat ditindaklanjuti bagi investor real estat yang mencari aset berkinerja tinggi.

## Tujuan
Mengidentifikasi tipe properti, lokasi, dan fitur arsitektural yang paling menguntungkan untuk investasi sewa jangka pendek di Bangkok.

## Dataset
- Sumber: Inside Airbnb (Bangkok)
- 28.806 listing dengan 79 fitur
- Dibersihkan dan disaring menjadi 12.576 listing aktif dengan ulasan terbaru

## Metodologi
1. **Pembersihan Data**: Mem-parsing harga, kamar mandi, dan fasilitas; menangani nilai kosong; menghapus pencilan.
2. **Rekayasa Fitur**: Membuat indikator biner untuk kolam renang, ruang kerja, dapur, gym, AC.
3. **Estimasi Pendapatan**: Menggunakan "model kewajaran" (tingkat ulasan 50%, rata-rata menginap 3 malam) untuk memperkirakan pendapatan bulanan.
4. **Analisis Eksploratif**:
   - Titik panas lokasi melalui peta panas
   - Kinerja tipe properti (box plot)
   - Dampak fasilitas terhadap pendapatan
   - Efisiensi pendapatan per tamu berdasarkan kapasitas

## Temuan Utama
- **Lokasi**: Konsentrasi pendapatan tinggi mengikuti jalur BTS/MRT, bukan batas administratif distrik.
- **Tipe Properti**: Seluruh rumah/ townhouse menghasilkan pendapatan tertinggi; kamar privat berkinerja rendah.
- **Nilai Arsitektural**: Dapur (+37%) dan ruang kerja (+26%) memberikan premi harga; kolam renang dan AC kini menjadi komoditas standar.
- **Efisiensi Ruang**: Pendapatan per tamu optimal pada kapasitas 5 dan 9 tamu; unit lebih besar (>13 tamu) menunjukkan penurunan efisiensi.

## Rekomendasi
- Prioritaskan unit dengan dapur lengkap dan ruang kerja khusus.
- Hindari properti dengan biaya layanan tinggi untuk kolam/gym kecuali benar-benar diperlukan.
- Targetkan properti dekat stasiun transportasi dan optimalkan tata ruang untuk 5 atau 9 tamu.

## Tools & Libraries
- Python (pandas, numpy, matplotlib, seaborn)
- Folium untuk peta panas interaktif
- Jupyter Notebook / Quarto



> **[📊 Lihat Laporan Interaktif (HTML)](https://s-hidayat.github.io/Bangkok-Airbnb-analysis/)**


## Author
**Samsur Hidayat** – Real Estate Data Analyst

---

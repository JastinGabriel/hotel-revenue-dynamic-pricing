# 🏨 Resort Hotel Revenue Analysis

Resort hotel revenue analysis &amp; dynamic pricing engine designed to assist Revenue Managers in rate setting, OTA channel optimization, and tracking Occupancy, ADR, and RevPAR.
> 📊 **Dashboard Interaktif:** [Buka di Tableau Public](https://public.tableau.com/) *(Ganti dengan tautan Tableau Public Anda)*

## 📌 Ringkasan Eksekutif (Executive Summary)

Banyak pihak mengira **okupansi tinggi (>85%)** berarti hotel berkinerja sehat. Faktanya, Resort Hotel berkapasitas 200 kamar ini justru mengalami **okupansi semu (*false fullness*)**:
* Kamar hampir selalu terisi penuh, tetapi rata-rata harga sewa harian (**ADR**) dan pendapatan per kamar (**RevPAR**) tertinggal jauh di bawah potensinya.
* Kebanyakan Revenue dikuasai datang dari OTA (*Online Travel Agent*) dengan tarif potongan komisi tinggi
* Jika kita Menggunakan harga flat tanpa strategi penyesuaian (dynamic pricing), hal ini menyebabkan kamar terjual terlalu dini di tarif terendah. Hotel pun kehilangan potensi pendapatan tinggi dari tamu last-minute yang bersedia membayar lebih mahal.

Proyek ini menghadirkan sistem pendukung keputusan (*decision-support system*) berbasis Python dan Tableau untuk mendeteksi lonjakan pesanan mendadak dan menyesuaikan harga secara bertingkat (naik hingga +40%) sebelum kamar habis terjual murah

## 🎯 Manfaat Proyek Bagi Revenue Manager & Manajemen

* **Penetapan Tarif Harian Otomatis:** Memberi panduan penyesuaian tarif berbasis tingkat Occupancy Rate.
* **Peringatan Dini Lonjakan Permintaan (*Demand Spike Alert*):** Mendeteksi tanggal-tanggal dengan laju pesanan tak wajar.


## 🖥️ Tampilan Dashboard Tableau

![Executive Dashboard](assets/Dashboard-Preview.png)

1. **Kartu Indikator Utama (KPI Cards):** Menyajikan performa bulanan untuk *Occupancy*, *Booking Pace* harian, *ADR*, dan *RevPAR*.
2. **Kontribusi Saluran Penjualan:** Perbandingan porsi kamar dan omzet antara *TA/TO*, *Direct*, dan *Corporate*[cite: 1].
3. **Kalender Peringatan Lonjakan (*Demand Spike Alert*):** Kalender berbasis warna yang baru mulai menyala saat pesanan melonjak di atas **16%**, dan berwarna merah pekat saat lonjakan menyentuh zona kritis **$\ge 25\%$**.
4. **Tabel Tindakan Harian (*Daily Pricing Grid*):** Panduan ringkas bagi resepsionis dan tim reservasi mengenai status okupansi serta pengali tarif yang harus dipasang hari ini[cite: 1].

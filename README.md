# 📊 Excel Dashboard – CPA-1 BNI

![Dashboard Preview](Ilustrasi Dashboard CPA 1-BNI.jpg)
Catatan: Gambar diatas digunakan sebagai ilustrasi dikarenakan dashboard berisi informasi bersifat rahasia perusahaan.

## 📝 Ringkasan Proyek

Dashboard ini dikembangkan menggunakan **Microsoft Excel** berdasarkan **180.450 data nasabah korporasi BNI** dari berbagai sumber (`Mapping`, `CPA-1`, dan `CPA-2`). Proyek ini bertujuan menyederhanakan proses validasi dan analisis data melalui visualisasi yang **interaktif dan mudah digunakan**, untuk mendukung **pengambilan keputusan tim Corporate Sales Advisory** berdasarkan distribusi pelanggan menurut wilayah, sektor industri, dan penanggung jawab.

> Proyek ini berangkat dari data mentah yang sebelumnya belum dikelola dengan baik, bahkan telah menjadi permasalahan berulang sejak beberapa periode sebelumnya. Awalnya saya ditugaskan hanya untuk mengabungkan, membersihkan, serta mengvalidasi data. 

> **Melihat potensi dampak bisnis dari data ini**, serta berangkat dari **pemahaman terhadap kebutuhan tim**, saya mengambil inisiatif untuk mengembangkan dashboard secara mandiri agar tim sales dapat lebih mudah memonitor dan mengambil keputusan berdasarkan data yang tersedia. Meski belum pernah membuat dashboard sebelumnya, saya belajar secara otodidak menggunakan sumber terbatas dan menyesuaikan dengan tools yang sudah familiar digunakan oleh tim, yaitu Microsoft Excel.

---

## 🧹 Proses Pembersihan & Persiapan Data

1. **Sumber Data:**
   - Mengintegrasikan tiga sumber utama: `Mapping` (referensi utama), `CPA-1`, dan `CPA-2` (sebagai data validasi).
   - Data kemudian dipisah per penanggung jawab/sales (`PIC`)  berdasarkan informasi di mapping.

2. **Proses Rekonsiliasi:**
   - Melakukan pencocokan data antar sheet menggunakan `CIF` sebagai identifier utama melalui formula `VLOOKUP`.
   - Pemberian kode warna pada data yang cocok dan tidak cocok untuk memudahkan proses audit dan validasi.

3. **Data Cleansing & Standarisasi:**
   - Menyusun entri yang tidak cocok dalam sheet baru.
   - Penyesuaian penulisan nama nasabah dengan menghapus entitas umum seperti “PT”, “CV”, “Tbk”, simbol, dan karakter khusus.
   - Implementasi fungsi `TRIM()` untuk membersihkan spasi ganda atau karakter tak terlihat.
   - Dilakukan pencocokan ulang setelah proses cleansing terhadap data di `CPA-1` dan `CPA-2`.

4. **Validasi Manual:**
   - Data yang tidak teridentifikasi atau tidak valid dikembalikan kepada masing-masing Sales Manager untuk klarifikasi lebih lanjut.
   - Semua sheet pendukung seperti `teknik cleansing` dihapus setelah data final terintegrasi secara utuh.

5. **Tantangan Teknis:**
   - Tidak adanya unique key di nama nasabah menyebabkan satu nama nasabah dapat memiliki lebih dari satu CIF.
   - Seluruh proses dilakukan di Microsoft Excel, menuntut ketelitian tinggi dalam validasi multi-sumber.

6. **Pembangunan Dashboard:**
   - Setelah proses konsolidasi selesai, dashboard dibangun menggunakan pivot table, slicer, dan berbagai jenis visualisasi yang memungkinkan eksplorasi data yang fleksibel dan terfokus.

---

## 📈 Fitur Utama Dashboard

Dashboard akhir mencakup:

- 🔢 **Total Jumlah Nasabah** (KPI Card)
- 📍 **Distribusi Pelanggan per Wilayah** (Bar Chart)
- 🧭 **Distribusi Nasabah per Divisi** (Pie Chart)
- 🗓️ **Update Timeline per Bulan & Kuartal** (Line Chart)
- 🏭 **Sektor Industri Nasabah** (Horizontal Bar Chart)
- 🧑‍💼 **Klasifikasi Tipe Nasabah** (Pie Chart):
  - Personal  
  - Pemerintah  
  - Korporasi Non-Bank  
  - Korporasi Bank
- 📁 **Daftar Nama dan Group Nasabah** (List)


### 🎛️ Fitur Interaktif:

Dashboard dilengkapi dengan slicer dan filter untuk membantu pengguna memfokuskan analisis berdasarkan:

- **Nama Sales**  
- **Divisi Penjualan**  
- **Sektor Industri**  
- **Wilayah Operasional**  
- **Periode Waktu: Tahun / Bulan / Kuartal**

---

## 📁 Struktur File

- `Mapping CPA1` – Sheet referensi untuk penugasan PIC  
- `CPA 1 & CPA 2` – Data nasabah mentah dari sumber distribusi  
- `Cleansing` – Sheet proses standarisasi dan validasi nama nasabah  
- `Pivot` – Pivot table pendukung visualisasi  
- `Dashboard` – Dashboard akhir berbasis Excel

---

## 🔍 Nilai Tambah & Hasil Akhir

Dashboard ini memberikan kontribusi strategis dalam:

- Memetakan portofolio nasabah korporasi secara terstruktur berdasarkan wilayah dan sektor industri.
- Meningkatkan efisiensi proses monitoring coverage sales.
- Memperkuat fungsi advisory melalui data yang lebih bersih, terstandarisasi, dan siap dianalisis.
- Memberikan tools visual yang membantu pengambilan keputusan berbasis data secara cepat, akurat, dan terarah.

---

> 🚀 Proyek ini menunjukkan inisiatif pribadi saya untuk menyelesaikan masalah nyata di lapangan melalui pendekatan data-driven, meski di luar jobdesk awal.  
> Saya percaya bahwa visualisasi yang sederhana namun tepat sasaran mampu meningkatkan efektivitas tim dan membuka peluang analisis yang lebih luas ke depannya.

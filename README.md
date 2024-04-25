# CapstoneProjectM2_SaaSSales

# Table of Content
0. Import Labraries
1. Define Problem
2. Data Understanding & Cleaning
3. Exploratory Data Analysis (EDA)
4. Conclusion & Recommendation

    
## Business Problem
SaaS adalah singkatan dari Software-as-a-Service. Ini adalah model pengiriman/penjualan perangkat lunak di mana penyedia pihak ketiga menghosting aplikasi dan membuatnya tersedia untuk Customer melalui Internet. Customer dapat mengakses aplikasi tersebut melalui browser dan membayar langganan bulanan untuk penggunaannya. AWS menghasilkan pendapatan dari penjualan langganan perangkat lunak mereka kepada Customer mereka, yang mana sebagian besar aplikasi yang mereka jual dijual dengan model langganan bulanan.

Dengan memahami bagaimana pemberian diskon memengaruhi profitabilitas, mengetahui tren penjualan yang berhubungan dengan kinerja produk, serta mengidentifikasi kontribusi Customer dan kinerja produk terhadap penjualan berdasarkan wilayah, perusahaan dapat mengambil keputusan yang lebih tepat dalam mengalokasikan sumber daya, menyesuaikan strategi pemasaran, dan meningkatkan kepuasan Customer secara keseluruhan.

Sebuah perusahaan yang menyediakan perangkat lunak sebagai layanan (Software As A Service). Perusahaan ingin mengoptimalkan strategi penjualan, meningkatkan profitabilitas, dan memahami lebih baik kebutuhan dan preferensi Customer. Oleh karena itu, perusahaan ingin merekrut Data Analis agar dapat mendapatkan wawasan yang berharga untuk membantu kemajuan perusahaan tersebut. Adapun beberapa pernyataan masalah terkait analasis yang akan dilakukan:
Dari pernyataan tersebut, dapat dirumuskan pertanyaan-pertanyaan lanjutan yang lebih rinci sebagai berikut:

  1. Bagaimana penggunaan diskon dan pengaruhnya terhadap profitabilitas perusahaan?
      - Perbandingan Transaksi Menggunakan Diskon
      - Hubungan antara tingkat diskon dengan margin keuntungan, dan Identifikasi titik optimal 
      - Tren pemberian diskon titik optimal dengan diskon diatas titik optimal.
  2. Bagaimana tren penjualan utama yang dapat diidentifikasi dari data historis?
      - Identifikasi tren dan pola penjualan dari data historis.
  3. Bagaimana kontribusi Customer terhadap perusahaan?
      - Identifikasi kontribusi Customer.
      - Faktor yang mempengaruhi kontribusi Customer yang janggal.
  4. Bagaimana kinerja produk terhadap penjualan antar wilayah geografis?
      - Identifikasi Kinerja Produk terhadap Profitabilitas Perusahaan berdasarkan Wilayah Geografis
      - Faktor yang mempengaruhi perbedaan keuntungan yang didapatkan dari produk yang unggul dan rugi

## Data Understanding and Preparation
Langkah pertama yang kita lakukan adalah memahami data dan melakukan data cleaning terhadap dataset untuk memaksimalkan proses analisis data
Data SaaS Sales yang digunakan bersumber dari [Kaggle](https://www.kaggle.com/datasets/nnthanh101/aws-saas-sales),
Dataset ini berisi informasi terkait aktivitas penjualan layanan software selama tahun 2020 sd th 2023. Ada 18 kolom di dalam dataset AWS SaaS Sales, yaitu:  

1. `Order ID`: Kode unik yang berbeda di setiap transaski.
2. `Order Date`: Tanggal ketika transaski dilakukan. 
3. `Date Key`: Angka yang merepresentasikan tanggal transaksi (YYYYMMDD). 
4. `Contact Name`: Contact Person (PIC) dari yang melakukan transaksi.
5. `Country`: Negara asal dari Perusahaan yang melakukan transaksi. 
6. `City`: Kota asal dari Perusahaan yang melakukan transaksi. 
7. `Region`: Wilayah dari Negara yang melakukan transaksi. 
8. `Subregion`: sub-Wilayah dari Negara yang melakukan transaksi.
9. `Customer`: Nama Perusahaan yang melakukan transaksi. 
10. `Customer ID`: Kode unik dari Customer. 
11. `Industry`: Industri dari Perusahaan. 
12. `Segment`: Segmen Perusahaan dari Customer (`SMB = Small, Medium Business`, `Enterprise`, `Strategic`).
13. `Product`: Product yang dibeli. 
14. `License`: Kode lisensi dari produk. 
15. `Sales`: Jumlah total penjualan dari transaksi. 
16. `Quantity`:  Jumlah item kuantitas dari transaksi. 
17. `Discount`: Diskon yang diberikan pada transaksi.
18. `Profit`: Keuntungan yang diperoleh dari transaksi. 

Dalam data understanding dan cleaning, kita melakukan sebagai berikut: 
1. Data Understanding
   - Melihat informasi dataset
   - Penyesuaian datatypes
   - Pengurangan dan penambahan kolom
   - Melakukan stastika deskriptif untuk mengetahui mean, nilai min & max, melihat distribusi data, mengecek outliers dan juga melihat menghitung korelasi antar kolom numerik.
   - Menghitung jumlah unique values dari kolom kategorik, dan melihat modus dari masing-masing kolom.
3. Data Cleaning
   - Melakukan perubahan tipe data pada kolom Order Date menjadi datetime, mengecek data outlier, dan distribusi data.
   - Pengecakan Missing dan Duplicated Values


## Exploratory Data Analysis
Dalam EDA, kita akan melakukan analisis permasalahan yang terdapat pada SaaS Sales ini dari beberapa aspek, yaitu:
  1. **Pengaruh Diskon terhadap Profitabilitas**
  2. **Tren Penjualan dan Kinerja Produk**
  3. **Kontribusi Customer terhadap Kinerja Perusahaan**
  4. **Kinerja Produk terhadap Penjualan Berdasarkan Region** 


## Dashboard Tableau
untuk dashboard SaaS Sales dapat diakses melalui link berikut : [Tableau](https://public.tableau.com/views/SaaSSales_17136300695510/SaaSDashboard?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link)

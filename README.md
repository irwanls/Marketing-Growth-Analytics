# Marketing Strategy – Data Marketing Growth Analytics

## Deskripsi Project

Project ini merupakan analisis **Marketing Growth Analytics** yang bertujuan untuk mengevaluasi performa strategi pemasaran dalam menghasilkan revenue. Analisis berfokus pada bagaimana pengguna mengenal perusahaan, perjalanan pengguna hingga melakukan pembelian, efektivitas setiap marketing channel, serta potensi revenue yang dapat dioptimalkan.

Latar belakang project menggunakan contoh strategi marketing Erigo yang berhasil memanfaatkan media sosial dan kolaborasi untuk meningkatkan penjualan. Dari kasus tersebut, project ini berfokus pada bagaimana data dapat digunakan untuk menganalisis performa marketing dalam menghasilkan revenue. :chatgpt-content-reference{index="0"}

## Dataset

Dataset yang digunakan:

[data_marketing_growth_analytics.csv](https://drive.google.com/file/d/16YPDZhN2sMJHJ5zdzvWKRuyknJokaRZY/view)

Dataset terdiri dari:

- **800 baris**
- **16 kolom**

Data mencakup informasi mengenai pengguna, channel marketing, source, device, session, page views, bounce, add to cart, purchase, revenue, advertising cost, clicks, impressions, repeat purchase, dan retention. 

## Tahapan Analisis

Analisis dilakukan melalui beberapa tahapan utama:

1. **Problem Statement**
2. **Data Understanding**
3. **Data Preparation**
4. **Visualization**
5. **Recommendation** 

### Data Preparation

Proses persiapan data meliputi pemeriksaan:

- Data type dan missing value
- Duplicate data
- Konsistensi data kategorikal
- Outlier

Hasil pengecekan menunjukkan tidak terdapat missing value pada dataset, tetapi kolom `first_visit_date` perlu diubah menjadi tipe data tanggal. 

Tidak ditemukan baris duplikat pada dataset.

Pengecekan pada kolom kategorikal juga menunjukkan tidak terdapat kategori yang tidak konsisten sehingga tidak diperlukan penanganan tambahan. 
## Hasil Analisis

### 1. Marketing Channel

Channel terbesar yang mengenalkan pengguna kepada perusahaan adalah:

- **Paid Ads: 31.38%**
- **Organic Search: 24.75%**
- **Social Media: 18.88%**

Paid Ads menjadi channel dengan jumlah pengguna terbesar pada tahap awal customer acquisition. 
### 2. Customer Journey

Dari **800 pengguna** yang mengunjungi website:

- **329 pengguna** melakukan Add to Cart
- **150 pengguna** melakukan Purchase

Bottleneck terbesar terdapat pada tahap menuju purchase dengan penurunan pengguna sebesar **45.59%**. Hal ini menjadi perhatian karena purchase merupakan aktivitas utama yang menghasilkan revenue bagi perusahaan. 

### 3. Purchase Rate

Berdasarkan purchase rate, **Social Media** menjadi channel dengan performa terbaik dengan purchase rate sebesar **22.52%**.

Urutan performa channel berdasarkan purchase rate adalah:

1. Social Media
2. Paid Ads
3. Referral
4. Email
5. Organic Search 

### 4. Average Revenue per User

Social Media juga memiliki **ARPU (Average Revenue per User)** tertinggi sebesar **Rp69.622 per user**, kemudian diikuti oleh Referral, Paid Ads, Organic Search, dan Email. 

### 5. Potensi Channel Referral

Channel Referral memiliki potensi untuk dikembangkan lebih lanjut.

Referral memiliki:

- **ARPU: Rp59.287 per user**
- **Purchase Rate: 18.67%**

ARPU Referral relatif tinggi, tetapi purchase rate masih berada di bawah Social Media dan Paid Ads. Peningkatan purchase rate pada channel Referral berpotensi menghasilkan revenue yang lebih besar. 

## Kesimpulan

Berdasarkan hasil analisis:

- **Social Media** menjadi marketing channel dengan performa terbaik dari sisi **Purchase Rate** dan **ARPU**.
- **Referral** memiliki potensi revenue yang tinggi sebesar **Rp59.287 per user**, tetapi purchase rate masih sebesar **18.67%**.
- Peningkatan conversion pada Referral dapat menjadi salah satu peluang untuk meningkatkan revenue perusahaan. 

## Recommendation

Strategi yang direkomendasikan adalah meningkatkan performa channel Referral melalui program seperti:

- Referral code
- Voucher **“Ajak Teman”**
- Reward untuk existing customer

Program tersebut diarahkan untuk meningkatkan purchase rate dari pengguna yang berasal dari Referral sehingga potensi revenue channel ini dapat dimaksimalkan. 

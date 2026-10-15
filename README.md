# Marketing Growth Analytics

## Project Overview

Project ini bertujuan untuk menganalisis performa marketing dalam menghasilkan revenue berdasarkan perilaku pengguna dan channel marketing yang digunakan.

Analisis difokuskan pada perjalanan pengguna mulai dari pertama kali mengenal perusahaan, melakukan interaksi dengan platform, menambahkan produk ke cart, hingga akhirnya melakukan purchase. Selain itu, project ini juga membandingkan performa masing-masing marketing channel berdasarkan **Purchase Rate** dan **Average Revenue per User (ARPU)** untuk mengidentifikasi channel dengan performa terbaik serta peluang yang masih dapat dioptimalkan.

Dataset yang digunakan adalah:

**`data_marketing_growth_analytics.csv`**

- Total Rows: **800**
- Total Columns: **16**

Beberapa informasi yang dianalisis mencakup channel acquisition, source, device, sessions, page views, bounce, add to cart, purchase, revenue, ad cost, clicks, impressions, repeat purchase, dan retention month.

---

## Data Quality & Preparation

Sebelum melakukan analisis, dilakukan proses pengecekan kualitas data untuk memastikan dataset dapat digunakan secara konsisten.

### 1. Data Types & Missing Values

Hasil pengecekan menunjukkan bahwa seluruh kolom pada dataset tidak memiliki **missing value**.

Namun, kolom `first_visit_date` perlu disesuaikan tipe datanya menjadi format **date** agar dapat digunakan dengan tepat dalam analisis berbasis waktu.

### 2. Duplicate Data

Tidak ditemukan baris yang terduplikasi pada dataset sehingga tidak diperlukan proses penghapusan duplicate data.

### 3. Data Consistency

Pengecekan juga dilakukan terhadap kolom kategorikal seperti `channel`, `source`, dan `device`.

Hasil pemeriksaan menunjukkan bahwa tidak terdapat kategori yang tidak konsisten sehingga tidak diperlukan proses standardisasi tambahan.

### 4. Outlier

Pengecekan outlier dilakukan pada seluruh variabel numerik.

Beberapa outlier teridentifikasi pada variabel:

- `bounce`
- `repeat_purchase`
- `purchase`
- `revenue`
- `retention_month`

Outlier tersebut tetap dipertahankan dan tidak dilakukan treatment tambahan.

---

## Marketing Analysis

### 1. Dari Mana User Mengenal Perusahaan?

Berdasarkan channel pertama yang membawa pengguna mengenal perusahaan, **Paid Ads** menjadi channel dengan proporsi pengguna terbesar.

Distribusi pengguna berdasarkan channel utama:

- **Paid Ads: 31.38%**
- **Organic Search: 24.75%**
- **Social Media: 18.88%**

Hasil ini menunjukkan bahwa Paid Ads memiliki kontribusi terbesar dalam mendatangkan awareness dan traffic awal.

---

### 2. User Journey & Conversion Funnel

Dari total **800 pengguna** yang pernah mengunjungi website:

- **329 pengguna** melakukan Add to Cart.
- **150 pengguna** akhirnya melakukan Purchase.

Bottleneck terbesar dalam funnel terjadi pada proses menuju purchase.

Terjadi penurunan sebesar **45.59%** dari pengguna yang sudah memasukkan produk ke cart menuju pengguna yang benar-benar melakukan pembelian.

Hal ini menjadi perhatian penting karena purchase merupakan aktivitas utama yang secara langsung menghasilkan revenue bagi perusahaan.

---

### 3. Channel dengan Purchase Rate Terbaik

Jika dibandingkan berdasarkan **Purchase Rate**, Social Media menjadi channel dengan performa terbaik.

**Social Media memiliki Purchase Rate sebesar 22.52%.**

Urutan performa channel berdasarkan Purchase Rate adalah:

1. Social Media
2. Paid Ads
3. Referral
4. Email
5. Organic Search

Hasil tersebut menunjukkan bahwa meskipun Paid Ads mendatangkan jumlah user terbesar, Social Media memiliki efektivitas yang lebih tinggi dalam mengubah pengguna menjadi pembeli.

---

### 4. Revenue Potential per Channel

Selain Purchase Rate, performa channel juga dianalisis menggunakan **Average Revenue per User (ARPU)**.

Social Media kembali menunjukkan performa tertinggi dengan:

**ARPU: Rp69,622 per user**

Diikuti oleh:

1. Social Media
2. Referral
3. Paid Ads
4. Organic Search
5. Email

Hasil ini menunjukkan bahwa Social Media tidak hanya memiliki Purchase Rate tertinggi, tetapi juga menghasilkan revenue rata-rata per user tertinggi.

---

## Growth Opportunity

Salah satu channel yang memiliki potensi untuk dikembangkan lebih lanjut adalah **Referral**.

Referral memiliki:

- **ARPU: Rp59,287 per user**
- **Purchase Rate: 18.67%**

Nilai ARPU Referral tergolong cukup tinggi, tetapi Purchase Rate-nya masih berada di bawah Social Media.

Kondisi tersebut menunjukkan adanya peluang untuk meningkatkan jumlah pengguna Referral yang akhirnya melakukan purchase.

Jika Purchase Rate Referral dapat ditingkatkan, channel ini berpotensi memberikan kontribusi revenue yang lebih besar bagi perusahaan.

---

## Recommendation

Berdasarkan hasil analisis, perusahaan dapat mengembangkan program referral untuk meningkatkan Purchase Rate dari channel Referral.

Beberapa bentuk program yang dapat digunakan antara lain:

- Referral Code
- Voucher "Ajak Teman"
- Reward bagi existing customer yang berhasil mengajak pengguna baru

Strategi ini diarahkan untuk meningkatkan konversi pengguna dari channel Referral sehingga potensi revenue dari channel tersebut dapat dimaksimalkan.

---

## Conclusion

Hasil analisis menunjukkan bahwa **Social Media merupakan marketing channel dengan performa terbaik**, baik berdasarkan Purchase Rate maupun Average Revenue per User (ARPU).

Social Media memiliki:

- **Purchase Rate tertinggi: 22.52%**
- **ARPU tertinggi: Rp69,622 per user**

Namun, terdapat peluang pertumbuhan pada **Referral Channel**.

Referral telah menghasilkan **ARPU sebesar Rp59,287 per user**, tetapi Purchase Rate masih berada pada **18.67%**.

Oleh karena itu, meningkatkan conversion rate dari channel Referral melalui program seperti referral code, voucher ajak teman, atau customer reward dapat menjadi salah satu strategi untuk meningkatkan revenue perusahaan.

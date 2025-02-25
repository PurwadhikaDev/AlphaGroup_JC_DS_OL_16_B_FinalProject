# Optimalisasi Strategi Telemarketing dan Prediksi Nasabah Potensial dalam  Kampanye Penawaran Term Deposit

Anggota Kelompok:

Destaria Anripal
Hermily Tjia

Tableau Link: https://public.tableau.com/app/profile/hermily1937/viz/AlphaGroup_Telemarketing_Bank_Campaign/Dashboard1?publish=yes

## Konteks

## Permasalahan
Perbankan di Portugal memainkan peran penting dalam perekonomian dengan menyediakan berbagai layanan keuangan, termasuk produk investasi seperti *term deposit*. Produk ini memberikan keuntungan bagi bank dalam menjaga stabilitas keuangan serta menawarkan opsi investasi berisiko rendah bagi nasabah. Namun, konversi pelanggan ke produk ini masih menjadi tantangan, terutama dalam strategi pemasaran yang dilakukan melalui telemarketing.

Tagus Bank menggunakan strategi telemarketing untuk menawarkan term deposit kepada nasabah. Meskipun metode ini memungkinkan bank menjangkau lebih banyak nasabah, efektivitasnya masih dipertanyakan karena banyak panggilan yang tidak menghasilkan konversi. Data menunjukkan bahwa dari seluruh kampanye yang telah dilakukan, hanya **11,3% nasabah yang menerima tawaran term deposit, sementara 88,7% lainnya menolak.** Selain itu, faktor seperti status pekerjaan, usia, riwayat kampanye sebelumnya, dan durasi panggilan diduga memiliki korelasi dengan keputusan nasabah dalam menerima atau menolak penawaran.

Tingginya tingkat penolakan ini mengindikasikan bahwa strategi telemarketing saat ini belum optimal dalam meningkatkan *conversion rate*. Untuk meningkatkan keberhasilan kampanye, diperlukan pendekatan berbasis data guna mengidentifikasi pola dan karakteristik nasabah yang lebih mungkin menerima penawaran. Dengan memahami faktor-faktor utama yang memengaruhi keputusan nasabah, tim telemarketing dapat menyusun strategi yang lebih tepat sasaran dan meningkatkan peluang konversi.

Oleh karena itu, **Head of Telemarketing** di Tagus Bank meminta tim Data Scientist untuk melakukan analisis data dan membangun model prediktif guna mengoptimalkan strategi pemasaran dan meningkatkan rasio konversi telemarketing. Model ini diharapkan dapat membantu tim telemarketing dalam menentukan kelompok nasabah dengan probabilitas konversi lebih tinggi, sehingga upaya pemasaran dapat lebih efektif dan terarah.

Target:  
- 0: Nasabah menolak penawaran term deposit
- 1: Nasabah menerima penawaran term deposit

## Rumusan Masalah
Strategi telemarketing yang tidak terarah dapat menyebabkan upaya pemasaran kurang efektif, menghabiskan waktu tim telemarketing, dan menurunkan peluang konversi. Saat ini, Tagus Bank menghadapi tantangan dalam meningkatkan conversion rate term deposit, karena kampanye telemarketing masih dilakukan secara luas tanpa mempertimbangkan karakteristik atau riwayat interaksi nasabah.

Jika strategi telemarketing tetap dilakukan secara acak tanpa analisis berbasis data, beberapa permasalahan yang dapat terjadi meliputi:
    
- Conversion Rate dari team Telemarketing tidak meningkat karena aktifitas telemarketing tidak difokuskan ke dataset yang memiliki potensial closing yang lebih besar.
    
- Aktifitas telemarketing yang tidak terarah (Spray and Prey) akan mengakibatkan konversi Nasabah tidak dapat diprediksi dengan baik, sehingga sales Forecast di team Telemarketing akan kurang tepat dan tidak dapat dikontrol.

Dengan adanya analisis yang memahami pola nasabah yang lebih responsif terhadap penawaran serta metode komunikasi yang paling efektif, team telemarketing bisa memprioritaskan aktifitas cold-calling menggunakan metode komunikasi yang lebih efektif dan ke kelompok Nasabah yang memiliki conversion rate tinggi.

Berdasarkan Dataset yang digunakan, sebagian besar Nasabah yang dihubungi team Telemarketing adalah nasabah baru.

## Tujuan
Berdasarkan permasalahan tersebut, Tagus Bank ingin membangun model prediktif untuk mengidentifikasi nasabah dengan probabilitas tinggi menerima penawaran *term deposi*. Dengan model ini, tim telemarketing dapat memprioritaskan panggilan kepada prospek yang lebih potensial, sehingga meningkatkan *conversion rate* dan mengoptimalkan hasil dari setiap kampanye telemarketing. Untuk itu, kita akan melakukan analisis berbasis data dengan menjawab pertanyaan berikut:

1. Bagaimana karakteristik demografis dan finansial nasabah memengaruhi keputusan mereka dalam menerima atau menolak penawaran term deposit?

2. Bagaimana efektivitas strategi kampanye saat ini dalam meningkatkan peluang nasabah menerima penawaran term deposit?

3. Sejauh mana riwayat interaksi nasabah dalam kampanye sebelumnya dan hasil kampanye sebelumnya memengaruhi kemungkinan mereka menerima penawaran term deposit pada kampanye saat ini?

4. Bagaimana kondisi ekonomi makro memengaruhi keputusan nasabah dalam menerima penawaran term deposit?

Selain itu, bank juga ingin mengidentifikasi faktor-faktor utama yang memengaruhi keputusan nasabah dalam menerima atau menolak penawaran. Dengan wawasan ini, strategi telemarketing dapat disesuaikan agar lebih efektif, meningkatkan kualitas interaksi dengan nasabah, dan secara keseluruhan memperbaiki pendekatan pemasaran yang digunakan.


## Pendekatan Analisis
Untuk mengoptimalkan strategi telemarketing, kita akan melakukan analisis data guna mengidentifikasi pola yang membedakan nasabah yang menerima dan menolak penawaran term deposit. Analisis ini mencakup karakteristik demografi dan finansial nasabah, efektivitas kampanye saat ini, hasil kampanye sebelumnya, serta dampak kondisi makroekonomi terhadap keputusan nasabah.

Setelah itu, kita akan membangun model klasifikasi berbasis Supervised Machine Learning untuk memprediksi probabilitas seorang nasabah menerima term deposit. Model ini akan menjadi alat bantu bagi tim telemarketing dalam pengambilan keputusan, sehingga strategi pemasaran lebih terarah dan efektif.

Berikut tahapan analisis dan pengembangan model yang akan dilakukan:
- **Data Cleaning**: Menangani data yang hilang, inkonsisten, atau duplikasi.
- **Exploratory Data Analysis (EDA)**: Memahami pola dalam data melalui visualisasi dan statistik deskriptif.
- **Feature Engineering & Preprocessing**: Mengubah dan menyesuaikan fitur agar optimal untuk model.
- **Benchmarking Model**: Mencoba beberapa algoritma Klasifikasi Supervised Machine Learning untuk menentukan model dengan performa terbaik.
- **Hyperparameter Tuning**: Mengoptimalkan parameter model untuk meningkatkan akurasi prediksi.
- **Model Evaluation & Selection**: Mengevaluasi model dengan metrik yang sesuai dengan tujuan bisnis.
- **Implementation**: Menerapkan model sebagai alat bantu bagi tim telemarketing dalam pengambilan keputusan.

## Metrik Evaluation
Metrik evaluasi yang akan digunakan adalah Precision dan F0.5 Score dengan keterangan sebagai berikut:

|  | Menolak Tawaran (0) | Menerima Tawaran (1) |
| --- | --- | --- |
| **Menolak Tawaran (0)** | **True Negative (TN)** | **False Positif (FP)** |
|  | Model memprediksi nasabah menolak tawaran deposito dan kenyataan nya nasabah memang tidak menerima tawaran. | Model memprediksi nasabah menerima tawaran deposito namun di kenyataannya nasabah tidak menerima tawaran deposito.|
| **Menerima Tawaran (1)** | **False Negatif (FN)** | **True Positif (TP)** |
|  | Model memprediksi nasabah menolak tawaran deposito namun dikenyataannya nasabah menerima tawaran. | Model memprediksi nasabah menerima tawaran deposito, dan di kenyataan nya nasabah memang menerima tawaran deposito.|


---



| **Tipe error** | **Konsekuensi** |
| --- | --- |
| False Positive | Kehilangan sumberdaya tanpa peningkatan convertion rate|
| False Negative | Kehilangan nasabah potensial sehingga menurunkan konversi|

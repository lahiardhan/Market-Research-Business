# Market Research for Business Decision-Making: Customer Churn Analysis for DQLab Sport Center

## 1. Background
DQLab Sport Center adalah sebuah toko ritel yang menyediakan berbagai produk olahraga seperti jaket, baju, tas, dan sepatu, dengan pelanggan setia sejak toko ini berdiri pada tahun 2013. Namun, belakangan ini, terjadi penurunan jumlah pelanggan yang melakukan pembelian ulang (repeat customers), yang dapat berdampak negatif pada pendapatan toko. Untuk memahami penyebab churn dan menyusun strategi yang tepat untuk mengurangi churn, manajemen memberikan data transaksi dari tahun 2013 hingga 2019 untuk dilakukan analisis.

## 2. Objective
- Mengidentifikasi pelanggan yang memiliki kemungkinan tinggi untuk churn.
- Menggali fitur atau pola yang paling berpengaruh dalam memprediksi churn.
- Memberikan rekomendasi berbasis data untuk membantu manajemen mengurangi churn.
- Menyediakan visualisasi hasil analisis dan rekomendasi untuk membantu dalam pengambilan keputusan bisnis.

## 3. Scope of the Project
- **Data Collection and Preparation**: Menggunakan data transaksi yang mencakup atribut pelanggan seperti jumlah transaksi, perbedaan tahun sejak transaksi terakhir, dan jumlah rata-rata transaksi.
- **Feature Engineering**: Mendefinisikan churn berdasarkan data transaksi dan membuat variabel yang relevan untuk memprediksi churn.
- **Model Development**: Membangun model prediksi churn menggunakan beberapa algoritma machine learning (termasuk Logistic Regression, Random Forest, SVM, dan Gradient Boosting).
- **Hyperparameter Tuning**: Mengoptimalkan model Gradient Boosting yang menunjukkan performa terbaik dengan menggunakan *RandomizedSearchCV*.
- **Model Evaluation**: Mengevaluasi kinerja model dengan metrik akurasi, presisi, dan recall.
- **Interpretability Analysis**: Menggunakan SHAP untuk memahami fitur mana yang paling berpengaruh dalam prediksi churn.
- **Recommendations**: Menyusun rekomendasi yang spesifik berdasarkan hasil analisis dan interpretasi model untuk mengurangi churn.

## 4. Approach
- **Exploratory Data Analysis (EDA)**: Menganalisis data untuk memahami distribusi, pola, dan karakteristik fitur yang ada.
- **Feature Selection and Engineering**: Mengidentifikasi dan menyiapkan fitur yang relevan, seperti *Count_Transaction*, *Year_Diff*, dan *Average_Transaction_Amount*.
- **Model Training**: Melatih beberapa model machine learning untuk membandingkan performanya, dan memilih model terbaik berdasarkan metrik evaluasi.
- **Hyperparameter Tuning**: Mengoptimalkan model Gradient Boosting menggunakan *RandomizedSearchCV* untuk mencapai hasil terbaik.
- **Interpretation and Visualization**: Menggunakan visualisasi dan interpretasi model untuk memahami pola churn pelanggan.
- **Insight and Recommendations**: Menyusun rekomendasi bisnis yang actionable untuk mengurangi churn berdasarkan hasil analisis fitur dan prediksi model.

## 5. Findings
- **Feature Importance**: Fitur *Count_Transaction* memiliki dampak terbesar terhadap prediksi churn, diikuti oleh *Year_Diff* dan *Average_Transaction_Amount*. Ini mengindikasikan bahwa pelanggan dengan jumlah transaksi yang lebih rendah dan yang tidak melakukan pembelian selama periode tertentu lebih cenderung untuk churn.
- **Model Performance**: Gradient Boosting menghasilkan performa terbaik dalam prediksi churn, dengan akurasi, presisi, dan recall yang paling tinggi dibandingkan dengan model lainnya.
- **Interpretability**: Analisis SHAP menunjukkan bagaimana setiap fitur mempengaruhi keputusan model, sehingga memungkinkan untuk memberikan insight yang lebih mendalam kepada pemangku kepentingan.

## 6. Recommendations
- **Retention Campaign**: Menargetkan pelanggan dengan *Count_Transaction* rendah melalui promosi atau insentif khusus untuk mendorong pembelian ulang.
- **Engagement Strategy**: Membuat program loyalty atau program membership bagi pelanggan setia untuk meningkatkan keterlibatan dan mencegah churn.
- **Follow-up on Inactive Customers**: Menghubungi pelanggan yang sudah tidak bertransaksi dalam 6 bulan terakhir, mungkin dengan menawarkan diskon atau penawaran eksklusif.
- **Visual Communication**: Menyajikan hasil analisis dalam bentuk visualisasi interaktif untuk membantu manajemen dalam memahami insight yang dihasilkan, sehingga dapat diterapkan dalam strategi bisnis yang efektif.

## 7. Conclusion
Dengan memahami faktor-faktor utama yang mempengaruhi churn di DQLab Sport Center, manajemen dapat menerapkan strategi yang lebih efektif untuk mempertahankan pelanggan dan meningkatkan loyalitas. Model Gradient Boosting yang telah dioptimalkan memberikan prediksi yang dapat diandalkan, serta insight yang actionable untuk membantu DQLab Sport Center mengurangi churn dan mendorong retensi pelanggan di masa mendatang.

---

## Libraries
- Python 3.x
- Pandas
- Scikit-Learn
- SHAP
- Matplotlib & Seaborn

## How to Run
1. Clone repository ini ke komputer Anda.
2. Pastikan Anda memiliki Python 3.x dan menginstal dependensi yang tercantum di atas.
3. Jalankan notebook pada folder `notebooks/` untuk mengikuti langkah-langkah analisis.

---
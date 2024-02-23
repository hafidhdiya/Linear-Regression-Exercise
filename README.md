# Linear Regression Exercise

### 1. Pendahuluan
Dataset yang digunakan adalah [Real Estate Price Prediction](https://www.kaggle.com/datasets/quantbruce/real-estate-price-prediction) dari Kaggle. Tujuan dari proyek ini adalah untuk memprediksi harga real estat berdasarkan beberapa fitur yang diberikan dalam dataset.

### 2. Data Cleaning
Proses data cleaning umumnya melibatkan langkah-langkah seperti menghapus nilai yang hilang atau tidak valid, menangani outlier, dan melakukan normalisasi atau standarisasi jika diperlukan. Namun, untuk langkah ini, kita akan melihat apakah ada nilai yang hilang atau fitur yang tidak relevan untuk dihapus.

### 3. Seleksi Fitur
Untuk menentukan fitur-fitur yang tidak berpengaruh, kita dapat menggunakan uji statistik seperti F-test dan T-test. F-test digunakan untuk mengetahui apakah ada setidaknya satu fitur yang secara signifikan berhubungan dengan variabel target, sedangkan T-test digunakan untuk menguji signifikansi koefisien setiap fitur.

### 4. Model Regresi Linear
Setelah seleksi fitur, langkah selanjutnya adalah membangun model regresi linear. Model ini memiliki bentuk umum:

\[ Y = b_0 + b_1X_1 + b_2X_2 + ... + b_nX_n + \varepsilon \]

di mana:
- \( Y \) adalah variabel target (harga real estat).
- \( X_1, X_2, ..., X_n \) adalah fitur-fitur yang dipilih.
- \( b_0, b_1, b_2, ..., b_n \) adalah koefisien.
- \( \varepsilon \) adalah kesalahan acak.

R-squared (koefisien determinasi) adalah metrik evaluasi yang mengukur seberapa baik model kita cocok dengan data. Nilai R-squared berkisar antara 0 hingga 1, di mana semakin dekat ke 1, semakin baik modelnya.

Interpretasi koefisien dan konstanta \( b_0, b_1, ..., b_n \) adalah sebagai berikut:
- \( b_0 \) adalah intercept, yang menunjukkan nilai prediksi ketika semua fitur lainnya nol.
- \( b_1, b_2, ..., b_n \) adalah koefisien untuk masing-masing fitur yang menunjukkan seberapa banyak perubahan yang diharapkan dalam variabel target untuk setiap perubahan satu unit dalam fitur terkait, dengan asumsi fitur lainnya tetap.

Dengan memahami koefisien ini, kita dapat menafsirkan efek masing-masing fitur terhadap harga real estat.

Ini adalah penjelasan dan langkah-langkah umum untuk menyelesaikan proyek seperti ini. Langkah-langkah ini memberikan landasan untuk membersihkan data, memilih fitur yang relevan, membangun model, dan menafsirkan hasilnya.

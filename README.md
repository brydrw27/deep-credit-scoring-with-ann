# Deep Credit Scoring System: Artificial Neural Network & PCA

Proyek ini adalah implementasi *end-to-end Machine Learning* untuk mengevaluasi kelayakan kredit nasabah (probabilitas gagal bayar/ *default*) berdasarkan metrik finansial komprehensif. Aplikasi ini dirancang menggunakan arsitektur **Artificial Neural Network (ANN)** yang dikombinasikan dengan **Principal Component Analysis (PCA)**.


## Pendekatan Analitis dan Statistika
Tantangan terbesar dalam data finansial adalah *multicollinearity* antar variabel seperti *Loan-to-Value (LTV)*, *Debt-to-Income Ratio (dtir1)*, dan *Credit Score*. Pipeline proyek ini dirancang untuk mengatasi hal tersebut melalui:
1. Pemisahan Data Ketat: Mencegah *data leakage* dengan melakukan *train-test split* sebelum tahap imputasi statistik.
2. Penanganan Imbalance Data (SMOTE): Menyeimbangkan kelas minoritas (kasus gagal bayar) agar model tidak bias terhadap mayoritas nasabah lancar.
3. Reduksi Dimensi (PCA): Mentransformasi fitur-fitur finansial multivariat menjadi matriks komponen ortogonal untuk mengoptimalkan kinerja *Neural Network* dan mengurangi *noise*.

## Teknologi yang Digunakan
* Bahasa Pemrograman: Python
* Machine Learning & Deep Learning: TensorFlow / Keras, Scikit-Learn, Imbalanced-learn
* Data Processing & Analisis: Pandas, NumPy
* Deployment: Streamlit, FastAPI, Hugging Face Spaces

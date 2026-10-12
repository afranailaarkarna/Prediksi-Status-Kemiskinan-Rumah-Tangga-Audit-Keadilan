# Prediksi Status Kemiskinan Rumah Tangga – Audit Keadilan

## Deskripsi Proyek

Proyek ini bertujuan untuk membangun model *machine learning* yang dapat memprediksi status kemiskinan rumah tangga berdasarkan karakteristik sosial dan ekonomi rumah tangga.

Selain mengevaluasi kemampuan model dalam melakukan prediksi, proyek ini juga melakukan **audit keadilan (*fairness audit*)** untuk melihat apakah model memberikan hasil yang relatif adil pada kelompok masyarakat yang berbeda.

Pendekatan ini penting karena model prediksi yang memiliki akurasi tinggi belum tentu memberikan hasil yang adil bagi seluruh kelompok. Oleh karena itu, analisis tidak hanya berfokus pada performa model, tetapi juga pada kemungkinan adanya perbedaan performa antar kelompok.

## Tujuan

Tujuan utama proyek ini adalah:

1. Membangun model *machine learning* untuk memprediksi status kemiskinan rumah tangga.
2. Melakukan proses pengolahan dan analisis data sebelum pemodelan.
3. Mengevaluasi performa model menggunakan beberapa metrik klasifikasi.
4. Menganalisis performa model pada kelompok yang berbeda.
5. Melakukan *fairness audit* untuk mengidentifikasi potensi ketidakadilan pada hasil prediksi.
6. Memberikan interpretasi terhadap hasil model dan temuan audit keadilan.

## Dataset

Dataset yang digunakan berisi informasi mengenai karakteristik rumah tangga yang dapat digunakan untuk mengidentifikasi status kemiskinan.

Variabel yang digunakan dalam proses analisis dapat mencakup karakteristik sosial, ekonomi, dan demografis rumah tangga.

> Catatan: Detail variabel dan sumber dataset dapat dilihat secara langsung pada notebook `SDGs_1.ipynb`.

## Metodologi

Tahapan analisis dalam proyek ini meliputi:

### 1. Data Preparation
- Memuat dataset.
- Memeriksa struktur dan karakteristik data.
- Menangani data yang tidak lengkap atau tidak sesuai.
- Melakukan transformasi data apabila diperlukan.

### 2. Exploratory Data Analysis

Dilakukan eksplorasi untuk memahami:
- Distribusi data.
- Hubungan antar variabel.
- Distribusi status kemiskinan.
- Karakteristik kelompok rumah tangga.

### 3. Pemodelan Machine Learning

Data digunakan untuk membangun model klasifikasi yang bertujuan memprediksi status kemiskinan rumah tangga.

Data dibagi menjadi data *training* dan *testing* untuk mengevaluasi kemampuan model terhadap data yang belum pernah dilihat sebelumnya.

### 4. Evaluasi Model

Performa model dievaluasi menggunakan metrik klasifikasi seperti:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 5. Fairness Audit

Selain evaluasi performa secara keseluruhan, dilakukan analisis terhadap performa model berdasarkan kelompok tertentu.

Audit ini bertujuan untuk melihat apakah terdapat perbedaan hasil prediksi atau performa model antar kelompok.

Beberapa indikator yang dapat digunakan dalam analisis fairness meliputi:

- Perbedaan tingkat *false positive*.
- Perbedaan tingkat *false negative*.
- Perbedaan *recall* antar kelompok.
- Perbedaan *precision* antar kelompok.

Hasil audit digunakan untuk mengidentifikasi potensi bias dan ketidakadilan dalam sistem prediksi.

## Hasil yang Diharapkan

Proyek ini diharapkan dapat menghasilkan:

- Model yang mampu melakukan prediksi status kemiskinan dengan performa yang baik.
- Evaluasi performa model secara menyeluruh.
- Analisis perbedaan performa antar kelompok.
- Identifikasi potensi bias pada model.
- Pemahaman mengenai pentingnya aspek fairness dalam penerapan machine learning pada masalah sosial.

## Teknologi yang Digunakan

Proyek ini menggunakan:

- Python
- Google Colab
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

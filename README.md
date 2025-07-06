# Klasifikasi Bunga Iris: Analisis Perbandingan Algoritma Machine Learning

## 📖 Ringkasan Proyek

Proyek ini menyajikan analisis dan perbandingan komprehensif dari tiga algoritma klasifikasi machine learning populer—**Decision Tree**, **K-Nearest Neighbors (KNN)**, dan **Support Vector Machine (SVM)**—menggunakan dataset bunga Iris yang terkenal. Tujuan utamanya adalah untuk mengevaluasi performa setiap model dalam mengklasifikasikan spesies bunga Iris secara akurat berdasarkan ukuran sepal (kelopak) dan petal (mahkota bunga).

Aplikasi ini akan memuat dataset, melakukan pra-pemrosesan data, melatih setiap model, dan kemudian mengevaluasi kinerjanya menggunakan metrik standar serta visualisasi yang mendalam.

---

## ✨ Fitur Utama

- **Pemuatan & Pra-pemrosesan Data**: Memuat dataset Iris dari file CSV dan menyiapkannya untuk pemodelan dengan menangani fitur serta melakukan *encoding* pada variabel target.
- **Pembagian Data**: Membagi dataset menjadi set pelatihan (*training set*) dan set pengujian (*testing set*) untuk memastikan evaluasi yang objektif.
- **Standardisasi Fitur**: Menyamakan skala fitur menggunakan `StandardScaler` untuk meningkatkan performa model, terutama untuk algoritma berbasis jarak seperti KNN dan SVM.
- **Pelatihan Model**: Mengimplementasikan dan melatih tiga model klasifikasi yang berbeda:
  - Decision Tree Classifier
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (SVM) dengan kernel linear
- **Evaluasi Performa**: Menilai akurasi setiap model dan menyajikan laporan klasifikasi terperinci yang mencakup *precision*, *recall*, dan *F1-score* untuk setiap spesies.
- **Visualisasi Data**: Menghasilkan beberapa plot untuk membantu memahami struktur data dan kinerja model:
  - **Pairplot**: Memvisualisasikan hubungan antar fitur dan pemisahan antar kelas.
  - **Perbandingan Akurasi**: Diagram batang untuk membandingkan skor akurasi dari berbagai model dengan mudah.
  - **Matriks Konfusi**: *Heatmap* untuk menunjukkan akurasi dan kesalahan klasifikasi untuk setiap model dan kelas.

---

## 📊 Dataset

Dataset yang digunakan adalah **Bunga Iris**, berisi 150 sampel dari tiga spesies: `Iris-setosa`, `Iris-versicolor`, dan `Iris-virginica`.

Empat fitur yang diukur dari setiap sampel:

1. Panjang Sepal (cm)
2. Lebar Sepal (cm)
3. Panjang Petal (cm)
4. Lebar Petal (cm)

---

### 📈 Hasil Analisis

| Model | Akurasi | Presisi (Rata-rata) | Recall (Rata-rata) | F1-Score (Rata-rata) |
| :--- | :---: | :---: | :---: | :---: |
| **Decision Tree** | **1.00** | 1.00 | 1.00 | 1.00 |
| **KNN** | **1.00** | 1.00 | 1.00 | 1.00 |
| **SVM** | 0.98 | 0.98 | 0.97 | 0.97 |

-   **Decision Tree & KNN**: Mencapai akurasi sempurna **100%**, tanpa kesalahan klasifikasi pada data uji.
-   **SVM**: Mencapai akurasi **98%**, dengan hanya satu kesalahan klasifikasi antara `Iris-versicolor` dan `Iris-virginica`.

---

### 🎨 Visualisasi

Visualisasi utama yang dihasilkan dalam analisis ini adalah:

* **Pairplot Fitur**: Menunjukkan bahwa spesies `Iris-setosa` sangat mudah dipisahkan, sementara ada sedikit tumpang tindih antara dua spesies lainnya.
* **Diagram Batang Perbandingan Akurasi**: Menampilkan perbandingan kinerja secara visual, di mana Decision Tree dan KNN mencapai skor tertinggi.
* **Matriks Konfusi**: Memberikan rincian visual tentang prediksi yang benar dan yang salah untuk setiap model.

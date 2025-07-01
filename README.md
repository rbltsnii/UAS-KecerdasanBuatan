# Klasifikasi Hoodie dan Sweater Menggunakan Convolutional Neural Network (CNN)

## 📌 Deskripsi
Proyek ini merupakan implementasi **Kecerdasan Buatan (Artificial Intelligence)** untuk mengklasifikasikan produk fashion — khususnya hoodie dan sweater — secara otomatis menggunakan algoritma **Convolutional Neural Network (CNN)**. Model ini dikembangkan untuk membantu platform e-commerce dan retailer fashion dalam mengelola katalog produk dengan lebih efisien.

## 👥 Anggota Kelompok
- Ruby Ardha Apriadi – 2306138  
- Rabiul Tsani Ghifarulhaq A – 2306141

## 🎓 Dosen Pengampu
**Leni Fitriani, S.Kom, M.Kom**

## 📈 Business Understanding
- **Permasalahan:** Hoodie dan sweater sering kali memiliki kemiripan visual sehingga sulit dibedakan secara manual. Hal ini menimbulkan risiko salah kategorisasi produk di e-commerce.
- **Tujuan:** Membuat model klasifikasi otomatis dengan akurasi minimal 90%.
- **User:** Platform e-commerce, retailer fashion, sistem rekomendasi, developer.
- **Manfaat AI:**  
  - Efisiensi labeling manual hingga 80%  
  - Klasifikasi yang konsisten dan akurat  
  - Skalabilitas memproses ribuan gambar  
  - Meningkatkan pengalaman pengguna.

## 📂 Data Understanding
- **Sumber Data:** Gambar hoodie dan sweater dari marketplace populer.
- **Jumlah Data:** 1.090 gambar (512 hoodie, 578 sweater).
- **Format Data:** Gambar RGB (.jpeg/.png), resolusi 150x150x3 pixels.
- **Target:** Klasifikasi biner (0: hoodie, 1: sweater).

## 🔍 Exploratory Data Analysis (EDA)
- Dataset relatif seimbang (53% sweater, 47% hoodie).
- Variasi warna, style, angle, dan background.
- Deteksi duplikasi dan kualitas gambar dilakukan secara manual.
- Distribusi rasio kelas diperhatikan agar training tidak bias.

## ⚙️ Data Preparation
- Pemeriksaan kualitas dan filtering gambar.
- Menghapus gambar duplikat.
- Normalisasi pixel ke rentang [0,1].
- Resize gambar ke 150x150 piksel.
- Split data: 80% training, 20% validation (stratified).

## 🧠 Modeling
- **Algoritma Utama:** Convolutional Neural Network (CNN).
  - Mendeteksi fitur visual seperti tepi, sudut, tekstur.
  - Cocok untuk data gambar dengan variasi visual tinggi.
- **Baseline:** Logistic Regression (untuk pembanding awal).
- **Implementasi:** Python + TensorFlow/Keras.
- **Hyperparameter Tuning:** Grid Search untuk Logistic Regression.

## ✅ Evaluation
- **Model Dasar (Logistic Regression):**
  - Akurasi: ~76%  
  - Confusion matrix, precision, recall, F1-score dievaluasi.
- **Model CNN:**
  - Akurasi training: 93,21%  
  - Akurasi validasi: 100%  
  - Menunjukkan performa sangat baik dalam membedakan hoodie dan sweater.

## 📌 Kesimpulan & Rekomendasi
- Model CNN terbukti efektif dengan akurasi validasi 100%.
- Tantangan:
  - Dataset masih terbatas (1.090 gambar).
  - Slight class imbalance.
  - Variasi style belum sepenuhnya tercakup.
  - Perlu GPU untuk training optimal.
- Rekomendasi:
  - Tambah data dengan variasi style lebih banyak.
  - Gunakan augmentasi data untuk variasi sudut & background.
  - Eksplorasi arsitektur CNN lain untuk hasil lebih baik.

## 📚 Referensi
- Ashari, A., et al. (2019). *Perbandingan Kinerja K-Means Dengan DBSCAN Untuk Clustering Data Penjualan Online Retail*.
- Hidayat, F. (2023). *Implementasi Klasifikasi Gambar Untuk Industri Pakaian*.
- Putri, F. G., et al. (2022). *Penerapan Metode CNN Untuk Clothing Image Recognition*.
- Susilayasa, I. M. A., et al. (2022). *Analisis Sentimen Ulasan E-Commerce Pakaian dengan CNN*.
- Sandag, G. A., et al. (2021). *Identifikasi Foto Fashion dengan CNN*.

## 📂 Lampiran
- Google Colab link: [Klik di sini](https://drive.google.com/drive/folders/1BQGb9HO28L8xQjlbc3qbU3OimROfzWVN?usp=sharing)

🌿 Sistem Prediksi Harga Jual dan Kualitas Rotan Kabupaten Sigi
Analisis data rotan menggunakan Linear Regression dan Support Vector Machine (SVM) untuk memperkirakan harga jual serta mengklasifikasikan kualitas rotan berdasarkan karakteristik fisik dan proses pengolahan.

📌 Deskripsi Proyek
Proyek ini dikembangkan untuk membantu melakukan analisis terhadap kualitas dan nilai jual rotan di Kabupaten Sigi. Data yang digunakan memuat berbagai atribut rotan seperti jenis, ukuran batang, kadar air, kerapatan, musim panen, lama pengeringan, serta tingkat cacat fisik.

Penelitian membandingkan dua pendekatan Machine Learning:

Tujuan	Metode
Prediksi Harga Jual	Linear Regression
Klasifikasi Kualitas	Support Vector Machine (SVC)
Dengan pendekatan ini, sistem dapat memberikan estimasi harga jual dan menentukan grade kualitas rotan secara otomatis berdasarkan karakteristik yang dimasukkan.

🔄 Alur Sistem
Dataset Rotan
      │
      ▼
Preprocessing Data
(Label Encoding)
      │
      ▼
Pembagian Data
(Training & Testing)
      │
 ┌───────────────┬───────────────┐
 ▼                               ▼
Linear Regression           SVM (SVC)
Prediksi Harga              Klasifikasi Grade
      │                               │
      └───────────────┬───────────────┘
                      ▼
              Evaluasi Model
📊 Variabel Dataset
Variabel Input
Jenis Rotan
Panjang Batang (m)
Diameter Batang (mm)
Kerapatan (g/cm³)
Kadar Air (%)
Musim Panen
Lama Pengeringan (hari)
Cacat Fisik (%)
Variabel Output
Regresi
Harga Jual (Rp/kg)
Klasifikasi
Grade Kualitas (A, B, C)
📈 Tahapan Analisis
1. Data Preparation
Dataset dibersihkan dan dikonversi ke format numerik menggunakan Label Encoding agar dapat diproses oleh algoritma Machine Learning.

2. Prediksi Harga Jual
Metode Linear Regression digunakan untuk mempelajari hubungan antara karakteristik rotan dengan harga jualnya.

Model menghasilkan:

MAE (Mean Absolute Error)
RMSE (Root Mean Square Error)
R² Score
3. Klasifikasi Kualitas
Support Vector Machine (SVC) digunakan untuk mengelompokkan kualitas rotan ke dalam kategori tertentu berdasarkan atribut fisik dan hasil pengolahan.

Evaluasi dilakukan menggunakan:

Accuracy
Confusion Matrix
📁 Struktur Proyek
📦 Prediksi-Rotan-Sigi
│
├── statistika.py
│
├── Laporan_Rotan_Sigi.xlsx
│
├── output/
│   ├── grafik_regresi.png
│   ├── confusion_matrix.png
│   └── hasil_prediksi.csv
│
├── hasil/
│   ├── evaluasi_regresi.csv
│   ├── evaluasi_svm.csv
│   └── data_prediksi_baru.csv
│
└── README.md
⚙️ Cara Menjalankan Program
1. Install Library
pip install pandas
pip install numpy
pip install matplotlib
pip install scikit-learn
pip install openpyxl
atau

pip install pandas numpy matplotlib scikit-learn openpyxl
2. Siapkan Dataset
Letakkan file:

Laporan_Rotan_Sigi.xlsx
pada folder yang sama dengan file program Python.

3. Jalankan Program
python statistika.py
🔧 Library yang Digunakan
Library	Fungsi
pandas	Membaca dan mengolah data
numpy	Operasi numerik
matplotlib	Visualisasi grafik
scikit-learn	Algoritma Machine Learning
openpyxl	Membaca file Excel
🧠 Penjelasan Metode
Linear Regression
Linear Regression digunakan untuk memperkirakan harga jual rotan berdasarkan hubungan antara variabel input dan target harga.

Persamaan umum:

Y = a + bX
Metode ini cocok digunakan untuk memprediksi nilai kontinu seperti harga.

Support Vector Machine (SVC)
Support Vector Machine bekerja dengan mencari batas pemisah terbaik antar kelas kualitas rotan.

Output yang dihasilkan berupa kategori kualitas seperti:

Grade A
Grade B
Grade C
Metode ini dikenal memiliki kemampuan klasifikasi yang baik pada data yang memiliki banyak atribut.

📊 Output Program
Program akan menghasilkan:

Hasil Regresi
MAE  : xxxx
RMSE : xxxx
R2   : xxxx
Hasil Klasifikasi
Akurasi : xx.xx %
Prediksi Data Baru
Harga Jual Prediksi : Rp xxxxx
Grade Kualitas      : A
🎯 Tujuan Penelitian
Menganalisis faktor-faktor yang mempengaruhi harga jual rotan.
Mengidentifikasi kualitas rotan berdasarkan karakteristik fisiknya.
Membandingkan efektivitas metode regresi dan klasifikasi dalam pengolahan data rotan.
Membangun sistem pendukung keputusan berbasis Machine Learning untuk komoditas rotan.
👤 Informasi Proyek
Judul:

Prediksi Harga Jual dan Klasifikasi Kualitas Rotan Menggunakan Linear Regression dan Support Vector Machine pada Data Rotan Kabupaten Sigi

Institusi:

Universitas Tadulako

Program Studi:

Teknik Informatika

📜 Lisensi
Proyek ini dibuat untuk kebutuhan akademik dan pembelajaran. Dataset digunakan sebagai bahan penelitian dan pengembangan sistem prediksi berbasis Machine Learning.

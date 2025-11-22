# water-quality-classification-knn
A Machine Learning model to detect potable water based on chemical properties using Python.

# Klasifikasi Kualitas Air Minum dengan K-NN

Proyek Machine Learning ini dibuat untuk memprediksi apakah air yang diminum aman dikonsumsi atau tidak berdasarkan kandungan kimianya.

## Latar Belakang
Pengecekan kualitas air secara manual di laboratorium membutuhkan waktu dan biaya. Jadi, saya mencoba buat program komputer yang dapat menebak kualitas air secara otomatis menggunakan data kimia.

## Algoritma
Saya pakai metode **K-Nearest Neighbors (K-NN)**.

Gampangnya, algoritma ini bekerja dengan cara "mencari kemiripan". Jika ada sampel air baru, komputer akan mengecek data air lain yang kandungan kimianya serupa. Kalau mayoritas tetangganya aman, berarti air baru itu kemungkinan besar aman juga.


## Tahapan Pengerjaan
1.  **Data Cleaning:** Menangani data yang kosong agar proses berjalan lancar.
2.  **Feature Scaling:** Menyamakan skala angka antar variabel (misalnya pH vs Zat Padat) agar perhitungan jarak K-NN akurat.
3.  **Mencari K Terbaik:** Menggunakan *Elbow Method* untuk menguji nilai K dari 1 hingga 30. Ditemukan bahwa **K=23** memberikan tingkat error terendah.
4.  **Evaluasi:** Menguji performa model dalam mendeteksi air yang tidak layak minum.

## Dataset
Data diambil dari Kaggle: *Water Potability Dataset*.
Fitur yang digunakan meliputi pH air, tingkat kekeruhan, zat padat terlarut, dan parameter kimia lainnya.

## Cara Menjalankan
1.  Clone repository ini.
2.  Pastikan Python dan library berikut sudah terinstall: `pandas`, `numpy`, `sklearn`.
3.  Buka dan jalankan file notebook (`.ipynb`).

---
*Dibuat untuk keperluan portofolio Data Science.*

# Tugas 1: Implementasi K-Means Clustering (Modul GPS Trajectories)

Repository ini berisi pengerjaan modul praktikum K-Means Clustering menggunakan dataset GPS Trajectories.

## 📌 Deskripsi
Mengelompokan data perjalanan berdasarkan jarak (`distance`) dan kecepatan (`speed`) menggunakan algoritma K-Means.

## 📊 Dataset
- **Nama**: GPS Trajectories (Go!Track)
- **Sumber**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/354/gps+trajectories)
- **File**: `go_track_tracks.csv`

## 📝 Langkah Pengerjaan (Sesuai Modul)
1. Load library yang diperlukan (pandas, numpy, sklearn, matplotlib, seaborn).
2. Load dataset dan menampilkan info data.
3. Menghapus kolom yang tidak digunakan (`linha`).
4. Menentukan variabel yang akan diklusterkan (`distance` dan `speed`).
5. Memvisualisasikan persebaran data awal.
6. Mengubah data frame menjadi array.
7. Melakukan normalisasi data menggunakan Min-Max Scaling.
8. Membuat model K-Means dengan `n_clusters=3` dan melakukan training.
9. Evaluasi model menggunakan Silhouette Score
10. Visualisasi hasil clustering beserta penanda centroid.

## ⚠️ Catatan Perbaikan dari Kode Modul
- Penambahan `n_init=10` pada `KMeans()` untuk mencegah *FutureWarning* dari sklearn.
- Mengganti `kmeans.fit(baca)` menjadi `kmeans.fit(x_scaled)` agar kode tidak error (dataframe baca mengandung tipe data string).
- Memperbaiki indeks dan label pada visualisasi akhir, karena kode asli modul merupakan salah ketik dari analisis RFM.

## 🚀 Cara Menjalankan
1. Clone repository ini
2. Letakkan file `go_track_tracks.csv` di folder yang sama
3. Jalankan file `modul_kmeans.py` atau `modul_kmeans.ipynb`
EOF

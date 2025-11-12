# EDA-KNIME-WORKFLOW

# 📊 EDA (Exploratory) KNIME Workflow

*Workflow* KNIME ini dirancang untuk melakukan Analisis Data Eksploratif (EDA) pada dataset untuk memahami karakteristik, distribusi, dan hubungan antarvariabel sebelum melangkah ke pemodelan yang lebih kompleks.

## 🛠️ Komponen Workflow

*Workflow* ini menggunakan serangkaian node standar KNIME untuk pemrosesan data, visualisasi, dan analisis statistik:

### 1. Pemrosesan Data Awal
* [cite_start]**CSV Reader (#1):** Node ini digunakan untuk membaca data awal dari file CSV ke dalam *workflow*[cite: 3].
* [cite_start]**Missing Value (#2):** Node ini digunakan untuk menangani nilai yang hilang dalam dataset (data *cleaning*)[cite: 6].

### 2. Analisis Hubungan
* [cite_start]**Linear Correlation (#3):** Node ini menghitung dan menampilkan korelasi linier antar kolom numerik dalam dataset[cite: 6].
* [cite_start]**Heatmap (#10):** Node ini memvisualisasikan matriks korelasi atau data lain dalam bentuk *heatmap* untuk melihat pola hubungan dengan cepat[cite: 5].
* [cite_start]**Scatter Plot Matrix (#5):** Node ini membuat plot sebar berpasangan (scatter plot matrix) untuk memvisualisasikan hubungan antara setiap pasangan variabel[cite: 6].

### 3. Analisis Distribusi & Statistik
* [cite_start]**Statistics (#11) / Statistics View (#12):** Node ini digunakan untuk menghitung ringkasan statistik deskriptif (seperti mean, median, standar deviasi, dll.) untuk kolom dalam dataset[cite: 6, 7].
* [cite_start]**Histogram (#6):** Node ini memvisualisasikan distribusi variabel numerik menggunakan histogram[cite: 6].
* [cite_start]**Box Plot (#4):** Node ini membuat *box plot* untuk memvisualisasikan ringkasan statistik lima angka (minimum, kuartil pertama, median, kuartil ketiga, maksimum) dan mengidentifikasi *outlier*[cite: 3].
* [cite_start]**Auto Binner (#8) & (#9):** Node ini secara otomatis mengelompokkan (binning) kolom data numerik ke dalam kategori atau interval[cite: 1, 2].

## ⚙️ Cara Menggunakan Workflow

1.  **Impor Data:** Pastikan data input Anda berupa file CSV dan konfigurasikan node **CSV Reader (#1)** dengan jalur file yang benar.
2.  **Jalankan Workflow:** Jalankan seluruh *workflow* atau setiap node secara berurutan.
3.  **Inspeksi Hasil:**
    * Klik kanan pada node visualisasi (seperti **Box Plot**, **Histogram**, **Heatmap**, **Scatter Plot Matrix**) dan pilih **View: ...** untuk melihat plot.
    * Klik kanan pada node **Statistics View (#12)** untuk melihat ringkasan statistik deskriptif dari data yang telah diproses.

# Klasifikasi Tingkat Risiko Obesitas Berdasarkan Kebiasaan Makan dan Aktivitas Fisik

## Ringkasan Proyek

Proyek ini bertujuan untuk mengklasifikasikan tingkat risiko obesitas berdasarkan kebiasaan makan, aktivitas fisik, dan karakteristik individu menggunakan pendekatan Data Science dan Machine Learning.

Data yang digunakan mencakup berbagai variabel, seperti usia, jenis kelamin, riwayat keluarga, kebiasaan mengonsumsi makanan tinggi kalori, frekuensi konsumsi sayuran, jumlah makan utama, kebiasaan mengonsumsi makanan ringan, konsumsi air, serta frekuensi aktivitas fisik.

Melalui proses analisis data dan pemodelan Machine Learning, proyek ini berupaya mengidentifikasi pola kebiasaan hidup yang berkaitan dengan kategori status berat badan dan obesitas.

Klasifikasi dilakukan ke dalam tujuh kategori, yaitu:
1. Insufficient Weight
2. Normal Weight
3. Overweight Level I
4. Overweight Level II
5. Obesity Type I
6. Obesity Type II
7. Obesity Type III

Proyek klasifikasi **7 kategori status berat badan/obesitas** dengan pendekatan data science. Notebook memuat Business Understanding, Data Gathering, EDA, Cleaning, Preprocessing, Feature Selection, Modelling, Evaluasi, dan Konklusi. Proyek ini **bukan alat diagnosis medis**; tidak diperlukan aplikasi web atau deployment.

**Catatan:** Hasil klasifikasi merupakan analisis berbasis dataset dan bukan diagnosis atau penilaian risiko medis secara langsung.

## 2. Informasi Anggota Kelompok

1. **Nomor Kelompok:** 55
2. **Nama Kelompok:** kaum deadline
3. **Nama Seluruh Anggota Kelompok:**

| No. | Nama | NIM | Kontribusi |
|---|---|---|---|
| 1 | Hasan | 123240041 | [Isi kontribusi anggota] |
| 2 | Nurjelita Sukmawati | 123240046 | [Isi kontribusi anggota] |
| 3 | Haerunisa | 123240047 | [Isi kontribusi anggota] |
| 4 | Puput Septiani | 123240263 | [Isi kontribusi anggota] |

**Catatan:** Bagian kontribusi perlu disesuaikan dengan pembagian tugas dan pekerjaan yang benar-benar dilakukan oleh masing-masing anggota.

## 3. Sumber Data

Dataset yang digunakan dalam proyek ini adalah **Estimation of Obesity Levels Based on Eating Habits and Physical Condition**.

Dataset diperoleh dari UCI Machine Learning Repository dan menggunakan salinan dataset yang tersedia di Kaggle sebagai referensi.

- Sumber resmi UCI: https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition
- Sumber Kaggle: https://www.kaggle.com/datasets/ruchikakumbhar/obesity-prediction

### Informasi Dataset

- Jumlah data: 2.111 baris.
- Jumlah kolom: 17 kolom.
- Jumlah fitur: 16 fitur.
- Variabel target: Obesity.
- Jenis permasalahan: Multiclass Classification.
- Jumlah kategori target: 7 kelas.

### Fitur Dataset

Beberapa variabel yang digunakan dalam dataset antara lain:

| Variabel | Keterangan |
|---|---|
| Gender | Jenis kelamin individu |
| Age | Usia individu |
| Height | Tinggi badan |
| Weight | Berat badan |
| family_history | Riwayat keluarga dengan kelebihan berat badan |
| FAVC | Kebiasaan mengonsumsi makanan tinggi kalori |
| FCVC | Frekuensi konsumsi sayuran |
| NCP | Jumlah makanan utama per hari |
| CAEC | Kebiasaan mengonsumsi makanan di antara waktu makan |
| SMOKE | Kebiasaan merokok |
| CH2O | Tingkat konsumsi air |
| SCC | Kebiasaan memantau konsumsi kalori |
| FAF | Frekuensi aktivitas fisik |
| TUE | Waktu penggunaan perangkat teknologi |
| CALC | Frekuensi konsumsi alkohol |
| MTRANS | Moda transportasi yang digunakan |
| Obesity | Kategori status obesitas sebagai variabel target |

## 4. Struktur Repository

Struktur folder proyek disusun sebagai berikut:

```text
ObesityPrediction/
│
├── README.md
│
├── data/
│   └── Obesity_prediction.csv
│
└── notebooks/
    └── DataScience_ObesityPrediction_ProyekAkhir.ipynb

```

Keterangan:

- `README.md`: Dokumentasi dan panduan proyek.
- `data/`: Folder penyimpanan dataset.
- `notebooks/`: Folder notebook yang berisi proses analisis dan pemodelan.

## 5. Panduan Menjalankan Proyek

Proyek ini dijalankan menggunakan Visual Studio Code (VS Code), Python, dan Jupyter Notebook.

### A. Persiapan

Pastikan aplikasi berikut sudah terinstal:

1. Python 3: https://www.python.org/downloads/
2. Visual Studio Code: https://code.visualstudio.com/
3. Git: https://git-scm.com/downloads/

Pada saat instalasi Python di Windows, pastikan opsi **Add Python to PATH** dicentang.

### B. Membuka Repository

1. Unduh atau clone repository proyek dari GitHub.
2. Ekstrak folder proyek jika menggunakan file ZIP.
3. Buka Visual Studio Code.
4. Pilih menu **File → Open Folder**.
5. Pilih folder utama proyek.

### C. Membuat Virtual Environment

Buka terminal di VS Code melalui menu **Terminal → New Terminal**.

Jalankan perintah:

```bash
python -m venv .venv
```

Aktifkan virtual environment pada Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

Jika menggunakan Command Prompt:

```cmd
.venv\Scripts\activate.bat
```

### D. Menginstal Library

Setelah virtual environment aktif, jalankan:

```bash
python -m pip install --upgrade pip
```

Kemudian instal seluruh library yang dibutuhkan:

```bash
pip install -r requirements.txt
```

### E. Memasang Extension VS Code

Buka menu Extensions di VS Code, kemudian instal:

- Python (Microsoft)
- Jupyter (Microsoft)

Extension tersebut digunakan untuk menjalankan notebook Python secara langsung di VS Code.

### F. Membuka dan Menjalankan Notebook

1. *Clone* atau unduh repository yang sudah berisi `Obesity_prediction.csv`, lalu tempatkan notebook pada folder `notebooks/`.
2. Instal Python serta Jupyter/VS Code Python dan Jupyter extension.
3. Jalankan perintah `python -m pip install -r requirements.txt` di root repository.
4. Buka notebook dan pilih **Run All**.
5. Tunggu hingga seluruh proses analisis dan pemodelan selesai.
6. Pastikan tabel, grafik, model, dan kesimpulan muncul dari CSV asli; simpan notebook **beserta hasil eksekusi** sebelum pengumpulan.
7. Jika CSV tidak ditemukan, notebook mencoba pembacaan dari GitHub (memerlukan internet). Notebook menolak berkas yang ukurannya bukan 2.111 × 17.

### G. Memastikan Dataset Terbaca

Pastikan file dataset berada pada folder `data` dengan nama:

```text
Obesity_prediction.csv
```

Karena notebook berada di dalam folder `notebooks`, lokasi relatif dataset yang digunakan adalah:

```python
../data/Obesity_prediction.csv
```

Jika terjadi kesalahan saat membaca dataset, periksa kembali nama file dan struktur folder repository.

### H. Menyimpan Hasil

Setelah seluruh cell berhasil dijalankan:

1. Pastikan tidak terdapat error.
2. Periksa hasil analisis, visualisasi, dan evaluasi model.
3. Simpan notebook menggunakan `Ctrl + S`.
4. Pastikan seluruh output notebook tersimpan.

## 6. Teknologi dan Library yang Digunakan

Proyek ini menggunakan beberapa teknologi dan library berikut:

| Teknologi / Library | Kegunaan |
|---|---|
| Python | Bahasa pemrograman utama |
| Pandas | Pengolahan dan analisis data |
| NumPy | Operasi numerik |
| Matplotlib | Visualisasi data |
| Seaborn | Visualisasi statistik |
| Scikit-learn | Preprocessing, pemodelan, dan evaluasi Machine Learning |
| Jupyter Notebook | Menjalankan dan mendokumentasikan proses analisis |
| Visual Studio Code | Lingkungan pengembangan proyek |
| Git & GitHub | Pengelolaan versi dan penyimpanan repository |

## 7. Metodologi Proyek

Proyek ini menggunakan pendekatan *Machine Learning* dengan metode klasifikasi multikelas untuk mengidentifikasi kategori tingkat obesitas berdasarkan karakteristik individu dan kebiasaan hidup. Proses pengerjaan mengikuti tahapan Data Science sebagai berikut:

1. **Business Understanding**

   Mengidentifikasi permasalahan klasifikasi tingkat obesitas, menentukan tujuan analisis, merumuskan pertanyaan penelitian, serta menetapkan metode dan metrik evaluasi yang digunakan.

2. **Data Gathering**

   Mengumpulkan dan memahami dataset obesitas yang bersumber dari UCI Machine Learning Repository, meliputi jumlah data, karakteristik variabel, deskripsi setiap fitur, serta informasi mengenai sumber dan kualitas dataset.

3. **Exploratory Data Analysis (EDA)**

   Melakukan analisis statistik deskriptif dan visualisasi data untuk mengetahui distribusi kategori obesitas, karakteristik individu, serta pola hubungan antara kebiasaan hidup dan tingkat obesitas. Setiap visualisasi disertai interpretasi berdasarkan hasil analisis.

4. **Cleaning dan Preprocessing**

   Memeriksa missing value, data duplikat, outlier, dan ketidaksesuaian tipe data. Selanjutnya dilakukan penanganan data sesuai kebutuhan, termasuk transformasi variabel kategorikal dan standardisasi fitur numerik. Tahapan ini juga mencakup Feature Selection untuk menentukan fitur yang relevan berdasarkan tujuan analisis.

5. **Modelling**

   Membangun model klasifikasi menggunakan Logistic Regression dan Random Forest, serta Dummy Classifier sebagai baseline pembanding. Proses pemodelan menggunakan pembagian data latih dan data uji serta validasi silang untuk membantu menilai kemampuan generalisasi model.

6. **Evaluasi**

   Mengevaluasi performa model menggunakan Accuracy, Precision, Recall, F1-score, dan Confusion Matrix. Hasil evaluasi digunakan untuk membandingkan kemampuan model dalam mengklasifikasikan tujuh kategori obesitas serta menentukan model terbaik berdasarkan metrik dan tujuan analisis.

7. **Konklusi**

   Menyimpulkan hasil analisis berdasarkan pertanyaan pada tahap Business Understanding, menjelaskan makna hasil evaluasi, menentukan model yang paling sesuai, serta mengidentifikasi keterbatasan dataset dan metode penelitian.

## 8. Hasil yang Diharapkan

Hasil yang diharapkan dari proyek ini adalah diperolehnya pemahaman mengenai karakteristik individu dan kebiasaan hidup yang berkaitan dengan kategori tingkat obesitas.

Melalui proses Exploratory Data Analysis (EDA), proyek ini diharapkan dapat memberikan gambaran mengenai distribusi kategori obesitas dan pola yang terdapat pada dataset.

Selanjutnya, proyek ini diharapkan menghasilkan model Machine Learning yang mampu melakukan klasifikasi tingkat obesitas berdasarkan fitur yang tersedia. Perbandingan beberapa model dilakukan untuk mengetahui perbedaan performa dan menentukan model yang paling sesuai berdasarkan hasil evaluasi.

Selain itu, proyek ini diharapkan dapat memberikan penjelasan mengenai kontribusi fitur terhadap proses klasifikasi, kesalahan prediksi yang terjadi, dan keterbatasan model.

Hasil akhir proyek disajikan dalam Jupyter Notebook yang memuat seluruh tahapan analisis, kode program, visualisasi, hasil evaluasi, interpretasi, serta kesimpulan yang dapat dipertanggungjawabkan secara akademis.

---

**Program Studi Informatika**  
**Jurusan Informatika**  
**Fakultas Teknik Industri**  
**Universitas Pembangunan Nasional "Veteran" Yogyakarta**  
**2026**

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

Tahapan proyek meliputi Business Understanding, Data Understanding, Data Preparation, Exploratory Data Analysis (EDA), Modeling, Evaluation, dan Conclusion.

Hasil proyek diharapkan dapat memberikan gambaran mengenai pola kebiasaan makan dan aktivitas fisik pada berbagai kategori status obesitas serta menunjukkan kemampuan Machine Learning dalam melakukan klasifikasi berdasarkan variabel yang tersedia.

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
- `requirements.txt`: Daftar library Python yang dibutuhkan.
- `data/`: Folder penyimpanan dataset.
- `notebooks/`: Folder notebook yang berisi proses analisis dan pemodelan.
- `laporan/`: Folder dokumen laporan proyek.

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

1. Buka folder `notebooks`.
2. Pilih file `UTS_DataScience_ObesityPrediction_ProyekAkhir.ipynb`.
3. Klik **Select Kernel** pada bagian kanan atas notebook.
4. Pilih interpreter Python dari virtual environment `.venv`.
5. Jalankan setiap cell secara berurutan atau pilih **Run All**.
6. Tunggu hingga seluruh proses analisis dan pemodelan selesai.

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

Proses pengerjaan proyek mengikuti tahapan Data Science sebagai berikut:

1. **Business Understanding**  
   Menentukan tujuan dan permasalahan yang ingin diselesaikan melalui analisis data obesitas.

2. **Data Understanding**  
   Memahami karakteristik dataset, jumlah data, tipe variabel, distribusi kelas, dan kondisi data.

3. **Data Preparation**  
   Melakukan pemeriksaan data, penanganan data duplikat, serta preprocessing sesuai kebutuhan pemodelan.

4. **Exploratory Data Analysis (EDA)**  
   Melakukan eksplorasi dan visualisasi untuk mengetahui pola kebiasaan hidup dan karakteristik individu pada setiap kategori obesitas.

5. **Modeling**  
   Membangun model Machine Learning untuk melakukan klasifikasi kategori status obesitas.

6. **Evaluation**  
   Mengevaluasi performa model menggunakan metrik seperti Accuracy, Precision, Recall, F1-Score, dan Confusion Matrix.

7. **Conclusion**  
   Menyimpulkan hasil analisis dan evaluasi model berdasarkan proses yang telah dilakukan.

## 8. Catatan dan Batasan Proyek

- Dataset yang digunakan tidak secara khusus merepresentasikan seluruh populasi Indonesia.
- Hasil klasifikasi dipengaruhi oleh karakteristik dan distribusi data yang digunakan.
- Tinggi badan dan berat badan dapat digunakan dalam eksplorasi data, tetapi perlu dikeluarkan dari fitur pemodelan apabila kategori target dibentuk berdasarkan BMI, untuk menghindari target leakage.
- Model yang dihasilkan hanya digunakan untuk kebutuhan pembelajaran dan analisis data, bukan sebagai pengganti pemeriksaan atau diagnosis tenaga kesehatan.

---

**Program Studi Informatika**  
**Jurusan Informatika**  
**Fakultas Teknik Industri**  
**Universitas Pembangunan Nasional "Veteran" Yogyakarta**  
**2026**

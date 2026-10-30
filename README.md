# Analisis Pola Kebiasaan Hidup dan Karakteristik Individu pada Berbagai Kategori Status Obesitas

## 1. Ringkasan Proyek

Proyek ini menerapkan tahapan Data Science untuk menganalisis pola kebiasaan hidup dan karakteristik individu pada berbagai kategori status obesitas. Dataset memuat informasi demografis, kebiasaan makan, konsumsi air, aktivitas fisik, penggunaan perangkat teknologi, moda transportasi, serta label kategori status obesitas.

Tujuan proyek:
- Memahami karakteristik dan kualitas dataset.
- Melakukan Exploratory Data Analysis (EDA) untuk menemukan pola dan insight.
- Membersihkan serta mempersiapkan data untuk pemodelan.
- Membangun dan membandingkan model klasifikasi untuk tujuh kategori pada kolom target `Obesity`.
- Mengevaluasi performa model dan menginterpretasikan hasil secara kritis.

Proyek ini bersifat akademik. Hasil klasifikasi **bukan alat diagnosis medis**, tidak membuktikan hubungan sebab-akibat, dan bukan pengganti pemeriksaan tenaga kesehatan.

## 2. Informasi Anggota dan Kontribusi

## Informasi Kelompok

1. **Nomor Kelompok:** 55
2. **Nama Kelompok:** kaum deadline
3. **Nama Seluruh Anggota Kelompok:**

| No. | Nama | NIM | Kontribusi |
|---|---|---|---|
| 1 | Hasan | 123240041 | *Isi kontribusi aktual anggota*  |
| 2 | Nurjelita Sukmawati | 123240046 | *Isi kontribusi aktual anggota*  |
| 3 | Haerunisa | 123240047 | *Isi kontribusi aktual anggota*  |
| 4 | Puput Septiani | 123240263 | *Isi kontribusi aktual anggota*  |

## 3. Sumber Data

Dataset yang digunakan adalah **Estimation of Obesity Levels Based on Eating Habits and Physical Condition**.

- **Sumber resmi:** UCI Machine Learning Repository  
  https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition
- **Tautan dataset yang dicantumkan dalam laporan kelompok:** Kaggle – Obesity Prediction  
  https://www.kaggle.com/datasets/ruchikakumbhar/obesityprediction
- **File lokal:** `data/Obesity_prediction.csv`
- **Ukuran dataset:** 2.111 baris dan 17 kolom (16 fitur dan 1 target), sesuai dokumentasi dataset/laporan kelompok.
- **Target klasifikasi:** `Obesity`, yang berisi tujuh kategori status berat badan.

Dataset berisi informasi responden dari Meksiko, Peru, dan Kolombia. Berdasarkan laporan acuan kelompok, dataset juga mencakup data sintetis yang dibentuk menggunakan SMOTE. Karena itu, interpretasi perlu mempertimbangkan keterbatasan representativitas dan potensi bias data sintetis.

### Data Dictionary Ringkas

| Kolom | Keterangan |
|---|---|
| `Gender` | Jenis kelamin |
| `Age` | Usia (tahun) |
| `Height` | Tinggi badan (meter) |
| `Weight` | Berat badan (kg) |
| `family_history` | Riwayat keluarga dengan overweight |
| `FAVC` | Kebiasaan mengonsumsi makanan tinggi kalori |
| `FCVC` | Frekuensi konsumsi sayur |
| `NCP` | Jumlah makan utama per hari |
| `CAEC` | Kebiasaan mengonsumsi camilan di antara waktu makan |
| `SMOKE` | Kebiasaan merokok |
| `CH2O` | Tingkat konsumsi air |
| `SCC` | Kebiasaan memantau asupan kalori |
| `FAF` | Frekuensi aktivitas fisik |
| `TUE` | Waktu penggunaan perangkat teknologi |
| `CALC` | Frekuensi konsumsi alkohol |
| `MTRANS` | Moda transportasi |
| `Obesity` | Label kategori status berat badan (target) |

## 4. Struktur Repository

```text
ObesityPrediction_Repository/
├── README.md
├── requirements.txt
├── Laporan_UTS_Acuan.pdf
├── data/
│   └── Obesity_prediction.csv
└── notebooks/
    └── UTS_DataScience_ObesityPrediction_ProyekAkhir.ipynb
```

## 5. Panduan Menjalankan Proyek

### A. Menggunakan Google Colab

1. Buka https://colab.research.google.com/.
2. Upload notebook dari folder `notebooks/`.
3. Upload `Obesity_prediction.csv` dari folder `data/` ke sesi Colab, atau hubungkan Google Drive.
4. Sesuaikan lokasi file CSV pada sel pembacaan dataset (`file_path` atau `DATA_PATH`).
5. Instal dependensi jika diperlukan:

   ```python
   !pip install pandas numpy matplotlib seaborn scikit-learn scipy
   ```

6. Jalankan semua sel notebook secara berurutan dari awal sampai akhir.
7. Periksa output, tabel, grafik, dan interpretasinya. Lengkapi bagian konklusi berdasarkan hasil aktual.

### B. Menjalankan secara lokal

1. Pastikan Python 3.10 atau versi kompatibel telah terpasang.
2. Clone repository:

   ```bash
   git clone <URL_REPOSITORY_GITHUB>
   cd ObesityPrediction_Repository
   ```

3. Buat virtual environment (opsional):

   ```bash
   python -m venv .venv
   ```

   Windows:

   ```bash
   .venv\Scripts\activate
   ```

   macOS/Linux:

   ```bash
   source .venv/bin/activate
   ```

4. Instal pustaka:

   ```bash
   pip install -r requirements.txt
   ```

5. Jalankan Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Buka notebook pada folder `notebooks/`, lalu jalankan semua sel secara berurutan.

## 6. Alur Analisis dalam Notebook

Notebook mengikuti tahapan proyek Data Science berikut:

1. **Business Understanding** — latar belakang, permasalahan, pertanyaan analisis, tujuan, metode, metrik keberhasilan, dan batasan.
2. **Data Gathering** — pemuatan dataset, sumber data, dan pemahaman variabel.
3. **EDA** — statistik deskriptif, visualisasi distribusi, hubungan fitur, dan interpretasi temuan.
4. **Cleaning dan Preprocessing** — pemeriksaan kualitas data, penanganan duplikasi/missing value bila ditemukan, transformasi data, dan feature selection.
5. **Modelling** — pelatihan dan perbandingan model klasifikasi.
6. **Evaluasi** — evaluasi menggunakan metrik klasifikasi dan visualisasi pendukung.
7. **Konklusi** — jawaban atas pertanyaan Business Understanding, interpretasi hasil, keputusan, dan keterbatasan.

## 7. Catatan Interpretasi dan Etika

- `Height` dan `Weight` dapat digunakan untuk eksplorasi deskriptif, tetapi tidak digunakan sebagai fitur prediksi apabila label target diturunkan dari IMT. Penggunaan keduanya dapat menyebabkan *target leakage*.
- Data sintetis dan duplikasi dapat memengaruhi evaluasi model. Pemisahan data dan validasi harus dilakukan dengan hati-hati.
- Periksa performa setiap kelas, bukan hanya akurasi keseluruhan.
- Periksa kemungkinan bias, termasuk perbedaan komposisi gender antar kelas.
- Korelasi dan feature importance tidak boleh ditafsirkan sebagai bukti sebab-akibat.
- Hasil model tidak dimaksudkan untuk diagnosis atau keputusan medis individual.

## 8. Lisensi dan Atribusi

Dataset dirujuk melalui UCI Machine Learning Repository dan tautan Kaggle yang dicantumkan dalam laporan kelompok. Periksa kembali ketentuan lisensi dan atribusi pada halaman sumber resmi sebelum penggunaan atau distribusi ulang dataset. Cantumkan atribusi dataset dalam laporan akademik.

---

**Program Studi Informatika**  
**Jurusan Informatika, Fakultas Teknik Industri**  
**Universitas Pembangunan Nasional “Veteran” Yogyakarta**  
**2026**

# Analisis Prediksi Promosi Karyawan

## Deskripsi Singkat
Proyek ini merupakan tugas kuliah yang berfokus pada analisis data karyawan untuk memprediksi apakah seorang karyawan berpotensi mendapatkan promosi. Proses yang dilakukan meliputi eksplorasi dataset, preprocessing data, pembangunan model, dan evaluasi performa model.

## Tujuan
Tujuan dari proyek ini adalah:
- memahami karakteristik dataset employee promotion,
- melakukan preprocessing data sebelum pemodelan,
- membangun model klasifikasi untuk prediksi promosi,
- mengevaluasi performa model menggunakan metrik yang relevan.

## Dataset
Dataset yang digunakan terdiri dari dua file utama:
- `train.csv` → data latih yang memuat fitur dan target promosi,
- `test.csv` → data uji tanpa target.

Secara umum, dataset berisi informasi seperti:
- `department`
- `region`
- `education`
- `gender`
- `recruitment_channel`
- `no_of_trainings`
- `age`
- `previous_year_rating`
- `length_of_service`
- `KPIs_met >80%`
- `awards_won?`
- `avg_training_score`
- `is_promoted` (khusus data latih)

## Struktur Project
```text
employee_promotion/
├── main.ipynb
├── train.csv
├── test.csv
└── README.md
```

## Alur Pengerjaan
### 1. Import Library
Tahap awal dilakukan dengan mengimpor library yang dibutuhkan, seperti:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

### 2. Load Dataset
Dataset dimuat dari file `train.csv` dan `test.csv` untuk dilakukan analisis lebih lanjut.

### 3. Exploratory Data Analysis (EDA)
Tahap EDA dilakukan untuk memahami kondisi data, meliputi:
- melihat jumlah baris dan kolom,
- memeriksa tipe data,
- memeriksa missing values,
- memeriksa duplikasi data,
- melihat distribusi target,
- menganalisis hubungan antar fitur.

### 4. Data Preprocessing
Tahap preprocessing dilakukan agar data siap digunakan oleh model. Langkah yang dapat dijelaskan pada bagian ini antara lain:
- menangani missing values,
- melakukan encoding pada fitur kategorikal,
- memisahkan fitur dan target,
- membagi data train dan validation,
- menyiapkan data untuk proses modeling.

### 5. Pembuatan Model
Pada tahap ini dilakukan pembangunan model klasifikasi untuk memprediksi promosi karyawan. Model yang digunakan dapat dijelaskan pada bagian ini, misalnya:
- Decision Tree
- Random Forest
- Logistic Regression
- model lain sesuai eksperimen

### 6. Evaluasi Model
Evaluasi model dilakukan menggunakan metrik yang sesuai untuk klasifikasi, misalnya:
- accuracy,
- precision,
- recall,
- F1-score,
- confusion matrix.

Karena dataset promosi biasanya tidak seimbang, evaluasi sebaiknya tidak hanya berfokus pada accuracy, tetapi juga memperhatikan precision, recall, dan F1-score.

### 7. Prediksi pada Data Test
Setelah model terbaik diperoleh, model dapat digunakan untuk memprediksi data pada `test.csv`.

## Susunan Laporan Tugas Kuliah
Berikut susunan laporan yang disarankan:

### BAB 1. Pendahuluan
Isi bagian ini dapat mencakup:
- latar belakang,
- rumusan masalah,
- tujuan penelitian / analisis,
- manfaat penelitian.

### BAB 2. Landasan Teori
Isi bagian ini dapat mencakup:
- data mining / machine learning,
- klasifikasi,
- konsep preprocessing data,
- algoritma yang digunakan,
- metrik evaluasi.

### BAB 3. Metodologi
Isi bagian ini dapat mencakup:
- sumber dataset,
- deskripsi variabel,
- alur penelitian,
- metode preprocessing,
- metode pembagian data,
- metode pelatihan model,
- metode evaluasi.

### BAB 4. Hasil dan Pembahasan
Isi bagian ini dapat mencakup:
- hasil EDA,
- hasil preprocessing,
- hasil pelatihan model,
- hasil evaluasi model,
- analisis performa model,
- pembahasan kelebihan dan kekurangan pendekatan.

### BAB 5. Kesimpulan dan Saran
Isi bagian ini dapat mencakup:
- kesimpulan utama dari analisis,
- jawaban atas tujuan penelitian,
- saran pengembangan atau perbaikan model.

## Contoh Poin Pembahasan
Beberapa poin yang bisa dimasukkan ke dalam pembahasan:
- apakah terdapat missing values pada dataset,
- apakah data target seimbang atau tidak,
- fitur apa yang paling berpengaruh terhadap prediksi,
- bagaimana performa model yang digunakan,
- apakah model masih memerlukan iterasi atau perbaikan.

## Cara Menjalankan
1. Buka file `main.ipynb` menggunakan Jupyter Notebook atau VS Code.
2. Jalankan setiap sel secara berurutan.
3. Amati hasil preprocessing, pelatihan model, dan evaluasi.
4. Gunakan hasil tersebut sebagai dasar penulisan laporan.

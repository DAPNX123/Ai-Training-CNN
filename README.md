# Intel Image Classification: CNN & Transfer Learning

Proyek ini bertujuan untuk mengklasifikasikan citra pemandangan alam ke dalam 6 kategori menggunakan Jaringan Saraf Tiruan (*Convolutional Neural Network* / CNN). Proyek ini berfokus pada penanganan *overfitting* dan peningkatan metrik evaluasi melalui pendekatan *Transfer Learning*.

## 📁 Dataset
Dataset yang digunakan adalah **Intel Image Classification Dataset** yang terdiri dari 6 kelas:
- Buildings (Bangunan)
- Forest (Hutan)
- Glacier (Gletser)
- Mountain (Gunung)
- Sea (Laut)
- Street (Jalanan)

## 🧠 Skenario Eksperimen
Proyek ini membandingkan 3 arsitektur model secara bertahap:
1. **Eksperimen 1 (Baseline Custom CNN):** Model dasar CNN yang dibuat dari awal. Menghasilkan akurasi 83%, namun terdeteksi mengalami *overfitting*.
2. **Eksperimen 2 (CNN + Dropout):** Modifikasi model pertama dengan penambahan lapisan `Dropout(0.5)`. Berhasil menstabilkan model dan menghilangkan *overfitting*.
3. **Eksperimen 3 (Transfer Learning - MobileNetV2):** Menggunakan model pra-latih (*pre-trained*) MobileNetV2. Menghasilkan performa terbaik dengan tingkat akurasi mencapai **90%**.

## 📊 Hasil Analisis Utama (Error Analysis)
- Model mencapai akurasi nyaris sempurna pada kelas **Forest (99.3%)**.
- Kesalahan prediksi tertinggi (*misclassification*) terjadi antara kelas **Glacier** dan **Mountain** karena tingginya kemiripan fitur spasial dan palet warna (tekstur salju putih, bebatuan, dan langit biru).

## 🛠️ Teknologi yang Digunakan
- Python
- TensorFlow / Keras (Deep Learning Framework)
- Scikit-learn (Evaluasi Metrik)
- Matplotlib & Seaborn (Visualisasi Data)

## 🚀 Cara Menjalankan Kode
1. Clone repositori ini:
   ```bash
   git clone [https://github.com/username-kamu/nama-repo-kamu.git](https://github.com/username-kamu/nama-repo-kamu.git)

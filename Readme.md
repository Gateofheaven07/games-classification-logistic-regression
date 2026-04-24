# Analisis Popularitas Game Online: Prediksi Interaksi Menggunakan Model Linear

Proyek ini bertujuan untuk mengklasifikasikan tingkat popularitas game online berdasarkan metadata tekstual seperti nama, deskripsi, dan tag menggunakan teknik Machine Learning.

## 📌 1. Problem Understanding

Masalah utama dalam platform distribusi game adalah banyaknya konten yang tersedia, sehingga sulit untuk memprediksi game mana yang akan mendapatkan interaksi tinggi (likes).

- **Tujuan**: Membangun model klasifikasi untuk membedakan antara game "Populer" dan "Niche".
- **Target**: Biner (1: Populer, 0: Niche), ditentukan berdasarkan median jumlah likes dari seluruh dataset.
- **Pendekatan**: Menggunakan algoritma **Logistic Regression** (Linear Model) karena efektivitasnya yang tinggi dalam menangani data tekstual sparse hasil TF-IDF.

## 📊 2. Data Understanding

Dataset berisi informasi metadata dari ribuan game online. Kolom kunci meliputi:

- `name`: Judul game.
- `likes`: Jumlah interaksi positif (target dasar).
- `description`: Penjelasan singkat mengenai gameplay.
- `tags`: Kategori atau genre game.

**Statistik Data**:

- Total Data: ~11,400 game.
- Threshold Median: Penentuan kelas dilakukan secara otomatis untuk memastikan distribusi data yang seimbang (balanced dataset).

## 💡 3. Business Insights

Berdasarkan hasil analisis dan koefisien model, ditemukan beberapa poin penting:

- **Genre Power**: Game dengan tag 'Action', 'Multiplayer', dan 'Mobile' memiliki peluang lebih tinggi secara signifikan untuk menjadi populer.
- **Optimasi Metadata**: Deskripsi yang mengandung kata kunci spesifik tentang mekanik game (seperti 'driving', 'battle', 'puzzle') membantu algoritma pencarian dan pengguna dalam menemukan game.
- **Engagement Driver**: Game yang bersifat kompetitif atau sosial cenderung mengumpulkan likes lebih banyak dibanding game single-player linier.

## ✅ 4. Kesimpulan

1. **Performa Model**: Algoritma Linear (Logistic Regression) berhasil mencapai akurasi stabil di angka **~73%**.
2. **Kestabilan**: Model menunjukkan kurva belajar (Learning Curve) yang sehat tanpa indikasi overfitting yang parah.
3. **Rekomendasi**: Pengembang sebaiknya fokus pada genre yang memiliki interaksi tinggi dan memastikan kata kunci yang relevan dimasukkan ke dalam metadata tags untuk meningkatkan visibilitas.

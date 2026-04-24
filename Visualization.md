# Dokumentasi Insight Visualisasi

## 1. Top 10 Games Chart

- **Insight**: Menunjukkan dominasi luar biasa dari game mobile (seperti Subway Surfers). Game dengan kategori 'Action' dan 'Running' menduduki peringkat teratas.
- **Kegunaan**: Memberikan benchmark angka likes bagi developer untuk target viralitas.

## 2. Visual Classification Report (Heatmap)

- **Insight**: Skor Precision dan Recall yang seimbang (~0.73) menunjukkan model memiliki performa yang adil pada kelas 0 (Niche) maupun kelas 1 (Populer).
- **Kegunaan**: Memvalidasi kualitas prediksi model pada data yang belum pernah dilihat (test set).

## 3. Confusion Matrix

- **Insight**: Visualisasi ini merinci jumlah prediksi yang benar (diagonal utama). Konsentrasi angka yang tinggi pada True Positives dan True Negatives membuktikan keandalan model.
- **Kegunaan**: Melihat di mana model melakukan kesalahan (False Positive/Negative) untuk perbaikan ke depan.

## 4. Learning Curve

- **Insight**:
  - **Status Model**: Model **TIDAK Overfitting** dan **TIDAK Underfitting** (Good Fit).
  - **Analisis**: Garis skor _Training_ dan _Cross-Validation_ terlihat konvergen (semakin mendekat) seiring bertambahnya jumlah sampel. Jarak (gap) yang sempit di akhir grafik menunjukkan model mampu melakukan generalisasi dengan baik pada data baru, bukan sekadar menghafal data latihan.
- **Kegunaan**: Menjamin stabilitas dan reliabilitas model untuk digunakan pada data produksi.

## 5. Feature Importance (Keywords)

- **Insight**: Kata kunci 'action', 'multiplayer', '3d', dan 'mobile' memiliki nilai koefisien positif tertinggi. Sebaliknya, kata kunci yang terlalu spesifik atau tidak relevan memiliki pengaruh rendah.
- **Kegunaan**: Panduan strategis bagi tim konten untuk melakukan optimasi SEO pada deskripsi game agar meningkatkan potensi popularitas.

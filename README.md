# Classifying Handwritten Digits with SVM

Proyek machine learning untuk mengklasifikasikan gambar angka tulisan tangan (0–9) menggunakan algoritma **Support Vector Machine (SVM)**.

## Deskripsi

Notebook ini membangun model klasifikasi citra digit tulisan tangan dengan SVM. Alurnya mencakup eksplorasi data, praproses, pelatihan model, hingga evaluasi performa. SVM dipilih karena efektif untuk data berdimensi tinggi seperti piksel gambar dan mampu memisahkan kelas non-linear lewat kernel trick.

## Tujuan

- Memahami cara kerja SVM untuk klasifikasi multikelas.
- Membandingkan pengaruh kernel (linear, polynomial, RBF) terhadap akurasi.
- Mengevaluasi model dengan metrik yang tepat.

## Dataset

- Dataset: **MNIST / scikit-learn Digits**
- Isi: gambar digit tulisan tangan beserta label 0–9.

## Alur Kerja

1. **Import library & load data**
2. **Eksplorasi data (EDA)**: visualisasi contoh gambar dan distribusi kelas
3. **Praproses**: normalisasi/scaling piksel, pembagian data latih dan uji
4. **Pelatihan model**: SVM dengan kernel tertentu **['linear', 'poly', 'rbf']**
5. **Tuning hyperparameter** (`C`, `gamma`) dengan GridSearchCV
6. **Evaluasi**: accuracy, precision, recall, F1-score, dan confusion matrix

## Teknologi

- Python
- NumPy, Pandas
- Matplotlib / Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

## Hasil

Model mencapai akurasi sekitar **99.229** pada data uji.
| Class        | Precision | Recall | F1-Score | Support |
|--------------|-----------|--------|----------|---------|
| 0            | 1.00      | 1.00   | 1.00     | 166     |
| 1            | 0.99      | 1.00   | 1.00     | 171     |
| 2            | 1.00      | 1.00   | 1.00     | 167     |
| 3            | 0.98      | 0.99   | 0.99     | 172     |
| 4            | 0.99      | 1.00   | 1.00     | 171     |
| 5            | 0.98      | 0.99   | 0.99     | 167     |
| 6            | 1.00      | 0.99   | 1.00     | 167     |
| 7            | 1.00      | 0.99   | 1.00     | 170     |
| 8            | 0.99      | 0.98   | 0.98     | 166     |
| 9            | 0.98      | 0.97   | 0.98     | 169     |
|              |           |        |          |         |
| Accuracy     | —         | —      | 0.99     | 1686    |
| Macro Avg    | 0.99      | 0.99   | 0.99     | 1686    |
| Weighted Avg | 0.99      | 0.99   | 0.99     | 1686    |

## Cara Menjalankan

1. Clone repositori:
   ```bash
   git clone https://github.com/unggaputra/Classifying-Handwritten-Digits-with-SVM.git
   ```
2. Install dependensi:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn jupyter
   ```
3. Buka dan jalankan notebook:
   ```bash
   jupyter notebook Classifying_Handwritten_Digits_with_SVM.ipynb
   ```

## Author

[unggaputra](https://github.com/unggaputra)

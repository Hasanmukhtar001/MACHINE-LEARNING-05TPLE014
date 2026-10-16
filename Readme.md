# Analisis Variabel Gaya Hidup dan Pola Makan Terhadap Tingkat Obesitas di Dhaka

Proyek ini bertujuan untuk memetakan serta memprediksi tingkat obesitas masyarakat urban berdasarkan kebiasaan konsumsi harian, aktivitas fisik, dan profil fisik individu. Menggunakan **Dhaka Obesity Dataset**, eksperimen dilakukan secara komprehensif mulai dari tahap eksplorasi data (*EDA*), *preprocessing*, *clustering*, hingga pemodelan klasifikasi (*supervised learning*).

---

## 📌 Pendekatan dan Metodologi

Alur kerja pada proyek ini dibagi menjadi beberapa tahapan utama:

1. **Eksplorasi Data Awal (EDA) & Analisis Cluster:**
   - Menelaah karakteristik distribusi fitur numerik seperti *Age*, *Height*, dan *Weight*.
   - Menerapkan *K-Means Clustering* yang dioptimalkan dengan *Elbow Method* serta pemetaan dimensi *PCA 2D* untuk melihat pengelompokan alami profil fisik pasien.

2. **Data Cleaning & Preprocessing:**
   - Identifikasi dan pembersihan data terduplikasi untuk menjaga validitas model.
   - Transformasi variabel kategorikal menjadi format angka menggunakan teknik *One-Hot Encoding* dan *Label Encoding*.
   - Pembagian dataset menjadi data latih (80%) dan data uji (20%) secara proporsional (*Stratified Splitting*).

3. **Pengembangan & Evaluasi Model:**
   - Pelatihan model klasifikasi berbasis *Random Forest* untuk memprediksi kategori kelas *Obesity Level*.
   - Evaluasi performa menggunakan metrik *Accuracy*, *Precision*, *Recall*, dan *F1-Score*.

---

## 🛠️ Stack & Library yang Digunakan

* **Bahasa Pemrograman:** Python
* **Pengolahan & Analisis Data:** `pandas`, `numpy`
* **Visualisasi Data:** `matplotlib`, `seaborn`
* **Machine Learning & Preprocessing:** `scikit-learn` (`RandomForestClassifier`, `KMeans`, `PCA`, `StandardScaler`)

---

## 🚀 Struktur Direktori Project

```text
.
├── Dhaka Obesity.csv     # Dataset utama
├── notebook.ipynb        # Lembar kerja eksplorasi & eksperimen ML
└── README.md             # Dokumentasi proyek  
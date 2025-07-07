# 💬 Analisis Sentimen Ulasan Aplikasi Dana

Repositori ini merupakan proyek analisis sentimen terhadap ulasan pengguna aplikasi **DANA** (Dompet Digital Indonesia) dengan pendekatan **machine learning**. Data dikumpulkan melalui proses scraping dari Google Play Store, kemudian dilakukan pelabelan, pelatihan model, dan evaluasi akurasi klasifikasi sentimen (positif vs negatif).

---

## 📌 Tujuan Proyek

- Mengambil data ulasan aplikasi DANA dari Play Store.
- Membersihkan dan memproses teks ulasan.
- Melakukan pelabelan sentimen berdasarkan kata kunci atau manual.
- Membangun model machine learning untuk klasifikasi sentimen.
- Mengevaluasi performa model dan memberikan insight dari hasil prediksi.

---

## 🧩 File dalam Repositori

- `code_scraping.py`  
  Script Python untuk melakukan web scraping ulasan aplikasi DANA dari Play Store menggunakan library seperti `google-play-scraper` atau `requests + BeautifulSoup`.

- `ulasan_aplikasi.csv`  
  Dataset hasil scraping yang berisi ulasan pengguna, rating, dan waktu posting. File ini menjadi sumber utama untuk proses analisis sentimen.

- `pelatihan_model.ipynb`  
  Notebook Jupyter yang berisi proses:
  - Preprocessing teks (cleansing, stopword removal, stemming)
  - Labeling data sentimen (otomatis/manual)
  - Ekstraksi fitur (TF-IDF)
  - Pelatihan model klasifikasi seperti Naive Bayes, Logistic Regression, atau SVM
  - Evaluasi performa model (akurasi, precision, recall, F1)

- `requirements.txt`  
  Berisi daftar library yang diperlukan agar proyek dapat dijalankan dengan lingkungan Python yang sesuai.

---

## 🔧 Cara Menjalankan

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Jalankan code_scraping.py untuk mengambil data terbaru dari Play Store (opsional, bisa langsung pakai ulasan_aplikasi.csv).

3. Buka dan jalankan seluruh sel dalam pelatihan_model.ipynb untuk melakukan preprocessing, pelatihan, dan evaluasi model klasifikasi sentimen.

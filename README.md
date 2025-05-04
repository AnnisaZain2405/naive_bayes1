# 🎯 Klasifikasi Emosi dari Teks Menggunakan Naive Bayes

Proyek ini merupakan eksperimen sederhana untuk mengklasifikasikan emosi dari teks berbahasa Inggris menggunakan algoritma Machine Learning Naive Bayes, dengan hasil akhir ditampilkan dalam Bahasa Indonesia lengkap dengan ikon emoji. Eksperimen dilakukan menggunakan Google Colab dengan dataset terbuka dari Hugging Face.

---

## 📚 Deskripsi Singkat

Emosi merupakan bagian penting dalam komunikasi manusia. Dengan kemampuan mengklasifikasikan emosi dari teks, sistem AI dapat memahami konteks emosional dari pengguna, yang sangat berguna dalam chatbot, analisis sentimen, maupun aplikasi kesehatan mental.

Eksperimen ini menggunakan pendekatan klasik dengan:
- **Preprocessing teks** (tokenisasi, stopwords removal, normalisasi)
- **Ekstraksi fitur** menggunakan TF-IDF
- **Klasifikasi** menggunakan **Multinomial Naive Bayes**

---

## 🧪 Dataset

Dataset yang digunakan berasal dari:
- 📦 `dair-ai/emotion` dari Hugging Face Datasets
- Jumlah kelas emosi: 6
  - 😢 **Kesedihan** (`sadness`)
  - 😊 **Kebahagiaan** (`joy`)
  - ❤️ **Cinta** (`love`)
  - 😠 **Marah** (`anger`)
  - 😨 **Takut** (`fear`)
  - 😮 **Terkejut** (`surprise`)

---

## 🧠 Algoritma yang Digunakan

### Naive Bayes (MultinomialNB)
- Merupakan model probabilistik sederhana namun efektif.
- Cocok untuk data teks yang telah dikonversi menjadi fitur frekuensi atau TF-IDF.
- Asumsi independensi antar fitur.

---

## 🔧 Langkah-langkah Eksperimen

1. **Load Dataset** dari Hugging Face
2. **Preprocessing** teks (lowercasing, hapus stopwords, karakter khusus)
3. **Transformasi fitur** menggunakan `TfidfVectorizer`
4. **Split data** menjadi data latih dan uji
5. **Training model** Multinomial Naive Bayes
6. **Evaluasi model** menggunakan Confusion Matrix, Akurasi, dan Classification Report
7. **Prediksi interaktif** dari input teks pengguna

---

## 📈 Hasil

- Akurasi model: ~85% (tergantung eksperimen)
- Confusion Matrix menunjukkan performa tinggi pada kelas joy dan sadness
- Dapat memprediksi emosi kalimat seperti:
  Kalimat: "Aku merasa dicintai dan dihargai"
  Hasil: Cinta ❤️

---

## 🎨 Visualisasi

- 📊 Distribusi emosi dari dataset
- 🔍 Confusion Matrix
- 🤖 Output prediksi real-time dengan emoji

---

## 🚀 Cara Menjalankan di Google Colab

1. Buka [Google Colab](https://colab.research.google.com)
2. Upload file `.ipynb` atau copy-paste dari `notebook.ipynb`
3. Jalankan sel dari atas ke bawah

---

## 📝 Referensi

- Dataset: [https://huggingface.co/datasets/dair-ai/emotion](https://huggingface.co/datasets/dair-ai/emotion)
- Scikit-learn Documentation: [https://scikit-learn.org](https://scikit-learn.org)
- NLP Preprocessing: NLTK

---

## 📌 Catatan

Eksperimen ini dapat dikembangkan lebih lanjut menggunakan:
- Model berbasis LSTM atau BERT
- Dataset berbahasa Indonesia
- Tampilan antarmuka interaktif (Gradio atau Streamlit)

---

## 👨‍💻 Penulis

Nama: ANNISA ZAIN NADIA FITRI
Universitas: UIN Prof. K.H. Saifuddin Zuhri Purwokerto  
Mata Kuliah: Metodologi Penelitian Informatika


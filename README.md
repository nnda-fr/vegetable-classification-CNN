# Vegetable Classification Project 🥦🥕🍅

[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat&logo=tensorflow)](https://www.tensorflow.org/)
[![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)](https://www.python.org/)
[![Kaggle](https://img.shields.io/badge/Dataset-Vegetable_Images-green?style=flat&logo=kaggle)](https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset)

Proyek ini adalah sistem klasifikasi gambar otomatis menggunakan **Deep Learning** dengan arsitektur **Convolutional Neural Network (CNN)**. Model dilatih untuk mengenali 15 jenis sayuran berbeda dengan akurasi tinggi (>95%).

## 📌 Fitur Utama
- **Dataset Besar:** Menggunakan lebih dari 15.000 gambar.
- **Manual Data Splitting:** Data dibagi secara mandiri menjadi Train (80%), Validation (10%), dan Test (10%).
- **Multi-Format Deployment:** Model tersedia dalam format `.pb` (SavedModel), `.tflite` (Mobile), dan `.json` (TensorFlow.js).
- **Callback Implementation:** Training otomatis berhenti ketika target akurasi tercapai untuk mencegah *overfitting*.

## 📂 Struktur Direktori Submission
Berdasarkan kriteria proyek, struktur folder diatur sebagai berikut:
```text
submission/
├── tfjs_model/          # Model untuk deployment web (JS)
├── tflite/              # Model terkompresi untuk Android/iOS
├── saved_model/         # Model asli TensorFlow
├── notebook.ipynb       # Kode lengkap eksperimen
├── README.md            # Dokumentasi proyek
└── requirements.txt     # Daftar pustaka (library)

```

## 🛠️ Arsitektur Model

Model dibangun menggunakan API `tf.keras.Sequential` dengan komponen:

* **Conv2D Layer:** Untuk ekstraksi fitur gambar.
* **MaxPooling2D:** Untuk reduksi dimensi spasial.
* **Dropout:** Untuk mengurangi risiko overfitting.
* **Dense Layer:** Sebagai classifier akhir dengan aktivasi Softmax.

## 🚀 Cara Menjalankan

1. **Clone Repository:**
```bash
git clone [https://github.com/username-kamu/vegetable-classification.git](https://github.com/nnda-fr/vegetable-classification.git)

```


2. **Install Dependencies:**
```bash
pip install -r requirements.txt

```


3. **Training/Inference:**
Buka `notebook.ipynb` di Google Colab atau Jupyter Notebook dan jalankan sel secara berurutan.

## 📊 Hasil Evaluasi

Model berhasil mencapai:

* **Training Accuracy:** > 95%
* **Validation Accuracy:** > 95%
* **Test Accuracy:** > 95%

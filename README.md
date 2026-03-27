# Decoding Rest and Detecting Sleep Disorders with Data Science

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

Proyek ini bertujuan untuk menganalisis hubungan antara gaya hidup, parameter kesehatan fisik, dan kualitas tidur untuk mendeteksi gangguan klinis seperti **Insomnia** dan **Sleep Apnea** menggunakan pendekatan Machine Learning.

---

## Business & Research Questions
Melalui proyek ini, saya menjawab beberapa pertanyaan kunci:
1. **Faktor Dominan:** Variabel apa yang paling signifikan dalam memprediksi gangguan tidur?
2. **Korelasi Gaya Hidup:** Sejauh mana tingkat stres dan aktivitas fisik memengaruhi kualitas istirahat?
3. **Prediksi Akurat:** Seberapa efektif model Machine Learning dalam melakukan klasifikasi gangguan tidur secara otomatis?

---

## Dataset Overview
Dataset mencakup informasi komprehensif dari 374 individu, yang terdiri dari:
* **Profil Demografis:** Usia, Jenis Kelamin, Profesi.
* **Parameter Tidur:** Durasi tidur, Kualitas tidur.
* **Aktivitas & Kesehatan:** Tingkat stres, Kategori BMI, Tekanan Darah, Detak Jantung, dan Langkah Harian.
* **Target:** No Disorder, Insomnia, Sleep Apnea.
* **Link Dataset:** [Kaggle - Sleep Health and Lifestyle Dataset](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset/data)

---

## Methodology & Modeling
Saya mengeksperimenkan dua algoritma klasifikasi untuk mendapatkan performa terbaik:

### 1. K-Nearest Neighbors (KNN)
* **Akurasi: 94.67%**
* **Insight:** Performa tinggi pada KNN menunjukkan bahwa data memiliki pemisahan kelas yang sangat jelas (*well-clustered*) berdasarkan kemiripan fitur antar individu.

### 2. Random Forest (RF)
* **Akurasi: 92.00%**
* **Key Finding:** Melalui analisis **Feature Importance**, ditemukan bahwa **Tekanan Darah (Systolic & Diastolic)** memiliki *Information Gain* tertinggi, membuktikan adanya korelasi klinis yang kuat antara hipertensi dan gangguan tidur.

---

## Key Insights
* **Clinical Correlation:** Tekanan darah terbukti menjadi prediktor yang lebih stabil dibandingkan variabel subjektif seperti skor stres.
* **BMI Impact:** Individu dalam kategori *Overweight* menunjukkan kecenderungan lebih tinggi terhadap *Sleep Apnea*.
* **Stress vs Quality:** Terdapat korelasi negatif yang kuat di mana peningkatan tingkat stres secara konsisten menurunkan durasi dan kualitas tidur.

---

## Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn.
* **Platform:** Google Colab

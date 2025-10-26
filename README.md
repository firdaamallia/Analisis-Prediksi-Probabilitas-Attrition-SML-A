# Analisis Prediksi Probabilitas Attrition pada Karyawan

**Nadine Zahirah Putri Widianti** — NRP: 5003231005<br>
**Firda Amallia Trisnawati** — NRP: 5003231006<br>
**Andra Eka Wijayanti** — NRP: 5003231012<br>

Mata Kuliah **Statistics Machine Learning A**<br>
Departemen Statistika, Institut Teknologi Sepuluh Nopember (ITS)

---

## 📚 Daftar Isi
- [Domain Proyek: Sumber Daya Manusia (HR)](#domain-proyek-sumber-daya-manusia-hr)
  - [Referensi](#referensi)
- [Business Understanding](#business-understanding)
  - [Problem Statements](#problem-statements)
  - [Goals](#goals)
  - [Solution Statements](#solution-statements)
  - [Project Benefits](#project-benefits)
- [Data Understanding](#data-understanding)
  - [Sumber Data](#sumber-data)
  - [Deskripsi Fitur](#deskripsi-fitur)
  - [Penjelasan Kontekstual Fitur](#penjelasan-kontekstual-fitur)
  - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Modeling & Evaluation](#modeling--evaluation)
- [Kesimpulan & Insight](#kesimpulan--insight)

---

## Domain Proyek: Sumber Daya Manusia (HR)
Manajemen sumber daya manusia merupakan salah satu pilar utama dalam menjaga keberlanjutan dan daya saing sebuah perusahaan di era bisnis modern. Salah satu tantangan terbesar yang dihadapi organisasi adalah tingginya tingkat attrition atau employee turnover, yaitu kondisi ketika karyawan meninggalkan perusahaan baik secara sukarela maupun tidak. Fenomena ini menimbulkan berbagai konsekuensi, seperti meningkatnya biaya rekrutmen dan pelatihan, menurunnya produktivitas tim, serta terganggunya stabilitas operasional dan moral kerja di lingkungan perusahaan [1]. Beragam faktor dapat memengaruhi keputusan seorang karyawan untuk bertahan atau keluar, mulai dari karakteristik demografis, posisi jabatan, tingkat kepuasan kerja, beban kerja, hingga frekuensi lembur [2]. Pemahaman mendalam terhadap faktor-faktor ini memungkinkan perusahaan untuk mengambil langkah strategis dalam mempertahankan talenta terbaik, meningkatkan kesejahteraan karyawan, serta menciptakan lingkungan kerja yang lebih sehat dan produktif.
Proyek ini berada dalam domain People Analytics dan Human Resource Management (HRM), dengan fokus pada pengembangan model prediktif untuk mempelajari dan memprediksi perilaku employee attrition. Melalui pemanfaatan teknik data science dan machine learning, proyek ini bertujuan untuk mengidentifikasi variabel-variabel yang paling berpengaruh terhadap keputusan karyawan untuk keluar, membangun model prediksi yang mampu mengestimasi kemungkinan attrition secara akurat meskipun menghadapi tantangan seperti ketidakseimbangan kelas dan interaksi fitur yang kompleks, memberikan insight strategis yang dapat digunakan oleh manajemen untuk merancang kebijakan retensi karyawan yang lebih efektif. Dengan demikian, hasil analisis dari proyek ini diharapkan dapat membantu organisasi mengantisipasi potensi turnover lebih dini, meminimalkan biaya yang timbul akibat kehilangan karyawan berprestasi, serta meningkatkan keberlanjutan dan efisiensi operasional perusahaan secara keseluruhan.

### Referensi
- Dataset: IBM HR Analytics Employee Attrition & Performance
- Sumber: [Kaggle Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

---

## Business Understanding

### Problem Statements
Perusahaan mengalami tingkat turnover tinggi dan membutuhkan model untuk memprediksi karyawan yang berpotensi resign.

### Goals
Membangun model klasifikasi untuk memprediksi probabilitas attrition dan menemukan faktor dominan yang memengaruhinya.

### Solution Statements
Menggunakan algoritma machine learning seperti **Logistic Regression, Random Forest, dan LightGBM** untuk menemukan model terbaik dengan metrik **AUC** tertinggi.

### Project Benefits
- Membantu HR mengidentifikasi risiko attrition dini.  
- Menyediakan insight bagi strategi retensi karyawan.  

---

## Data Understanding

### Sumber Data
Data berasal dari dataset IBM HR Analytics (Kaggle) dengan 1470 observasi dan 35 variabel.

### Deskripsi Fitur
Menjelaskan setiap fitur seperti:
- `Age`: Umur karyawan  
- `JobRole`: Jabatan karyawan  
- `MonthlyIncome`: Gaji bulanan  
- `Attrition`: Target variabel (Yes/No)

### Penjelasan Kontekstual Fitur
Fitur numerik dan kategorikal dianalisis untuk memahami pola distribusi dan korelasi antar variabel.

### Exploratory Data Analysis (EDA)
- Visualisasi distribusi dan outlier  
- Analisis missing value  
- Korelasi antar fitur  
- Analisis proporsi karyawan yang keluar

---

## Modeling & Evaluation
Model yang digunakan:
- Logistic Regression  
- Random Forest  
- LightGBM  
- XGBoost  

Evaluasi dilakukan menggunakan metrik:
- Accuracy  
- Precision, Recall, F1-Score  
- ROC-AUC  

Model terbaik: **LightGBM dengan AUC = 0.83**

---

## Kesimpulan & Insight
- Faktor paling berpengaruh terhadap attrition adalah *JobSatisfaction*, *MonthlyIncome*, dan *YearsAtCompany*.  
- Perusahaan dapat mengurangi attrition dengan memperbaiki kompensasi dan engagement karyawan.

---

📊 *Project dibuat untuk tugas mata kuliah Statistical Machine Learning A (2025).*

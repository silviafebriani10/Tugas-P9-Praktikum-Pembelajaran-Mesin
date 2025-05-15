# Analisis Sentimen dengan SVM dan TF-IDF
# # Silvia Febriani – 1227050126

---

### Dataset  
Dataset yang digunakan diunduh dari [https://www.kaggle.com/c/si650winter11/data](https://www.kaggle.com/c/si650winter11/data). Dataset ini berupa file TSV (*tab-separated values*), di mana:

- **Kolom pertama**: Label sentimen (`0` = negatif, `1` = positif)  
- **Kolom kedua**: Teks ulasan

---

### Preprocessing  
Tahapan preprocessing meliputi:

- Lemmatization: mengubah kata ke bentuk dasar  
- Transformasi teks ke dalam bentuk vektor menggunakan **CountVectorizer**

---

### Feature Extraction  
Dilakukan ekstraksi fitur menggunakan **TF-IDF (Term Frequency-Inverse Document Frequency)** untuk memperoleh token atau kata-kata yang paling penting berdasarkan kemunculannya.

---

### SVM Classifier  
Hasil dari TF-IDF digunakan sebagai input untuk model **Support Vector Machine (SVM)**. Model ini digunakan untuk mengklasifikasikan apakah ulasan bersentimen **positif** atau **negatif**.

---

### Hasil  
Berikut adalah hasil evaluasi model berupa **Classification Report**:

          precision    recall  f1-score   support

       0       0.99      0.99      0.99       557
       1       0.99      0.99      0.99       830

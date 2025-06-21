# 📊 Prediksi Risiko Kesehatan Berdasarkan Data Medis dan Dukungan AI Granite

## 🧾 Project Overview

Proyek ini bertujuan untuk mengklasifikasikan tingkat risiko kesehatan seseorang berdasarkan data medis diabetes (usia, tekanan darah, BMI, dan skor metabolik lainnya) dari dataset publik. Dengan bantuan AI model IBM Granite, proyek ini juga menghasilkan ringkasan kondisi pasien dalam bahasa alami dan rekomendasi makanan berdasarkan kondisi tersebut.

Proyek ini menggabungkan pendekatan statistik (Machine Learning) dan pendekatan bahasa alami (LLM) untuk membantu interpretasi data medis menjadi lebih mudah dipahami, khususnya oleh pasien awam maupun tenaga medis.

---

## 🔗 Dataset

Dataset yang digunakan adalah "Dataset diabetes". Dataset dapat diakses melalui link berikut [dataset](https://www.kaggle.com/code/nandaprasetia/dataset-diabetes#Loading-the-Diabetes-Dataset)

---

## 💡 Insight & Findings

1. Fitur dengan korelasi tertinggi terhadap risiko adalah **BMI**, **tekanan darah (bp)**, dan **s5**.
2. Penggunaan model AI (Granite IBM) menambahkan interpretasi manusiawi terhadap data numerik dan menghasilkan ringkasan yang selaras dengan kondisi pasien.
4. AI juga memberikan **rekomendasi makanan** berdasarkan kondisi pasien, sehingga hasil analisis dapat langsung ditindaklanjuti dalam bentuk tindakan preventif.

---

## 🤖 AI Support Explanation

Model AI yang digunakan adalah **IBM Granite 3.3-8B-Instruct**, diakses melalui **Replicate API**.

AI digunakan untuk dua hal utama:
- **Ringkasan kondisi pasien**
- **Rekomendasi gaya hidup/makanan**: Granite memberikan saran makanan yang sebaiknya dikonsumsi atau dihindari

Prompt dikirim dalam Bahasa Indonesia agar output bisa digunakan langsung dalam konteks lokal dan dapat dipahami pengguna awam.

Contoh prompt:
```plaintext
Ringkas kondisi pasien ini dan sebutkan tingkat risiko kesehatannya (Rendah, Sedang, atau Tinggi). Tulis dalam Bahasa Indonesia

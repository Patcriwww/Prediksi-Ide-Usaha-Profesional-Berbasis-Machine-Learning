# Prediksi Ide Usaha Profesional Berbasis Machine Learning

Repository ini berisi implementasi sistem prediksi ide usaha berbasis **Machine Learning** yang dibangun menggunakan **Python dan Flask**. Sistem ini bertujuan untuk membantu pengguna mendapatkan rekomendasi dan prediksi kelayakan ide usaha berdasarkan data historis dan fitur-fitur bisnis tertentu yang diproses oleh model pembelajaran mesin.

Proyek ini dikembangkan sebagai studi penerapan **Data Science dan Machine Learning** dalam bidang kewirausahaan dan pengambilan keputusan bisnis.

---

## Deskripsi Proyek

Aplikasi ini merupakan web-based system yang menggunakan model Machine Learning terlatih untuk melakukan analisis terhadap data usaha, kemudian menghasilkan prediksi atau rekomendasi ide bisnis yang potensial. Sistem terdiri dari:

- Proses training model dari dataset (`dataset.csv`)
- Penyimpanan model dalam format `.pkl`
- REST API berbasis Flask untuk melakukan prediksi
- Antarmuka web sederhana untuk input dan visualisasi hasil

Model dilatih menggunakan pendekatan supervised learning dan disimpan pada folder `models/` untuk digunakan kembali saat proses inferensi.

---

## Fitur Utama

1. Prediksi ide usaha berdasarkan data input pengguna  
2. Model Machine Learning terlatih dan tersimpan (model persistence)  
3. REST API untuk proses inferensi  
4. Antarmuka web sederhana (HTML + CSS)  
5. Ringkasan hasil training dalam format JSON  

---

## Arsitektur Sistem

User Input (Web Interface)  
→ Flask Controller  
→ Prediction Service  
→ Machine Learning Model (.pkl)  
→ Hasil Prediksi  
→ Ditampilkan ke User  

---

## Teknologi yang Digunakan

- Python 3.x  
- Flask  
- Scikit-learn  
- Pandas  
- NumPy  
- HTML, CSS  
- Pickle (Model Serialization)

---

## Struktur Folder

```
Prediksi-Ide-Usaha-Profesional-Berbasis-Machine-Learning/
│
├── app.py
├── config.py
├── requirements.txt
├── controllers/
│   └── prediction_controller.py
├── services/
│   └── prediction_service.py
├── models/
│   ├── predictor.py
│   ├── train_model.py
│   ├── model.pkl
│   └── training_summary.json
├── data/
│   └── dataset.csv
├── templates/
│   └── index.html
├── static/
│   └── style.css
└── README.md
```

---

## Alur Kerja Sistem

1. Dataset diproses dan digunakan untuk melatih model (`train_model.py`).  
2. Model hasil training disimpan dalam format `.pkl`.  
3. User memasukkan parameter usaha melalui web interface.  
4. Controller memanggil service prediksi.  
5. Model melakukan inferensi.  
6. Hasil prediksi dikembalikan dan ditampilkan ke user.  

---

## Cara Menjalankan

1. Install dependency  
   ```bash
   pip install -r requirements.txt
   ```

2. Jalankan server  
   ```bash
   python app.py
   ```

3. Akses melalui browser  
   ```
   http://127.0.0.1:5000
   ```

---

## Tujuan Pembelajaran

Project ini bertujuan untuk memahami:

- Penerapan Machine Learning pada bidang bisnis  
- Proses training dan deployment model  
- Integrasi model ML dengan web application  
- Arsitektur dasar REST API menggunakan Flask  
- Konsep model persistence dan inference  

---

## Author

Fachri Reyhan  
Mahasiswa – Teknologi Informasi / Informatika  
Tahun: 2026  

---

## Lisensi

Proyek ini dibuat untuk keperluan akademik dan pembelajaran.  
Dapat digunakan sebagai referensi dengan mencantumkan sumber.

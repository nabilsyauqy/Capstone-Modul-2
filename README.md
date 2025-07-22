# Airbnb Bangkok Data Analysis

## Deskripsi Proyek
Analisis ini bertujuan untuk mengidentifikasi faktor-faktor utama yang mempengaruhi harga listing Airbnb di Bangkok. Proyek ini mencakup tahapan EDA (Exploratory Data Analysis), data cleaning, analisis per fitur, insight, dan rekomendasi bisnis. Hasil analisis dapat digunakan untuk membantu host menentukan strategi harga yang optimal.

## Struktur File
- `analisis_airbnb_bangkok_struktur.py` — Script utama analisis, sudah naratif dan siap dipecah ke notebook.
- `eda_airbnb_bangkok.py` — Script khusus EDA eksplorasi awal.
- `dashboard_airbnb_bangkok.py` — Dashboard interaktif Streamlit untuk eksplorasi data.
- `Airbnb_Bangkok_Analysis.pptx` — Template presentasi PowerPoint (jika tersedia).
- `airbnb_bangkok_clean.csv` — Data bersih hasil cleaning (diekspor dari script, untuk Tableau/dsb).

## Cara Menjalankan Analisis
1. **Jalankan script utama:**
   - Buka `analisis_airbnb_bangkok_struktur.py` di Jupyter Notebook atau editor Python.
   - Jalankan cell satu per satu dari atas ke bawah.
   - Semua output, insight, dan visualisasi akan muncul sesuai urutan analisis.

2. **Ekspor Data Bersih ke CSV (untuk Tableau/dsb):**
   - Setelah proses cleaning, tambahkan kode berikut:
     ```python
     df.to_csv('airbnb_bangkok_clean.csv', index=False)
     ```
   - File `airbnb_bangkok_clean.csv` akan muncul di folder project.

3. **Jalankan Dashboard Streamlit (opsional):**
   - Pastikan sudah install streamlit: `pip install streamlit`
   - Jalankan di terminal:
     ```bash
     streamlit run dashboard_airbnb_bangkok.py
     ```

4. **Membuat Dashboard Tableau (opsional):**
   - Import file `airbnb_bangkok_clean.csv` ke Tableau Desktop/Public.
   - Buat visualisasi: histogram harga, boxplot, bar chart property_type/neighbourhood, scatterplot harga vs rating, dsb.
   - Gabungkan sheet ke dashboard, tambahkan filter interaktif.

## Insight & Rekomendasi Singkat
- Harga listing dipengaruhi oleh tipe properti, lokasi, jumlah kamar tidur, rating, dan jumlah review.
- Tipe 'Entire home/apt' dan lokasi strategis seperti Sukhumvit, Silom, cenderung memiliki harga lebih tinggi.
- Listing dengan rating dan jumlah review lebih tinggi cenderung lebih mahal.
- Superhost cenderung mematok harga lebih tinggi (jika ada kolom superhost).
- Rekomendasi: Tingkatkan kualitas listing, fokus pada rating, pilih tipe properti dan lokasi strategis, monitor harga kompetitor. 
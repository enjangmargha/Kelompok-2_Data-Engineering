 🌟ETL: Analisis Hubungan Pendidikan dan Pengangguran terhadap Kemiskinan 🌟

📝 Deskripsi
Proyek ini bertujuan untuk melakukan proses ETL (Extract, Transform, Load) untuk menganalisis hubungan antara tingkat pengeluaran pendidikan, tingkat kemiskinan kerja, dan tingkat kemiskinan umum di berbagai negara. Data diekstrak dari sumber publik, dibersihkan, digabungkan, dan dimuat ke database PostgreSQL untuk dianalisis menggunakan model regresi linear. Hasil akhir dari proyek ini adalah sebuah model prediktif beserta rekomendasi kebijakan berbasis data.

🚀 Alur Kerja Proyek
Proyek ini dibagi menjadi beberapa tahapan utama yang terdokumentasi di dalam notebook:

Ekstraksi Data (Extract): Mengambil data dari API World Bank (Pendidikan & Kemiskinan) dan ILO (Kemiskinan Kerja).
Transformasi Data (Transformasi): Membersihkan, memfilter indikator, mengubah format data (wide-to-long), dan menyeragamkan kolom.
Integrasi & Pemuatan (Load): Menggabungkan ketiga dataset yang sudah bersih dan memuatnya ke database PostgreSQL di Aiven.
Analisis & Machine Learning: Membangun model Regresi Linear Sederhana dan Multivariat untuk menemukan korelasi antar variabel.
Rekomendasi Kebijakan: Memberikan saran kebijakan berdasarkan hasil dan interpretasi model.

Tech Stack & Library
🤝 Kontributor
| Contributor                      | GitHub Profile                                   |
|----------------------------------|--------------------------------------------------|
| **Rengga Adhiva Fajar Purnama**  | [🌐 Profile](https://github.com/renggaadhivaaa)  |
| **Abyan Raga Kusuma**            | [🌐 Profile](https://github.com/abyan441)        |
| **Alwi Sihabudin**               | [🌐 Profile](https://github.com/sihabalwi)       |


Ekspor ke Spreadsheet
⚙️ Cara Menjalankan
Clone repositori ini secara lokal:

Bash

git clone [https://github.com/enjangmargha/Kelompok-2_Data-Engineering]
Pasang semua library yang dibutuhkan. Anda dapat menggunakan pip:
Bash

pip install pandas numpy requests scikit-learn matplotlib seaborn sqlalchemy psycopg2-binary
Buka dan jalankan file Kelompok_2_Data_Engineering.ipynb menggunakan Jupyter Notebook atau Google Colab.
Opsional: Untuk menjalankan bagian pemuatan data (Load), pastikan Anda mengganti kredensial koneksi Aiven PostgreSQL di dalam notebook dengan kredensial Anda sendiri.

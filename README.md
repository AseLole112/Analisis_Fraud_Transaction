Fraud transaction adalah transaksi palsu (penipuan) yang terjadi pada transaksi keuangan. Hal ini merupakan suatu hal yang sangat penting untuk dicegah dimana kita sebagai manusia membutuhkan uang dalam memenuhi kebutuhan hidup kita sehari-hari. Dan bukan suatu hal yang tidak mungkin di zaman serba canggih ini kita menggunakan transaksi transfer sebagai sarana transaksi. Dan seiring banyak digunakannya transaksi transfer tersebut, banyak oknum yang memanfaatkan hal ini untuk menipu orang lain. 

Analisis Fraud Transaction Detection adalah proyek deteksi fraud (penipuan) pada transaksi keuangan. Di mana sistem ini sebagai "satpam digital" yang bekerja 24/7 untuk mengecek setiap transaksi yang masuk dan memberikan peringatan jika ada sesuatu yang terlihat tidak beres.

Apa yang Dilakukan Proyek Ini?
Proyek ini mengubah model Machine Learning yang rumit menjadi sebuah API (Application Programming Interface) yang bisa diakses dari mana saja.
Pedoman dari proyek ini : https://github.com/juniorcl/transaction-fraud-detection

Input: Data transaksi (jumlah uang, saldo awal, jenis transaksi, dll) yang berjumlah sebanyak 6 juta lebih transaksi.

Proses: Data "dibersihkan" secara otomatis, diolah fiturnya (Feature Engineering), dan discale agar model paham.

Output: Prediksi instan — apakah transaksi ini Aman (0) atau Mencurigakan/Fraud (1).

Untuk membangun ini, saya menggunakan:

Python & Pandas: Untuk mengolah data mentah.

Scikit-Learn: Otak di balik model deteksi fraud saya.

Flask: Jembatan (web server) agar model saya bisa menerima "tamu" (data) dari luar.

Ngrok: Terowongan ajaib yang membuat server lokal di laptop saya bisa diakses dari seluruh dunia via internet.

📂 Struktur Pipeline
Sistem ini tidak langsung menebak begitu saja. Ada proses yang disebut Pipeline untuk memastikan data rapi sebelum masuk ke model:

Data Cleaning: Mengubah nama kolom yang berantakan menjadi rapi (snake_case).

Feature Engineering: Membuat informasi baru dari data yang ada (misal: menghitung selisih saldo sebelum dan sesudah transaksi).

Data Preparation: Mengubah kategori menjadi angka dan menyeimbangkan skala data (Scaling).

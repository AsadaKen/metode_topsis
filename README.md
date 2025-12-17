# 🧮 Sistem Pendukung Keputusan (SPK) - Metode TOPSIS

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

> Aplikasi berbasis web sederhana untuk membantu pengambilan keputusan menggunakan metode **TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution)**.

## 📖 Tentang Proyek

Proyek ini adalah implementasi algoritma **TOPSIS** menggunakan **Vanilla JavaScript** (tanpa framework/library tambahan). Aplikasi ini dirancang untuk menyelesaikan masalah Multi-Criteria Decision Making (MCDM) secara dinamis.

User dapat menentukan sendiri jumlah kriteria, bobot, jenis atribut (Benefit/Cost), serta rentang nilai (sub-kriteria) yang diinginkan. Perhitungan dilakukan secara *real-time* di sisi klien (browser).

### ✨ Fitur Utama
* **Dynamic Configuration:** Jumlah kriteria dan rentang nilai tidak dibatasi (fleksibel).
* **Interactive UI:** Desain modern, bersih, dan responsif (Mobile Friendly).
* **CRUD Data:** Tambah, Edit, dan Hapus data alternatif dengan mudah.
* **Step-by-Step Calculation:** Menampilkan transparansi perhitungan:
    1.  Konversi Nilai Gap.
    2.  Matriks Normalisasi (R).
    3.  Matriks Terbobot (Y).
    4.  Solusi Ideal Positif (A+) & Negatif (A-).
    5.  Jarak Euclidean (D+ & D-).
    6.  Nilai Preferensi (V) & Perangkingan.

## 🛠️ Teknologi yang Digunakan

* **HTML5:** Struktur semantik halaman.
* **CSS3:** Styling modern (Flexbox/Grid), Responsive Design, dan Custom Properties (Variables) untuk tema warna.
* **Vanilla JavaScript (ES6+):** Logika algoritma TOPSIS, manipulasi DOM, dan manajemen state aplikasi.

## 🚀 Cara Menjalankan

Aplikasi ini bersifat **Static Web Page**, artinya tidak memerlukan instalasi backend (seperti PHP/Node.js) atau database server.

1.  **Clone** repositori ini:
2.  Buka file `index.html` menggunakan browser modern (Chrome, Edge, Firefox).
3.  Aplikasi siap digunakan!

## 🧠 Alur Logika TOPSIS

Aplikasi ini mengikuti tahapan standar metode TOPSIS:
1.  **Membangun Matriks Keputusan Terormalisasi:**
    Setiap nilai alternatif dibagi dengan akar dari jumlah kuadrat semua nilai pada kriteria tersebut.
2.  **Membangun Matriks Terormalisasi Terbobot:**
    Mengalikan matriks normalisasi dengan bobot preferensi (W) yang telah ditentukan.
3.  **Menentukan Solusi Ideal:**
    * **Ideal Positif (A+):** Nilai Max (jika Benefit) atau Min (jika Cost).
    * **Ideal Negatif (A-):** Nilai Min (jika Benefit) atau Nilai Max (jika Cost).
4.  **Menghitung Jarak Solusi (Separation Measure):**
    Menggunakan rumus jarak Euclidean.
5.  **Menghitung Nilai Preferensi:**
    Menentukan kedekatan relatif terhadap solusi ideal positif. Alternatif dengan nilai tertinggi menjadi prioritas utama.

## 👨‍💻 Author

Dibuat dengan ❤️ oleh **Anugrah Syahru Ramadhan**
* Mahasiswa Teknik Informatika
* Universitas Teknologi Akba Makassar

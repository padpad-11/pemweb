# Dokumentasi Tugas 2 Pemweb - Pusat Karir ITERA

## 1. Alasan Penggunaan Struktur Semantik
Penggunaan elemen semantik HTML5 bertujuan agar struktur dokumen halaman web memiliki makna yang jelas, baik bagi pengembang, mesin pencari (SEO), maupun teknologi pembaca layar (*screen reader*).

* **`<header>`**: Digunakan sebagai area navigasi utama dan identitas situs (Logo dan Judul Career Center ITERA).
* **`<nav>`**: Membungkus daftar tautan navigasi (navbar) agar browser mengenali area tersebut sebagai menu utama.
* **`<main>`**: Membungkus seluruh konten utama halaman web agar terpisah dari navigasi header dan footer.
* **`<section>`**: Membagi halaman menjadi beberapa kelompok konten berdasarkan kriteria tertentu (Beranda, Tentang, Aktivitas, Berita).
* **`<article>`**: Digunakan untuk bagian informasi yang dapat berdiri sendiri, seperti postingan Informasi Kolaborasi, Lowongan, dan Beasiswa.
* **`<aside>`**: Membungkus informasi pendukung atau pelengkap seperti Alamat Lokasi Kampus dan Kontak Langsung.
* **`<table>`**: Digunakan untuk menyajikan data terstruktur berupa Jadwal Operasional Kantor.
* **`<footer>`**: Berisi informasi hak cipta, lokasi, dan tautan akses cepat ke fakultas-fakultas di ITERA.

---

## 2. Tantangan dan Solusi

* **Tantangan 1: Navigasi Navbar Tidak Merespons Tanpa CSS/JS**
  * *Solusi*: Menggunakan atribut `id` pada setiap elemen target (`<section>` dan `<article>`) yang nilainya disesuaikan dengan nilai `href="#..."` pada tag `<a>` di dalam navbar.

* **Tantangan 2: Warning pada Validasi W3C Validator**
  * *Solusi*: 
    1. Mengubah tag `<p>` judul pada elemen `<article>` menjadi tag heading (`h3`) karena W3C mewajibkan setiap `<article>` memiliki heading.
    2. Mengubah hirarki `<h1>` banner menjadi `<h2>` agar hanya ada satu `<h1>` utama pada dokumen.
    3. Menghapus atribut usang (*obsolete*) `border` dan `cellspacing` pada tag `<table>`.

* **Tantangan 3: Kendala Identitas dan Path Terlalu Panjang pada Git/GitHub**
  * *Solusi*: Menyelaraskan lokasi inisialisasi Git tepat di dalam folder proyek, mengonfigurasi identitas global Git (`user.email` & `user.name`), serta menambahkan aturan `.gitignore` untuk mengecualikan folder `.vscode`.

---

## 3. Hasil Validasi
Halaman HTML ini telah diuji menggunakan **W3C Markup Validation Service** dan dinyatakan memenuhi standar HTML

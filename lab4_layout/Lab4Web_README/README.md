# Lab4Web — Praktikum Layout Web

## Deskripsi
Repository **Lab4Web** berisi hasil praktikum pemrograman web tentang pembuatan layout halaman menggunakan HTML dan CSS. Praktikum dimulai dari box element, kemudian dikembangkan menjadi halaman dengan header, navigasi, konten utama, sidebar/widget, kartu fitur, dan footer.

## Tujuan Praktikum
- Memahami penggunaan elemen `div` sebagai wadah konten.
- Mengatur warna, jarak, ukuran, dan tata letak menggunakan CSS.
- Membuat navigasi ant halaman.
- Menyusun area konten utama dan sidebar/widget.
- Mengembangkan halaman **About** dan **Contact**.
- Mendokumentasikan proses pengerjaan melalui screenshot.

## Struktur File
Contoh struktur folder yang disarankan:

```text
Lab4Web/
├── home.html
├── artikel.html
├── about.html
├── kontak.html
├── style.css
├── README.md
└── assets/
    ├── home-html-struktur.png
    └── home-html-konten.png
```

> Sesuaikan nama file dan folder dengan struktur proyek yang digunakan. Pastikan gambar screenshot berada di folder `assets` agar tampil di README GitHub.

## Langkah Praktikum

### 1. Membuat struktur HTML
Buat file `home.html` dengan deklarasi HTML, bagian `head`, pengaturan karakter UTF-8, viewport, judul halaman, dan pemanggilan file CSS melalui:

```html
<link rel="stylesheet" href="style.css">
```

Di dalam `body`, siapkan wadah utama untuk menampung elemen-elemen halaman.

### 2. Membuat header dan navigasi
Tambahkan judul halaman menggunakan elemen `<header>` dan menu navigasi menggunakan `<nav>`. Menu mengarah ke halaman Home, Artikel, About, dan Kontak.

```html
<header>
  <h1>Layout Sederhana</h1>
</header>

<nav>
  <a href="home.html" class="active">Home</a>
  <a href="artikel.html">Artikel</a>
  <a href="about.html">About</a>
  <a href="kontak.html">Kontak</a>
</nav>
```

### 3. Menambahkan konten utama
Bagian hero menampilkan judul, paragraf pengantar, dan tautan untuk membaca informasi lebih lanjut. Gunakan elemen `<section>` agar struktur konten lebih teratur.

### 4. Membuat sidebar/widget
Sidebar menggunakan elemen `<aside>`. Di dalamnya dapat dibuat widget daftar tautan dan widget teks informasi. Widget membantu menampilkan informasi tambahan tanpa mengganggu konten utama.

### 5. Menambahkan kartu fitur
Kartu fitur dapat memuat gambar, judul, deskripsi, dan tautan detail. Pada contoh praktikum digunakan gambar placeholder untuk memperlihatkan bentuk dan ukuran gambar. Ganti placeholder dengan gambar proyek sendiri jika diperlukan.

### 6. Menambahkan footer
Footer menampilkan informasi hak cipta atau identitas pembuat halaman, misalnya:

```html
<footer>
  <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
```

### 7. Membuat halaman About
Halaman About berisi deskripsi singkat tentang profil atau situs, tujuan, keahlian, serta portofolio. Portofolio dapat disusun dalam bentuk beberapa kartu proyek.

### 8. Membuat halaman Contact
Halaman Contact berisi formulir yang dapat diisi pengunjung, misalnya nama, email, subjek, dan pesan. Gunakan label yang terhubung dengan input agar formulir lebih mudah digunakan. Atribut `required` dapat ditambahkan pada kolom wajib.

### 9. Menguji halaman
Buka `home.html` menggunakan browser atau jalankan melalui ekstensi Live Server pada Visual Studio Code. Periksa navigasi, tampilan layout, tautan, dan formulir. Pastikan semua file HTML menggunakan nama file dan lokasi yang sesuai dengan tautan navigasinya.

## Screenshot Praktikum

### Struktur awal `home.html`
![Struktur awal home.html](assets/home-html-struktur.png)

Screenshot ini menunjukkan bagian awal dokumen HTML, pemanggilan stylesheet, serta susunan header dan navigasi.

### Konten dan sidebar `home.html`
![Konten dan sidebar home.html](assets/home-html-konten.png)

Screenshot ini menunjukkan bagian hero, widget/sidebar, dan awal area konten utama beserta kartu fitur.

## Menjalankan Proyek
1. Buka folder proyek `Lab4Web` di Visual Studio Code.
2. Pastikan file HTML dan `style.css` berada di lokasi yang benar.
3. Klik kanan `home.html`, lalu pilih **Open with Live Server** jika ekstensi Live Server tersedia. Alternatifnya, buka file HTML langsung melalui browser.
4. Gunakan menu navigasi untuk membuka halaman Home, Artikel, About, dan Kontak.

## Git: Commit dan Push
Jika repository GitHub belum dihubungkan, jalankan perintah berikut di terminal pada folder proyek. Ganti `USERNAME` dengan nama akun GitHub sendiri.

```bash
git init
git add .
git commit -m "Praktikum Lab4Web: layout web"
git branch -M main
git remote add origin https://github.com/USERNAME/Lab4Web.git
git push -u origin main
```

Jika remote repository sudah pernah ditambahkan, tidak perlu menjalankan `git remote add origin` lagi. Untuk perubahan berikutnya, gunakan:

```bash
git add .
git commit -m "Menambahkan halaman About dan Contact"
git push
```

Setelah berhasil diunggah, salin URL repository GitHub dan kumpulkan melalui e-learning eCampus.

## Kesimpulan
Praktikum ini memperkenalkan pembuatan layout web menggunakan HTML dan CSS. Struktur halaman disusun melalui header, navigasi, konten utama, sidebar/widget, kartu fitur, dan footer. Halaman About digunakan untuk menampilkan deskripsi dan portofolio, sedangkan halaman Contact menyediakan formulir pesan. Dokumentasi README dan screenshot membantu menjelaskan tahapan pengerjaan serta hasil praktikum.

---
**Catatan:** Pastikan halaman `about.html` dan `kontak.html` sudah dibuat dan diuji sebelum dikumpulkan. Screenshot tambahan dari hasil tampilan browser juga dapat dimasukkan ke folder `assets` dengan menambahkan sintaks `![Keterangan screenshot](assets/nama-file.png)` pada bagian yang sesuai.

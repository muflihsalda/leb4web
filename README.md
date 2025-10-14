🧾 LAPORAN PRAKTIKUM 4 – CSS Layout

Nama: (isi nama kamu)
NIM: (isi NIM kamu)
Kelas: (isi kelas kamu)
Mata Kuliah: Pemrograman Web
Dosen Pengampu: Agung Nugroho, S.Kom., M.Kom
Universitas: Universitas Pelita Bangsa

🎯 Tujuan Praktikum

Mahasiswa memahami struktur dasar pembuatan layout web.

Mahasiswa memahami konsep box element (margin, padding, border, content).

Mahasiswa mampu menggunakan CSS Float untuk mengatur tata letak elemen.

Mahasiswa memahami penggunaan HTML5 Semantic Element.

Mahasiswa dapat membuat layout web sederhana dengan tampilan profesional.

🧰 Peralatan dan Bahan

Text Editor: Visual Studio Code

Browser: Google Chrome / Microsoft Edge

Bahasa: HTML5 & CSS3

Folder proyek: Lab4Web

🧩 Langkah-Langkah Praktikum
1️⃣ Membuat Struktur Awal HTML

Membuat file home.html dengan struktur dasar HTML5 dan menautkan style.css.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
        <header><h1>Layout Sederhana</h1></header>
    </div>
</body>
</html>


Penjelasan:
Bagian ini merupakan struktur awal dokumen HTML dengan container sebagai pembungkus utama layout.

2️⃣ Menambahkan Navigasi

Menambahkan elemen <nav> berisi link navigasi ke halaman lain.

<nav>
    <a href="home.html" class="active">Home</a>
    <a href="artikel.html">Artikel</a>
    <a href="about.html">About</a>
    <a href="kontak.html">Kontak</a>
</nav>


Penjelasan:
Tag <nav> berfungsi sebagai navigasi utama untuk berpindah antar halaman. Class active digunakan untuk menandai halaman yang sedang dibuka.

3️⃣ Membuat Hero Section

Membuat area banner utama (Hero Panel) untuk memperkenalkan isi website.

<section id="hero">
    <h1>Hello World!</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>


Penjelasan:
Bagian ini biasanya ditempatkan di bawah navigasi dan berfungsi sebagai elemen visual utama dari halaman.

4️⃣ Menambahkan Konten Utama dan Sidebar

Membagi halaman menjadi dua bagian utama dengan float:

Main Content (#main)

Sidebar (#sidebar)

<section id="wrapper">
    <section id="main">
        <div class="row">
            <div class="box">
                <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">
                <h3>Heading</h3>
                <p>Deskripsi singkat konten.</p>
            </div>
        </div>
    </section>

    <aside id="sidebar">
        <div class="widget-box">
            <h3 class="title">Widget Header</h3>
            <ul>
                <li><a href="#">Widget Link</a></li>
                <li><a href="#">Widget Link</a></li>
            </ul>
        </div>
    </aside>
</section>


Penjelasan:
Bagian ini mengatur layout dua kolom menggunakan float. Elemen aside digunakan untuk menempatkan konten tambahan di sisi kanan.

5️⃣ Menambahkan Artikel dan Divider

Membuat bagian artikel dengan tag <article> dan garis pembatas <hr class="divider" />.

<hr class="divider" />
<article class="entry">
    <h2>Featurette Heading</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
    <p>Isi artikel atau deskripsi konten utama...</p>
</article>


Penjelasan:
Elemen <article> menandakan isi konten utama.
<hr> digunakan sebagai pemisah antar bagian agar lebih rapi.

6️⃣ Membuat Halaman About

Membuat halaman baru about.html berisi deskripsi dan portfolio.

Isi utamanya seperti:

<section id="hero">
  <h1>Tentang Kami</h1>
  <p>Informasi tentang profil dan portfolio.</p>
</section>


Penjelasan:
Halaman ini menampilkan deskripsi singkat, serta contoh karya atau project yang pernah dibuat.

7️⃣ Membuat Halaman Kontak

Membuat halaman baru kontak.html dengan form input.

<form class="contact-form">
  <label for="nama">Nama:</label>
  <input type="text" id="nama" name="nama">

  <label for="email">Email:</label>
  <input type="email" id="email" name="email">

  <label for="pesan">Pesan:</label>
  <textarea id="pesan" name="pesan"></textarea>

  <button type="submit">Kirim Pesan</button>
</form>


Penjelasan:
Form ini berfungsi untuk mengumpulkan data dari pengguna, meskipun belum tersambung ke backend (simulasi tampilan saja).

8️⃣ Membuat Footer

Tambahkan footer di bagian bawah halaman.

<footer>
    <p>&copy; 2025 - Universitas Pelita Bangsa</p>
</footer>


Penjelasan:
Footer berfungsi menampilkan informasi hak cipta atau kontak tambahan.

9️⃣ Menulis Style CSS

File style.css digunakan untuk mengatur tampilan setiap elemen agar layout terlihat rapi.

Contoh potongan penting:

body {
    font-family: 'Open Sans', sans-serif;
    color: #5a5a5a;
}
nav {
    background-color: #1f5faa;
}
#hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
}
#main {
    float: left;
    width: 640px;
    padding: 20px;
}
#sidebar {
    float: left;
    width: 260px;
    padding: 20px;
}
footer {
    clear: both;
    background-color: #1d1d1d;
    color: #eee;
    text-align: center;
    padding: 20px;
}


Penjelasan:
Setiap bagian diberi styling tersendiri agar posisi, warna, dan jarak antar elemen tampak proporsional.

📸 Hasil Tampilan Akhir

Halaman Home

Menampilkan header, navigasi, hero, main content, sidebar, dan footer.
(sertakan screenshot di laporan)

Halaman About

Menampilkan deskripsi dan portfolio proyek.
(sertakan screenshot di laporan)

Halaman Kontak

Menampilkan form isian nama, email, pesan.
(sertakan screenshot di laporan)

✅ Kesimpulan

Dari praktikum ini dapat disimpulkan bahwa:

Layout web dapat dibuat dengan mengombinasikan HTML5 semantic element dan CSS Float.

Elemen seperti header, nav, section, article, aside, dan footer membantu membentuk struktur layout yang terorganisir.

Dengan satu file CSS, tampilan setiap halaman dapat dijaga konsistensinya.

Mahasiswa mampu membuat layout web sederhana yang responsif dan menarik secara visual.

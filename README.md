# lab4web

# Praktikum 4: CSS Layout
<p>Nama  :Muflih Salda Maulana</p>
<p>Nim  :312410527</p>
<p>Kelas  :TI.24.A5</p>

## Tujuan
1. Memahami struktur dasar pembuatan layout web.
2. Memahami konsep box element.
3. Memahami penggunaan CSS float dan clear.
4. Memahami HTML5 semantic element.
5. Membuat layout web sederhana menggunakan CSS.

---

## Tahap 1 – Membuat Struktur Dasar HTML
Langkah pertama adalah membuat file **home.html** berisi kerangka HTML dasar dengan elemen:
`<header>`, `<nav>`, `<section>`, dan `<footer>`.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Layout Sederhana</title>
</head>
<body>
  <header><h1>Layout Sederhana</h1></header>
  <nav>
    <a href="home.html">Home</a>
    <a href="artikel.html">Artikel</a>
    <a href="about.html">About</a>
    <a href="kontak.html">Kontak</a>
  </nav>
  <footer>© 2021 - Universitas Pelita Bangsa</footer>
</body>
</html>
````

**Hasil Tahap 1:**
Tampilan masih polos tanpa CSS.

<img width="672" height="298" alt="layout sederhana1" src="https://github.com/user-attachments/assets/79e34b5f-7ee8-4c8f-a98d-7660eb3de3f7" />

---

## Tahap 2 – Menambahkan File CSS dan Styling Dasar

Buat file **style.css** lalu hubungkan ke `home.html`.
Tambahkan pengaturan font, margin, dan header agar tampilan lebih rapi.

```css
* { margin: 0; padding: 0; }
body {
  font-family: 'Open Sans', sans-serif;
  color: #5a5a5a;
}
header h1 {
  color: #b5b5b5;
  margin: 20px 10px;
}
```

**Hasil Tahap 2:**
Teks menjadi lebih halus dan tata letak mulai terlihat rapi.

<img width="679" height="290" alt="layout sederhana2" src="https://github.com/user-attachments/assets/79501ed0-4b93-4b67-992c-72b5d62e63f7" />

---

## Tahap 3 – Membuat Navigasi

Tambahkan CSS untuk membuat navigasi berwarna biru dan tombol aktif.

```css
nav {
  background-color: #1f5faa;
}
nav a {
  color: white;
  padding: 15px 30px;
  display: inline-block;
  text-decoration: none;
  font-weight: bold;
}
nav a:hover, nav a.active {
  background-color: #2b83ea;
}
```

**Hasil Tahap 3:**
Navigasi sudah berwarna biru dengan efek hover dan tampilan aktif pada menu **Home**.

<img width="679" height="409" alt="layout sederhana3" src="https://github.com/user-attachments/assets/1dcf7366-f4f8-45d1-b565-df1b35630d99" />

---

## Tahap 4 – Menambahkan Hero Section

Tambahkan bagian **Hero** berisi judul dan teks sambutan menggunakan `<section id="hero">`.

```html
<section id="hero">
  <h1>Hello World!</h1>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
  <a href="#" class="btn">Learn more »</a>
</section>
```

Dan tambahkan CSS:

```css
#hero {
  background-color: #e4e4e5;
  padding: 50px 20px;
  margin-bottom: 20px;
}
#hero h1 { font-size: 35px; }
```

**Hasil Tahap 4:**
Tampilan menampilkan area hero dengan teks dan tombol link.

<img width="1346" height="595" alt="layout sederhana4" src="https://github.com/user-attachments/assets/30d6d5b3-6223-45fe-974d-903761cc33be" />

---

## Tahap 5 – Menambahkan Sidebar Widget

Tambahkan elemen `<aside>` dengan beberapa widget.

```html
<aside id="sidebar">
  <div class="widget-box">
    <h3 class="title">Widget Header</h3>
    <ul>
      <li><a href="#">Widget Link</a></li>
      <li><a href="#">Widget Link</a></li>
      <li><a href="#">Widget Link</a></li>
      <li><a href="#">Widget Link</a></li>
      <li><a href="#">Widget Link</a></li>
    </ul>
  </div>
  <div class="widget-box">
    <h3 class="title">Widget Text</h3>
    <p>Vestibulum lorem elit, iaculis in nisl volutpat...</p>
  </div>
</aside>
```

**Hasil Tahap 5:**
Tampilan sudah memiliki sidebar di sisi kanan dengan area widget.

<img width="1149" height="720" alt="layout sederhana5" src="https://github.com/user-attachments/assets/b192df54-4919-4360-a1f7-8246cf4a8a4b" />

---

## Tahap 6 – Menambahkan Box Content pada Main

Tambahkan 3 box konten dalam `<section id="main">`.

```html
<div class="box">
  <img src="https://dummyimage.com/120/db7d25/fff.png" class="image-circle">
  <h3>Heading</h3>
  <p>Donec sed odio dui...</p>
  <a href="#">View detail</a>
</div>
```

Dan CSS:

```css
.box {
  float: left;
  width: 33.3%;
  text-align: center;
  padding: 10px;
}
.image-circle { border-radius: 50%; }
```

**Hasil Tahap 6:**
Tampilan menampilkan tiga box berjejer rapi di bawah hero panel.

<img width="1108" height="718" alt="layout sederhana6" src="https://github.com/user-attachments/assets/35a356db-0737-448b-afd3-1dbcd86fd0f1" />


---

## Tahap 7 – Menambahkan Artikel dan Tampilan Akhir

Tambahkan artikel dengan gambar di sisi kiri dan kanan serta divider pemisah.

```html
<article class="entry">
  <h2>First featurette heading.</h2>
  <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
  <p>Lorem ipsum dolor sit amet...</p>
</article>
```

Tambahkan CSS:

```css
.entry img {
  float: left;
  margin-right: 15px;
  border-radius: 5px;
}
.divider {
  border-top: 1px solid #eee;
  margin: 40px 0;
}
```

📸 **Hasil Tahap 7:**
Layout web sudah lengkap — terdiri dari header, navigasi, hero, konten utama, sidebar, dan footer.

<img width="1069" height="679" alt="layout sederhana7" src="https://github.com/user-attachments/assets/660687d1-ab2a-4674-8bc3-967fae6a4411" />

---
**Hasil MenambahKan Menu About Dan Kontak**
<p>About</p>
<img width="1215" height="719" alt="hasil tambahan about" src="https://github.com/user-attachments/assets/612a8bf0-bf87-492e-8ea6-4976bc25f522" />

<p>Kontak</p>

<img width="1139" height="671" alt="hasil tambahan kontak" src="https://github.com/user-attachments/assets/f2219689-0e6a-4b42-99b7-09c6a3fd1e04" />

## Kesimpulan

Dari praktikum ini, telah dipelajari bagaimana:

* Menggunakan **CSS float** dan **clear** untuk mengatur posisi elemen.
* Memanfaatkan **HTML5 semantic elements** dalam pembuatan layout.
* Menggabungkan HTML dan CSS menjadi satu tampilan web yang rapi dan terstruktur.


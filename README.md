
# 🧾 **LAPORAN PRAKTIKUM 4 – CSS Layout**

**Nama:** *(Muflih Salda Maulana)*

**NIM:** *(312410527)*

**Kelas:** *(TI.24.A5)*

**Mata Kuliah:** Pemrograman Web

**Dosen Pengampu:** Agung Nugroho, S.Kom., M.Kom

**Universitas Pelita Bangsa**

---

## 🎯 **Tujuan Praktikum**

1. Memahami struktur dasar pembuatan layout web.
2. Mempelajari konsep **box model**: margin, padding, border, dan content.
3. Menerapkan **CSS Float** untuk mengatur posisi elemen.
4. Menggunakan elemen semantik HTML5 (`header`, `nav`, `section`, `article`, `footer`).
5. Membuat layout web sederhana yang terstruktur dan konsisten.

---

## 🧰 **Peralatan dan Bahan**

* **Text Editor:** Visual Studio Code
* **Browser:** Google Chrome / Edge
* **Bahasa:** HTML5 dan CSS3
* **Struktur Folder:**

  ```
  Lab4Web/
  ├── home.html
  ├── about.html
  ├── kontak.html
  └── style.css
  ```

---

## 🧩 **Langkah-Langkah Praktikum**

---

### **1️⃣ Membuat Struktur Awal HTML**

Buka Visual Studio Code → buat folder `Lab4Web`.
Di dalamnya buat file baru `home.html`.

```html
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
```

🖼️ **Gambar 1.1** – Tampilan awal `home.html` di browser
*(contoh: hasil awal hanya teks “Layout Sederhana”)*
![Gambar 1.1](screenshots/gambar1.png)

---

### **2️⃣ Menambahkan Navigasi (Menu)**

Tambahkan elemen `<nav>` di bawah header:

```html
<nav>
  <a href="home.html" class="active">Home</a>
  <a href="artikel.html">Artikel</a>
  <a href="about.html">About</a>
  <a href="kontak.html">Kontak</a>
</nav>
```

🖼️ **Gambar 2.1** – Tampilan menu navigasi pada browser
![Gambar 2.1](screenshots/gambar2.png)

**Penjelasan:**
Tag `<nav>` digunakan untuk membuat menu utama website.
Class `active` digunakan menandai halaman yang sedang aktif.

---

### **3️⃣ Membuat Hero Section (Banner Utama)**

Tambahkan kode berikut di bawah `<nav>`:

```html
<section id="hero">
  <h1>Hello World!</h1>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
  <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```

🖼️ **Gambar 3.1** – Tampilan hero/banner utama
![Gambar 3.1](screenshots/gambar3.png)

**Penjelasan:**
Bagian ini menampilkan teks utama dan tombol untuk memperkenalkan isi website.

---

### **4️⃣ Membuat Konten Utama dan Sidebar**

Tambahkan struktur berikut di bawah hero section:

```html
<section id="wrapper">
  <section id="main">
    <div class="row">
      <div class="box">
        <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">
        <h3>Heading</h3>
        <p>Deskripsi singkat konten utama.</p>
      </div>
      <div class="box">
        <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="image-circle">
        <h3>Heading</h3>
        <p>Deskripsi singkat konten utama.</p>
      </div>
    </div>
  </section>

  <aside id="sidebar">
    <div class="widget-box">
      <h3 class="title">Widget Header</h3>
      <ul>
        <li><a href="#">Widget Link 1</a></li>
        <li><a href="#">Widget Link 2</a></li>
      </ul>
    </div>
  </aside>
</section>
```

🖼️ **Gambar 4.1** – Tampilan dua kolom (konten dan sidebar)
![Gambar 4.1](screenshots/gambar4.png)

**Penjelasan:**

* Elemen `#main` berisi konten utama.
* Elemen `#sidebar` digunakan untuk menampilkan widget tambahan.
* Posisi diatur dengan **CSS Float**.

---

### **5️⃣ Menambahkan Artikel dan Divider**

Tambahkan di bawah konten utama:

```html
<hr class="divider" />
<article class="entry">
  <h2>Featurette Heading</h2>
  <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
  <p>Isi artikel utama...</p>
</article>
```

🖼️ **Gambar 5.1** – Tampilan artikel dengan pembatas garis
![Gambar 5.1](screenshots/gambar5.png)

**Penjelasan:**
Elemen `<article>` digunakan untuk konten artikel, sedangkan `<hr>` memberi garis pemisah antar bagian.

---

### **6️⃣ Membuat Halaman About**

Buat file baru **`about.html`**, lalu isi dengan:

```html
<section id="hero">
  <h1>Tentang Kami</h1>
  <p>Informasi tentang tim pengembang web, visi dan misi.</p>
</section>
```

🖼️ **Gambar 6.1** – Tampilan halaman About
![Gambar 6.1](screenshots/gambar6.png)

**Penjelasan:**
Halaman ini menampilkan deskripsi singkat dan contoh portfolio dari pembuat web.

---

### **7️⃣ Membuat Halaman Kontak**

Buat file baru **`kontak.html`**, lalu tambahkan form berikut:

```html
<section id="hero">
  <h1>Hubungi Kami</h1>
  <p>Silakan isi form di bawah ini.</p>
</section>

<form class="contact-form">
  <label for="nama">Nama:</label>
  <input type="text" id="nama" name="nama">

  <label for="email">Email:</label>
  <input type="email" id="email" name="email">

  <label for="pesan">Pesan:</label>
  <textarea id="pesan" name="pesan"></textarea>

  <button type="submit">Kirim Pesan</button>
</form>
```

🖼️ **Gambar 7.1** – Tampilan form kontak
![Gambar 7.1](screenshots/gambar7.png)

**Penjelasan:**
Form digunakan untuk menampung input dari pengunjung, meskipun belum disambungkan ke server.

---

### **8️⃣ Menambahkan Footer**

Tambahkan di bagian paling bawah semua halaman:

```html
<footer>
  <p>&copy; 2025 - Universitas Pelita Bangsa</p>
</footer>
```

🖼️ **Gambar 8.1** – Tampilan footer di bagian bawah halaman
![Gambar 8.1](screenshots/gambar8.png)

**Penjelasan:**
Footer berisi hak cipta atau informasi tambahan.

---

### **9️⃣ Menulis File `style.css`**

Buat file `style.css` di folder yang sama dan isi dengan:

```css
@import url('https://fonts.googleapis.com/css2?family=Open+Sans&display=swap');

* { margin: 0; padding: 0; box-sizing: border-box; }
body {
  font-family: 'Open Sans', sans-serif;
  color: #5a5a5a;
}

#container {
  width: 980px;
  margin: 0 auto;
  box-shadow: 0 0 1em #ccc;
}

/* Header & Nav */
header { padding: 20px; }
nav { background-color: #1f5faa; }
nav a {
  color: white;
  padding: 15px 30px;
  display: inline-block;
  text-decoration: none;
}
nav a.active, nav a:hover { background-color: #2b83ea; }

/* Hero */
#hero {
  background-color: #e4e4e5;
  padding: 50px 20px;
  margin-bottom: 20px;
}

/* Layout */
#main { float: left; width: 640px; padding: 20px; }
#sidebar { float: left; width: 260px; padding: 20px; }
footer {
  clear: both;
  background-color: #1d1d1d;
  color: #eee;
  text-align: center;
  padding: 20px;
}
```

🖼️ **Gambar 9.1** – Hasil layout lengkap setelah CSS diterapkan
![Gambar 9.1](screenshots/gambar9.png)

**Penjelasan:**
CSS di atas mengatur warna, jarak, dan posisi elemen dengan properti **float** dan **width**.
Font menggunakan **Open Sans** dari Google Fonts.

---

## ✅ **Hasil Akhir Layout Web**

| Halaman       | Deskripsi                                      | Screenshot                        |
| ------------- | ---------------------------------------------- | --------------------------------- |
| `home.html`   | Halaman utama berisi hero, konten, dan sidebar | ![Home](screenshots/home.png)     |
| `about.html`  | Halaman tentang dengan deskripsi dan portfolio | ![About](screenshots/about.png)   |
| `kontak.html` | Halaman kontak dengan form isian               | ![Kontak](screenshots/kontak.png) |

---

## 📎 **Kesimpulan**

Dari hasil praktikum ini dapat disimpulkan:

1. Struktur layout web dapat dibuat dengan kombinasi elemen semantik HTML5 dan CSS.
2. Properti **float** dan **width** digunakan untuk mengatur tata letak dua kolom (main dan sidebar).
3. Dengan satu file CSS (`style.css`), tampilan tiga halaman (`home`, `about`, `kontak`) dapat dijaga konsisten.
4. Mahasiswa mampu membuat layout web sederhana yang elegan dan responsif.

---

## 🔗 **Link Repository GitHub**

[👉 https://github.com/username/Lab4Web](https://github.com/username/Lab4Web)
*(Ganti `username` dengan akun GitHub kamu)*

---

## ✨ **Catatan Tambahan**

* Semua file (`home.html`, `about.html`, `kontak.html`, `style.css`) berada di folder yang sama.
* Pastikan URL Google Fonts ditulis satu baris agar tidak error.
* File HTML bisa diuji di browser menggunakan ekstensi **Live Server** pada VS Code.

---

Apakah kamu mau saya bantu **buatkan versi PDF-nya langsung dari laporan ini** (lengkap dengan placeholder gambar dan format rapi siap dikumpulkan)?

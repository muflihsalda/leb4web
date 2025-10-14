# leb4web

# Praktikum 4 - CSS Layout

**Mata Kuliah:** Pemrograman Web  
**Dosen Pengampu:** Agung Nugroho, S.Kom., M.Kom  
**Universitas Pelita Bangsa**  
**Nama:** Muflih Salda Maulana  
**NIM:** 312410527
---

## 🧩 Tujuan Praktikum
1. Mahasiswa mampu memahami struktur dasar pembuatan layout web.
2. Mahasiswa mampu memahami konsep box element (margin, padding, border, content).
3. Mahasiswa mampu menerapkan CSS Float untuk mengatur posisi elemen.
4. Mahasiswa mampu menggunakan elemen semantik HTML5.
5. Mahasiswa mampu membuat layout web sederhana menggunakan CSS.

---

## 📁 Struktur Folder
Lab4Web/
│
├── home.html
├── about.html
├── kontak.html
└── style.css


Semua halaman (`home.html`, `about.html`, dan `kontak.html`) menggunakan file CSS yang sama (`style.css`) agar tampilan konsisten di seluruh halaman.

---

## 🌐 Hasil dan Penjelasan

### 1️⃣ **Halaman Home (`home.html`)**
Halaman utama berisi:
- Header dan navigasi menu.
- Hero section (tampilan banner utama).
- Konten utama (`#main`) dengan tiga box (kolom).
- Sidebar berisi widget link dan text.
- Footer di bagian bawah halaman.

📸 **Screenshot:**
_(tambahkan screenshot tampilan home.html di sini)_

---

### 2️⃣ **Halaman About (`about.html`)**
Berisi:
- Deskripsi singkat tentang website/tim.
- Bagian portfolio dengan tiga project.
- Sidebar berisi informasi tambahan.

📸 **Screenshot:**
_(tambahkan screenshot tampilan about.html di sini)_

---

### 3️⃣ **Halaman Kontak (`kontak.html`)**
Berisi:
- Hero section dengan deskripsi kontak.
- Formulir isian (Nama, Email, Pesan).
- Sidebar berisi informasi kontak (email, telp, alamat).

📸 **Screenshot:**
_(tambahkan screenshot tampilan kontak.html di sini)_

---

## 🎨 **Penjelasan CSS Utama**
Beberapa bagian penting dalam `style.css`:

### 🔹 Reset dan Font
```css
@import url('https://fonts.googleapis.com/css2?family=Open+Sans&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


🔹 Struktur Layout
#container {
  width: 980px;
  margin: 0 auto;
  box-shadow: 0 0 1em #cccccc;
}

🔹 Navigasi
nav {
  background-color: #1f5faa;
}
nav a {
  color: #fff;
  padding: 15px 30px;
  display: inline-block;
  text-decoration: none;
  font-weight: bold;
}
nav a.active,
nav a:hover {
  background-color: #2b83ea;
}

🔹 Hero Panel
#hero {
  background-color: #e4e4e5;
  padding: 50px 20px;
  margin-bottom: 20px;
}

🔹 Main & Sidebar
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

🔹 Footer
footer {
  clear: both;
  background-color: #1d1d1d;
  color: #eee;
  text-align: center;
  padding: 20px;
}

✅ Kesimpulan

Dalam praktikum ini saya telah:

Membuat layout web sederhana menggunakan HTML5 dan CSS.

Menerapkan konsep box model, float, dan clearfix.

Membuat beberapa halaman web terhubung melalui menu navigasi.

Menerapkan gaya yang konsisten melalui satu file CSS (style.css).

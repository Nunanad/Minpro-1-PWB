## Nama : Nanda Pesona Putri
## NIM : 2409116101

# Personal Portfolio Website

Website ini merupakan project portfolio berbasis HTML dan CSS dengan Bootstrap 5 dan Vue JS untuk meningkatkan tampilan dan struktur kode.

Website dibuat sebagai tugas pengembangan web minpro 1.

---

## Teknologi yang Digunakan

- HTML5
- CSS3
- Bootstrap 5
- Vue JS (CDN)

---
## Section Hero

### Tampilan

<img width="1896" height="907" alt="image" src="https://github.com/user-attachments/assets/2fbc943f-9b71-4fe1-a185-862a6caa8790" />

### Penjelasan Code

<img width="1021" height="467" alt="image" src="https://github.com/user-attachments/assets/eef65e6b-511f-4498-b2ff-d16c79533b3c" />

Hero section diawali dengan elemen:

```html
<section class="hero d-flex align-items-center justify-content-center text-center">
```

Class yang digunakan:

- `hero` → class custom untuk styling utama hero section.
- `d-flex` → mengaktifkan Flexbox (Bootstrap).
- `align-items-center` → memposisikan konten secara vertikal di tengah.
- `justify-content-center` → memposisikan konten secara horizontal di tengah.
- `text-center` → membuat teks rata tengah.

---

Di dalamnya terdapat container:

```html
<div class="container">
```

Class `container` dari Bootstrap digunakan untuk menjaga tata letak tetap rapi dan responsif di berbagai ukuran layar.

---

#### Teks Perkenalan

```html
<h4 class="hello-text mb-2">Haloo saya</h4>
```

- `hello-text` → class custom untuk styling teks pembuka.
- `mb-2` → memberikan margin bawah.

---

#### Nama Dinamis

```html
<h1 class="fw-bold display-4">
    <span class="highlight">{{ name }}</span>
</h1>
```

- `fw-bold` → membuat teks menjadi tebal.
- `display-4` → ukuran heading besar (Bootstrap).
- `highlight` → class custom untuk memberi efek warna atau gaya khusus.
- `{{ name }}` → placeholder variabel dinamis (digunakan pada template engine seperti Blade, Vue, atau framework lainnya).

---

#### Deskripsi 

```html
<p class="lead mt-3">
    {{ description }}
</p>
```

- `lead` → membuat paragraf lebih menonjol.
- `mt-3` → memberi margin atas.
- `{{ description }}` → variabel dinamis untuk menampilkan deskripsi profil.

---

#### Tombol Instagram

```html
<a href="https://instagram.com/hi.nnaan"
   target="_blank"
   class="btn calm-btn mt-4">
   instagram
</a>
```

- `href` → mengarah ke akun Instagram.
- `target="_blank"` → membuka link di tab baru.
- `btn` → class tombol Bootstrap.
- `calm-btn` → class custom untuk styling tombol.
- `mt-4` → memberi jarak atas.

---

## Section About Me

### Tampilan

<img width="1890" height="913" alt="image" src="https://github.com/user-attachments/assets/dcd371d0-7c98-4309-9265-2f01753f482b" />

### Penjelasan Code

<img width="961" height="289" alt="image" src="https://github.com/user-attachments/assets/167879a3-2379-4a84-a0d4-6510dd89b5cb" />

Section diawali dengan elemen:

```html
<section id="about" class="about-section py-5">
```

- `id="about"` digunakan sebagai anchor agar dapat diakses melalui navigasi (misalnya melalui link `#about` pada navbar).
- `about-section` merupakan class tambahan untuk styling kustom.
- `py-5` adalah utility class Bootstrap yang memberikan padding vertikal (atas dan bawah).

---

Di dalamnya terdapat container Bootstrap:

```html
<div class="container">
```

Class `container` berfungsi untuk:
- Membatasi lebar konten
- Menjaga tata letak tetap rapi
- Membuat tampilan responsif di berbagai ukuran layar

---

Layout menggunakan sistem grid Bootstrap:

```html
<div class="row align-items-center">
```

- `row` digunakan sebagai pembungkus baris dalam sistem grid.
- `align-items-center` memastikan konten sejajar secara vertikal.

---

Kolom utama untuk teks menggunakan:

```html
<div class="col-md-7">
```

- `col-md-7` berarti kolom mengambil 7 dari total 12 grid pada layar ukuran medium (≥768px) ke atas.
- Pada layar kecil, kolom akan otomatis menyesuaikan menjadi full width (responsif).

---

Judul section:

```html
<h2 class="section-title mb-3">About Me</h2>
```

- `section-title` digunakan untuk styling tambahan.
- `mb-3` memberikan margin bawah agar tampilan lebih rapi.

---

Deskripsi profil:

```html
<p>
Saya adalah mahasiswa Sistem Informasi angkatan 2024
yang mempelajari coding, manajemen database serta analisa sistem.
</p>
```

Elemen `<p>` digunakan untuk menampilkan informasi singkat mengenai latar belakang dan bidang yang dipelajari.

---

## Section Experience

### Tampilan

<img width="1880" height="901" alt="image" src="https://github.com/user-attachments/assets/58524443-6a99-4aec-a0df-ebb9a3f788b4" />

### Penjelasan Code

<img width="1167" height="477" alt="image" src="https://github.com/user-attachments/assets/0da3a0b7-1065-4a01-a163-f905aadaaccf" />

Judul section ditampilkan menggunakan heading:

```html
<h5 class="mt-5 mb-4">Experience</h5>
```

- `mt-5` → memberikan margin atas.
- `mb-4` → memberikan margin bawah.
- Digunakan sebagai penanda awal bagian pengalaman.

---

### Layout Grid

Section menggunakan sistem grid Bootstrap:

```html
<div class="row">
```

- `row` berfungsi sebagai pembungkus baris.
- Setiap pengalaman ditempatkan dalam kolom terpisah agar tersusun rapi.

---

### Experience Card Structure

Setiap item pengalaman menggunakan struktur berikut:

```html
<div class="col-md-6 mb-3">
    <div class="exp-card p-3">
        <h6>Judul Pengalaman</h6>
        <small>Tahun</small>
        <p>Deskripsi singkat pengalaman</p>
    </div>
</div>
```

Penjelasan class yang digunakan:

- `col-md-6` → Membagi layout menjadi 2 kolom pada layar ukuran medium ke atas.
- `mb-3` → Memberikan jarak antar card.
- `exp-card` → Class custom untuk styling kartu pengalaman.
- `p-3` → Memberikan padding di dalam card.
  
---

## Section Certificates

### Tampilan

<img width="1898" height="910" alt="image" src="https://github.com/user-attachments/assets/20aa635f-56af-434c-b167-161450f8932f" />


### Penjelasan Code

<img width="1164" height="574" alt="image" src="https://github.com/user-attachments/assets/7d69ba03-8900-4ece-9807-2576e8ecc412" />

Section diawali dengan elemen:

```html
<section id="certificates" class="cert-section py-5">
```

Penjelasan atribut:

- `id="certificates"` → Digunakan sebagai anchor untuk navigasi (misalnya dari navbar dengan link `#certificates`).
- `cert-section` → Class custom untuk styling khusus bagian sertifikat.
- `py-5` → Utility class Bootstrap untuk memberikan padding vertikal.

---

### Container dan Judul

```html
<div class="container">
    <h2 class="section-title text-center mb-5">Sertifikat</h2>
</div>
```

- `container` → Membatasi lebar konten agar tetap rapi dan responsif.
- `section-title` → Class custom untuk styling judul.
- `text-center` → Membuat teks rata tengah.
- `mb-5` → Memberikan margin bawah agar terdapat jarak dengan konten berikutnya.

---

### Layout Grid

```html
<div class="row">
```

- `row` → Digunakan sebagai pembungkus sistem grid Bootstrap.
- Setiap sertifikat ditempatkan dalam kolom terpisah agar tersusun sejajar.

---

### Struktur Card Sertifikat

Setiap sertifikat menggunakan struktur berikut:

```html
<div class="col-md-4 mb-4">
    <div class="cert-card">
        <img src="images/filename.jpg" class="cert-img" alt="Certificate">
        <div class="p-3">
            <h6>Nama Sertifikat</h6>
            <p>Deskripsi sertifikat</p>
        </div>
    </div>
</div>
```

Penjelasan class:

- `col-md-4` → Membagi layout menjadi 3 kolom pada layar ukuran medium ke atas.
- `mb-4` → Memberikan jarak antar card.
- `cert-card` → Class custom untuk desain card sertifikat.
- `cert-img` → Class custom untuk mengatur tampilan gambar sertifikat.
- `p-3` → Memberikan padding pada bagian deskripsi.

---

## Navbar

### Tampilan

<img width="1898" height="69" alt="image" src="https://github.com/user-attachments/assets/13ffa760-1c96-4feb-8a69-5ebb528928b0" />


### Penjelasan Code

<img width="1093" height="614" alt="image" src="https://github.com/user-attachments/assets/ed3795e8-0fc6-4ccf-9803-f96d478f88d5" />

Navbar diawali dengan elemen:

```html
<nav class="navbar navbar-expand-lg navbar-light fixed-top custom-navbar">
```

Penjelasan class yang digunakan:

- `navbar` → Class dasar komponen navbar Bootstrap.
- `navbar-expand-lg` → Navbar akan dalam keadaan collapse (hamburger menu) pada layar kecil dan melebar penuh pada layar ukuran large (≥992px).
- `navbar-light` → Skema warna terang.
- `fixed-top` → Navbar akan tetap berada di bagian atas saat halaman di-scroll.
- `custom-navbar` → Class tambahan untuk styling kustom.

---

### Container

```html
<div class="container">
```

Digunakan untuk menjaga tata letak navbar tetap rapi dan responsif.

---

### Brand / Logo

```html
<a class="navbar-brand fw-bold" href="#home">NaN</a>
```

- `navbar-brand` → Digunakan untuk menampilkan nama brand atau logo website.
- `fw-bold` → Membuat teks menjadi tebal.
- `href="#home"` → Mengarahkan ke section dengan id `home`.

---

### Navbar Toggler (Hamburger Menu)

```html
<button class="navbar-toggler" type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav">
    <span class="navbar-toggler-icon"></span>
</button>
```

Digunakan untuk menampilkan tombol menu pada perangkat dengan layar kecil.

- `data-bs-toggle="collapse"` → Mengaktifkan fitur collapse Bootstrap.
- `data-bs-target="#navbarNav"` → Menentukan target elemen yang akan dibuka/ditutup.

---

### Menu Navigasi

```html
<div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav ms-auto">
```

- `collapse navbar-collapse` → Mengaktifkan fitur collapse untuk menu.
- `ms-auto` → Menggeser menu ke sisi kanan navbar.

---

### Item Menu

Contoh struktur item menu:

```html
<li class="nav-item">
    <a class="nav-link" href="#home">Beranda</a>
</li>
```

---


### ✔ Bootstrap 5
Digunakan untuk:
- Navbar
- Container
- Grid System (row, col)
- Card layout
- Progress bar
- Responsive design

### ✔ Vue JS
<img width="567" height="205" alt="image" src="https://github.com/user-attachments/assets/638645b0-4df6-45d7-9eb1-4b037af11f49" />


Walaupun data masih bersifat statis, struktur website sudah menggunakan konsep modern reactive system.

---

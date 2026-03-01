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

---

## Section Certificates

### Tampilan
- Layout grid 3 kolom
- Menggunakan card dengan gambar sertifikat
- Hover effect modern
- Background soft pink

### Penjelasan Code
- Menggunakan Bootstrap Grid (`col-md-4`)
- Card custom dengan class `.cert-card`
- Gambar menggunakan `object-fit: cover`
- Responsif mengikuti sistem grid Bootstrap

---

## Navbar

### Tampilan
- Fixed top navigation
- Smooth scroll ke setiap section
- Responsive collapse menu pada tampilan mobile

### Penjelasan Code
- Menggunakan komponen `navbar` Bootstrap 5
- Link menggunakan anchor ke ID section (`#home`, `#about`, `#certificates`)
- Smooth scroll menggunakan `scroll-behavior: smooth;` di CSS

---

## 🦶 Footer

### ✨ Tampilan
- Background soft pink
- Text copyright
- Tema konsisten dengan warna utama website

### 💻 Penjelasan Code
- Menggunakan `<footer>` sederhana
- Styling diatur di `style.css`

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
Digunakan untuk:
- Interpolation `{{ }}`
- Struktur `data()`
- Mounting dengan `.mount('#app')`

Walaupun data masih bersifat statis, struktur website sudah menggunakan konsep modern reactive system.

---

### Dokumentasi


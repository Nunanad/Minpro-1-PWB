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

### Penjelasan Code
- Menggunakan `<section id="home">`
- Interpolation Vue `{{ name }}` dan `{{ description }}`
- Styling menggunakan CSS custom
- Animasi menggunakan `@keyframes` pada CSS
- Tombol menggunakan tag `<a>` agar dapat redirect ke Instagram

---

## Section About Me

### Tampilan


### Penjelasan Code


- Menggunakan `container`, `row`, dan `col-md-` dari Bootstrap
- Skill menggunakan komponen `progress` Bootstrap
- Styling tambahan di file `style.css`
- Responsive design otomatis mengikuti grid Bootstrap

---

## Section Experience

### Tampilan
- Menggunakan card kecil
- Tata letak grid responsif (2 kolom desktop, 1 kolom mobile)
- Hover effect (card naik sedikit)

### Penjelasan Code
- Menggunakan Bootstrap Grid (`row` dan `col-md-6`)
- Card dibuat dengan div custom `.exp-card`
- Efek hover menggunakan `transform` dan `box-shadow`

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


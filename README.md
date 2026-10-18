# 🚀 Portofolio Pribadi - Bootstrap 5

Selamat datang di repository portofolio pribadi saya! Website ini dibangun menggunakan **HTML5** dan **Bootstrap 5 (Offline/Lokal)**. Project ini dibuat untuk melatih pemahaman mengenai pembuatan web yang *responsive*, bersih, dan interaktif.

---

## 🛠️ Teknologi & Fitur
- **HTML5 & CSS3**
- **Bootstrap 5.3** (Offline/Lokal dengan struktur folder `css` dan `js`)
- **Responsive Layout** (Otomatis menyesuaikan di layar HP, Tablet, dan Laptop/PC)
- **Komponen Utama**: Navbar, Hero Section, About Me, Project Cards, Form Kontak, & Footer.

---

## 💡 Rangkuman Konsep Grid Bootstrap 5 (Core Notes)

Catatan penting untuk mengingat logika kerja Grid & Utility Class di Bootstrap 5:

### 1. Rumus Dasar Grid Layout (`Container -> Row -> Col`)
Struktur wajib untuk membuat elemen berdampingan:
- `<div class="container">`: Pembungkus utama agar konten berada di tengah halaman.
- `<div class="row">`: Baris utama yang menampung total **12 slot/kolom**.
- `<div class="col-md-*">`: Kolom di dalam row. Angka di belakang `md` menentukan pembagian slot dari total 12.
  - *Contoh*: `col-md-6` (50% lebar), `col-md-4` (33% lebar), `col-md-2` (17% lebar). Total: $6 + 4 + 2 = 12$.

### 2. Responsif Otomatis (Tanpa `@media` manual)
- Prefix `-md-` menandakan aturan kolom aktif di layar **Medium (Tablet/Laptop $\ge 768px$)** ke atas.
- Di layar HP/layar kecil, elemen otomatis menjadi **lebar 100% (turun vertikal ke bawah)** secara rapi tanpa perlu menulis `@media query` manual.

### 3. Utility Classes Paling Sering Dipakai
- **Gutter (Jarak antar kolom/card)**: `g-4` pada elemen `row` untuk memberi sela antar-card secara otomatis.
- **Padding & Margin**: `py-*` (Padding atas-bawah), `my-*` (Margin atas-bawah), `mt-*`, `mb-*`.
- **Flexbox**: `d-flex`, `justify-content-between`, `align-items-center`, `gap-*`.
- **Tipografi**: `fw-bold` (Menebalkan teks / *font-weight*).
- **Garis Bawah Hiasan**:
  ```html
  <div class="border-bottom border-primary border-3 w-25 mx-auto mt-2"></div>
# LaraPress - Aplikasi Blog Sederhana

LaraPress adalah aplikasi blog sederhana yang dibangun menggunakan Laravel 12 untuk tujuan pembelajaran dan pengembangan keterampilan web development.

[Tampilan Halaman Utama LaraPress]<img width="1920" height="1080" alt="Screenshot 2025-10-03 103630" src="https://github.com/user-attachments/assets/bd717dca-9581-4a92-a823-7564f926623d" />
*Tampilan halaman utama LaraPress*

## 📋 Tentang Proyek

Proyek ini dibuat sebagai bagian dari pembelajaran Laravel framework. LaraPress mendemonstrasikan konsep-konsep dasar Laravel seperti routing, views, dan struktur MVC.

## 🚀 Fitur yang Sudah Diimplementasikan

### 1. **Halaman Utama (Welcome Page)**
   - Mengubah tampilan default Laravel menjadi halaman sederhana
   - Menampilkan judul "Selamat Datang di LaraPress"
   - Struktur HTML yang bersih dan minimal

### 2. **Halaman Tentang Kami**
   - Route: `/tentang-kami`
   - Menampilkan informasi tentang LaraPress
   - Menjelaskan tujuan proyek sebagai pembelajaran Laravel 12

## 📁 Struktur File yang Dimodifikasi

### File yang Dibuat/Dimodifikasi:

1. **`resources/views/welcome.blade.php`**
   - Mengubah tampilan default Laravel yang kompleks menjadi struktur HTML sederhana
   - Menampilkan pesan sambutan untuk pengunjung blog

2. **`resources/views/about.blade.php`** (BARU)
   - File view baru untuk halaman "Tentang Kami"
   - Berisi informasi tentang LaraPress sebagai proyek pembelajaran

3. **`routes/web.php`**
   - Menambahkan route baru `/tentang-kami` yang mengarah ke view `about.blade.php`

## 🛠️ Langkah-langkah Implementasi

### Step 1: Modifikasi Halaman Welcome
Mengubah file `resources/views/welcome.blade.php` dari tampilan default Laravel (266 baris) menjadi HTML sederhana:

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Datang di LaraPress</title>
</head>
<body>
    <h1>Selamat Datang di Blog LaraPress</h1>
    <p>Ini adalah halaman utama dari aplikasi blog kita.</p>
</body>
</html>
```

### Step 2: Membuat Route Baru
Menambahkan route baru di `routes/web.php`:

```php
Route::get('/tentang-kami', function () {
    return view('about');
});
```

### Step 3: Membuat View About
Membuat file baru `resources/views/about.blade.php`:

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tentang Kami - LaraPress</title>
</head>
<body>
    <h1>Tentang LaraPress</h1>
    <p>LaraPress adalah aplikasi blog sederhana yang dibuat dengan Laravel 12.</p>
    <p>Proyek ini dibuat untuk tujuan pembelajaran dan pengembangan keterampilan.</p>
</body>
</html>
```

## 🌐 Endpoint yang Tersedia

| Route | Method | Deskripsi |
|-------|--------|-----------|
| `/` | GET | Halaman utama LaraPress |
| `/tentang-kami` | GET | Halaman tentang LaraPress |

## 💻 Teknologi yang Digunakan

- **Framework**: Laravel 12
- **PHP Version**: 8.x
- **Database**: SQLite (default)
- **Frontend**: Blade Template Engine, HTML, CSS
- **Build Tool**: Vite

## 📸 Screenshot

### Halaman Utama
[Halaman Utama]<img width="1920" height="1080" alt="Screenshot 2025-10-03 104156" src="https://github.com/user-attachments/assets/f80770a5-312b-4eff-987a-704664144709" />
Halaman utama menampilkan sambutan sederhana kepada pengunjung blog LaraPress.

### Kesimpulan
Pada praktikum ini kita telah:
 - Menginstal proyek Laravel baru menggunakan Composer.
 - Menjalankan server lokal dengan perintah php artisan serve.
 - Mengenal struktur folder dasar Laravel, terutama routes/web.php untuk rute dan resources/views/ untuk tampilan.
 - Membuat halaman statis dengan cara mendefinisikan route di web.php dan membuat file view (Blade).
 - Menghubungkan antar halaman dengan menambahkan link navigasi.
 - Menerapkan siklus kerja dasar Laravel yaitu Request → Route → View → Response.

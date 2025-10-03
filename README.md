# 📘 Praktikum Laravel 1 - Instalasi, Konfigurasi, dan Halaman Pertama  

## ✨ Langkah Pengerjaan

### 1. Instalasi Proyek Laravel Baru
- Pastikan sudah ada **Composer** dan server lokal (Laragon/XAMPP).  
- Buka terminal lalu arahkan ke direktori web server, misalnya:
  ```bash
  cd C:\laragon\www
  ```
- Jalankan perintah instalasi:
  ```bash
  composer create-project laravel/laravel LaraPress
  ```

### 2. Menjalankan Server Development
- Masuk ke folder proyek:
  ```bash
  cd LaraPress
  ```
- Jalankan server bawaan Laravel:
  ```bash
  php artisan serve
  ```
- Akses di browser: [http://127.0.0.1:8000](http://127.0.0.1:8000)

### 3. Membuat dan Memodifikasi View
- Buka proyek di VS Code.  
- Edit file `resources/views/welcome.blade.php` agar menampilkan halaman utama sederhana.  

### 4. Menambahkan Halaman "Tentang Kami"
- Tambahkan route di `routes/web.php`:
  ```php
  Route::get('/tentang-kami', function () {
      return view('about');
  });
  ```
- Buat file `resources/views/about.blade.php` dengan isi HTML tentang LaraPress.  
- Tambahkan navigasi antar halaman (`welcome` <-> `about`).  

### 5. Membuat Halaman "Kontak" (Tugas Mandiri)
- Tambahkan route baru di `routes/web.php`:
  ```php
  Route::get('/kontak', function () {
      return view('kontak');
  });
  ```
- Buat file `resources/views/kontak.blade.php` berisi informasi kontak fiktif (email & nomor telepon).  
- Tambahkan link navigasi ke halaman lain (`welcome` ↔ `about` ↔ `kontak`).  

---
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/5c539a82-100a-4df0-9af4-e0047a82df79" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c8755d47-4b98-4fc4-a3cb-fc664fe88896" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b6739ae0-ee5a-443f-b910-0c2ef2559c3c" />


## ✅ Kesimpulan
Pada praktikum ini, kita telah berhasil:
- Menginstal dan menjalankan proyek Laravel baru dari awal.  
- Menjalankan server development lokal dengan `php artisan serve`.  
- Memahami alur dasar Laravel: **Request → Route → View → Response**.  
- Membuat halaman statis sederhana (`welcome`, `tentang kami`, dan `kontak`) serta menghubungkannya dengan navigasi.  

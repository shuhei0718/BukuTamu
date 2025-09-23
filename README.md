# 📖 Zie Buku Tamu

[![PHP](https://img.shields.io/badge/PHP-7%20%2F%208-blue?logo=php)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/Database-MySQL%2FMariaDB-orange?logo=mysql)](https://www.mysql.com/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-4-purple?logo=bootstrap)](https://getbootstrap.com/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

Sebuah aplikasi **Buku Tamu Digital** berbasis web menggunakan **PHP + MySQL** dengan tampilan modern dari **SB Admin 2**.  
Aplikasi ini memungkinkan pencatatan tamu, manajemen data, hingga pembuatan laporan dalam format **Excel** menggunakan **PhpSpreadsheet**.

---

## 🚀 Fitur Utama

### 🔐 Autentikasi Login
- Akses aplikasi hanya untuk user yang login  
- Session management untuk keamanan  

### 📑 Manajemen Buku Tamu
- Tambah, ubah, dan hapus data tamu  
- Data yang disimpan meliputi:  
  - Tanggal kunjungan  
  - Nama tamu  
  - Alamat  
  - Nomor HP/Telp  
  - Bertemu dengan  
  - Kepentingan  

### 📊 Laporan Tamu
- Filter laporan berdasarkan periode tanggal  
- Data laporan ditampilkan dalam tabel interaktif  
- Ekspor laporan ke file **Excel** dengan sekali klik  

### 🎨 UI Modern
- Menggunakan template **SB Admin 2 (Bootstrap 4)**  
- Sidebar navigasi responsif (dengan toggle untuk desktop & mobile)  
- Tabel interaktif dengan **DataTables**  

---

## 🛠️ Teknologi yang Digunakan
- **Backend:** PHP 7 / 8  
- **Database:** MySQL / MariaDB  
- **Frontend:** Bootstrap 4 (SB Admin 2 Template)  
- **Library:**  
  - [PhpSpreadsheet](https://phpspreadsheet.readthedocs.io/) → ekspor laporan ke Excel  
  - [FontAwesome](https://fontawesome.com/) → ikon  
  - [jQuery](https://jquery.com/) & [DataTables](https://datatables.net/) → tabel interaktif  

---

## 📂 Struktur Folder Utama

```bash
Rafa_Buku_Tamu/
├── assets/                 # CSS, JS, gambar
│   ├── css/                # Custom CSS (sb-admin-2.min.css, dll.)
│   ├── js/                 # Script utama (sb-admin-2.min.js, dll.)
│   ├── vendor/             # Library tambahan (Bootstrap, FontAwesome, DataTables)
├── templates/              # Template header & footer
├── vendor/                 # Composer packages (PhpSpreadsheet, dll.)
├── connection.php          # Koneksi database
├── function.php            # Fungsi helper (query, tambah data, dll.)
├── login.php               # Halaman login
├── logout.php              # Logout & destroy session
├── index.php               # Dashboard
├── buku-tamu.php           # CRUD buku tamu
├── users.php               # Manajemen user
├── laporan.php             # Halaman laporan tamu
├── export-laporan.php      # Export laporan ke Excel
└── composer.json           # Konfigurasi Composer



## 📊 Alur Aplikasi

1. **Login**  
   - User masuk menggunakan username & password  
   - Jika berhasil → diarahkan ke Dashboard  

2. **Dashboard**  
   - Menampilkan ringkasan data tamu  

3. **Buku Tamu**  
   - CRUD data tamu (tambah, ubah, hapus)  

4. **Laporan**  
   - User pilih periode tanggal  
   - Data ditampilkan dalam tabel  
   - Klik **Export to Excel** → generate file `Laporan Buku Tamu.xlsx`  

---

## ⚡ Instalasi & Setup

1. **Clone project**
   ```bash
   git clone https://github.com/username/Rafa_Buku_Tamu.git
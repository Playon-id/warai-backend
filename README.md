# Warai
**Warai** merupakan aplikasi yang bisa digunakan untuk orang tua atau wali murid yang membutuhkan pendamping belajar bagi anak-anaknya. Kami menggunakan [**Laravel Starter**](https://github.com/nasirkhan/laravel-starter) dalam project awal aplikasi ini.


# Demo
Periksa proyek demo berikut. Ini hanya instalasi langsung dari proyek tanpa modifikasi apa pun.

Demo URL: menyusul

```
User: super@admin.com
Pass: secret

User: user@user.com
Pass: secret

```

# Perintah Kustom

Kami telah membuat sejumlah perintah khusus untuk proyek tersebut. Perintah-perintah tersebut didaftar di bawah ini dengan penjelasan singkat tentang penggunaannya.

## Hapus Semua Cache

`composer clear-all`

ini adalah perintah pintas, hapus semua cache termasuk konfigurasi, rute, dan lainnya

## Perbaikan Gaya Kode

`composer fix-cs`

terapkan perbaikan gaya kode dengan perintah ini.


# Fitur

The `Laravel Starter` dilengkapi dengan sejumlah fitur yang paling umum di hampir semua aplikasi. Ini adalah proyek templat yang artinya dimaksudkan untuk dibangun sedemikian rupa sehingga dapat digunakan untuk proyek lain.

Ini adalah aplikasi modular, dan sejumlah modul diinstal secara default. Akan sangat membantu jika menggunakannya sebagai dasar untuk aplikasi di masa mendatang.

* Fitur Admin dan pandangan masyarakat yang sepenuhnya terpisah sebagai `Backend` dan `Frontend` namespace.
* Fitur utama dikembangkan sebagai `Modules`. Modul seperti Pos, Komentar, Tag dipisahkan dari fitur inti seperti Pengguna, Peran, Izin


## Fitur Admin

* User Authentication
* Social Login
  * Google
  * Facebook
  * Github
  * Build in a way adding more is much easy now
* User Profile with Avatar
  * Separate User Profile table
* Role-Permissions for Users
* Dynamic Menu System
* Language Switcher
* Localization enable across the porject
* Backend Theme
  * Bootstrap 4, CoreUI
  * Fontawesome 5
* Frontend Theme
  * Bootstrap 4, Now UI Kit
  * Fontawesome 5
* Article Module
  * Posts
  * Categories
  * Tags
  * Comments
  * wysiwyg editor
  * File browser
* Application Settings
* External Libraries
  * Bootstrap 4
  * Fontawesome 5
  * CoreUI
  * Now UI Kit
  * Datatables
  * Select2
  * Date Time Picker
* Backup (Source, Files, Database as Zip)
* Log Viewer
* Newsletter
* Notification
  * Dashboard and details view
* RSS Feed

## Fitur Inti yang akan dibuat
* Module Parent
* Module Teacher
* Module Order

# Panduan pengguna

## Instalasi

Ikuti langkah-langkah yang disebutkan di bawah ini untuk menginstal dan menjalankan proyek.

1. Gandakan atau unduh repositori
2. Buka direktori proyek dan jalankan `composer install`
3. Buat `.env` file dengan menyalin `.env.example`. Anda dapat menggunakan perintah untuk melakukan itu `cp .env.example .env`
4. Perbarui nama database dan kredensial dalam `.env` file
5. Jalankan perintahnya `php artisan migrate --seed`
6. Tautan direktori penyimpanan: `php artisan storage:link`
7. Setelah selesai dengan langkah di atas maka buat dulu key supaya website tidak error gateway `php artisan key:generate`. maka bisa di lihat dibagian file `.env` maka code `APP_KEY=base64:` akan terisi dengan sebuah token.
8. Anda dapat membuat entri virtualhost untuk mengakses aplikasi atau menjalankan `php artisan serve` dari root proyek dan mengunjungi `http://127.0.0.1:8000`

*Setelah membuat izin baru, gunakan perintah berikut untuk memperbarui izin yang diuangkan.*

`php artisan cache:forget spatie.permission.cache`


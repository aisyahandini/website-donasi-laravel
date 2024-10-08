<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/webiste-donasi-laravel/assets/142916107/8b668175-edfd-4b37-9bb5-291754cd53c2">
  <source media="(prefers-color-scheme: light)" srcset="https://github.com/webiste-donasi-laravel/assets/142916107/ea92ccf0-55e3-49bc-b743-78a1df2cffd3">
  <img alt="Header" height="80" >
</picture>
</div>

<img src="https://github.com/webiste-donasi-laravel/assets/142916107/cbff83f0-c91c-4291-9f02-9463e4533380" width="100%" height="2px"/>
<p/>

Website ini adalah platform donasi yang dikembangkan menggunakan Laravel 11. Proyek ini merupakan bagian dari tugas akhir mata kuliah Pemrograman Web Universitas Negeri Padang dengan berfokus pada implementasi fungsi CRUD (Create, Read, Update, Delete).

## 【 Daftar Isi 】

-   [Fitur-Fitur](#fitur)
-   [Tools yang Digunakan](#tools)
-   [Instalasi](#instalasi)
-   [Menjalankan Aplikasi](#jalankan)
-   [Konfigurasi Gambar](#konfigurasi)
-   [Kredit](#kredit)
-   [About & Help](#about)

<!------------>
</br>

## <a id="fitur"></a>【 Fitur-Fitur 】

-   **Halaman Donasi**: Pengguna dapat melihat jumlah donasi yang terkumpul.
-   **Halaman Pembayaran**: Pengguna dapat memberikan donasi berupa nama, pesan, jumlah, dan jenis pembayaran.
-   **Halaman List Donatur**: Pengguna dapat melihat list pengguna yang telah berdonasi.
-   **Autentikasi Pengguna**: Registrasi dan login pengguna.
-   **Dashboard Admin**: Panel untuk mengelola donasi dan pengguna.
-   **CRUD Donasi**: Pengelolaan data donasi (Create, Read, Update, Delete).

<!------------>
</br>

## <a id="tools"></a>【 Tools yang Digunakan 】

-   **Framework**: Laravel 11
-   **Database**: MySQL
-   **Dependency Manager**: Composer
-   **Front-end**: Blade Template Engine, Bootstrap

<!------------>
</br>

## <a id="screenshot"></a>【 Screenshot 】


<!------------>
</br>

## <a id="instalasi"></a>【 Instalasi 】

Setelah Anda melakukan cloning atau mengunduh secara manual repositori ini, jalankan prompt-prompt ini berikut pada terminal agar proyek dapat dijalankan:

1. Clone repositori ini ke lokal Anda (skip step ini jika Anda mengunduh secara manual):
    ```bash
    git clone https://github.com/SirGhazian/website-donasi-laravel.git
    ```
2. Buka folder repository yang telah diclone:
    ```bash
    cd website-donasi-laravel
    ```
3. Instal dependensi PHP menggunakan Composer:
    ```bash
    composer install
    ```
4. Ubah nama file `.env.example` menjadi `.env` dan sesuaikan line 22-27:
    ```bash
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=donasi_database
    DB_USERNAME=root
    DB_PASSWORD=
    ```
5. Migrasi database (Saat diminta konfirmasi, enter `yes`)
    ```bash
    php artisan migrate
    ```
6. Buat seed database untuk akun login
    ```bash
    php artisan db:seed AkunLogin
    ```
7. Buat seed database untuk list donatur
    ```bash
    php artisan db:seed ListDonatur
    ```
8. Generate application key:
    ```bash
    php artisan key:generate
    ```

<!------------>
</br>

## <a id="jalankan"></a>【 Menjalankan Aplikasi 】

Setelah berhasil melakukan step-step instalasi diatas, sekarang jalankan aplikasi dengan prompt:

1. Jalankan server pengembangan Laravel:
    ```bash
    php artisan serve
    ```
2. Buka browser dan buka link:
    ```bash
    http://localhost:8000
    ```

<!------------>
</br>

## <a id="konfigurasi"></a>【 Konfigurasi Aset Gambar 】

Untuk mengubah gambar seperti gambar header, banner, logo, ikon web, dan lainnya, Anda perlu mengikuti langkah-langkah konfigurasi berikut:

1. **Header dan Banner:**
   - Pastikan gambar yang akan digunakan memiliki resolusi dan proporsi yang sesuai dengan desain halaman web Anda.
   - Letakkan gambar pada folder public/image

2. **Ikon Web & Logo:**
   - Persiapkan gambar logo dalam format yang mendukung transparansi jika diperlukan (misalnya PNG dengan latar belakang transparan).
   - Pada direktori resource/views/layouts/header.blade.php, ubah link rel ikon pada tag <head>
   - Pada direktori resource/views/layouts/header.blade.php, ubah link href logo navbar pada tag <nav>

Pastikan untuk menguji setiap perubahan gambar untuk memastikan bahwa mereka sesuai dengan estetika dan tujuan situs web Anda. Perubahan ini tidak hanya mempengaruhi penampilan visual situs web Anda tetapi juga dapat memengaruhi pengalaman pengguna secara keseluruhan.

<!------------>
</br>

## <a id="kredit"></a>【 Kredit 】

Gambar-gambar tertentu diambil dari Google Images dan merupakan hak cipta dari pemiliknya masing-masing. Gambar-gambar ini digunakan hanya untuk tujuan ilustratif. Beberapa gambar yang digunakan dalam proyek ini diambil dari sumber-sumber berikut:

-   Sabang Merauke NEWS
-   Tempo Co
-   Deras Id

<!------------>
</br>

## <a id="about"></a>【 About and Help 】



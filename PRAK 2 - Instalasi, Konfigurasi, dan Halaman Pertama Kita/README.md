<h1>Pertemuan Laravel 1 - (request -> root -> view -> response)</h1>
<h2>Nama : Muhammad Zaidan Ahbab</h2>
<h2>NPM  : 4523210081</h2>

<h3>1. Instalasi Laravel</h3>
1. Install laravel sesuai dengan os masing-masing.


<img width="616" height="125" alt="image" src="https://github.com/user-attachments/assets/bb7ac2ad-7269-4ce4-a296-4a3addd0469c" />


2. "composer global require laravel/installer"

<h3>2. Install XAMPP</h3>
1. Install XAMPP sesuai dengan os masing-masing.

<img width="641" height="360" alt="image" src="https://github.com/user-attachments/assets/3e211bf9-96a8-480e-bfc9-5bb62f512210" />


<h3>3. Install project laravel "LaraPress"</h3>
1. Buka terminal, arahnya ke folder root XAMPP. Untuk XAMPP, C:\xampp\htdocs. untuk di linux /opt/lampp/htdocs

2. Jalankan perintah berikut, untuk menginstall project laravel "LaraPress", "composer create-project laravel/laravel LaraPress"

3. Masuk ke dalam folder LaraPress, "cd LaraPress"

4. Jalankan server artisan, "php artisan serve"

5. Muncul IP di terminal, buka di browser, biasanya "http://127.0.0.1:8000"

6. Muncul tampilan utama Laravel

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e5b8e4be-3b0b-43b3-9adb-3042dca170d8" />

7. Buka roject di code editor, contoh VSCODE

8. Masuk ke resources/views/welcome.blade.php, kemudian ubah HTML nya seperi berikut

    ```<!DOCTYPE html>
    <html>
    <head>
        <title>Selamat Datang di LaraPress</title>
    </head>
    <body>
        <h1>Selamat Datang di Blog LaraPress</h1>
        <p>Ini adalah halaman utama dari aplikasi blog kita.</p>
    </body>
    </html>

9. Tampilan utama laravel akan berubah.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7825b413-2a44-4104-8366-689c42f72876" />


10. Tambahkan halaman statis baru, buat route baru di routes/web.php, tambah kan di paling bawah

    ```Route::get('/tentang-kami', function () {
    return view('about'); // Kita akan menampilkan view bernama 'about'

11. Tambah view baru, sama seperti di atas, ada di resources/views, buat file baru, about.blade.php, isinya ini

    ```<!DOCTYPE html>
    <html>
    <head>
        <title>Tentang Kami - LaraPress</title>
    </head>
    <body>
        <h1>Tentang LaraPress</h1>
        <p>LaraPress adalah sebuah proyek blog sederhana yang dibuat untuk mempelajari dasar-dasar framework Laravel 12.</p>
    </body>
    </html>

12. Buka http://127.0.0.1:8000/tentang-kami. maka tampilan akan berubah menjadi Tentang LaraPress
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2dccb8ce-9a68-4cf0-a7fe-d3becfc1a93f" />

13. Tambahkan link navigasi agar bisa pindah halaman.
    ```- Di welcome.blade.php, tambahkan di bawah paragraf: <a href="/tentang-kami">Lihat Halaman Tentang Kami</a>
    - Di about.blade.php, tambahkan di bawah paragraf: <a href="/">Kembali ke Halaman Utama</a>

<h3>4. Tugas membuat halaman statis kontak</h3>
1. Buat route dan views baru

  Route::get('/kontak', function () {
    return view('kontak');
});

  ```<!DOCTYPE html>
  <html>
  <head>
      <title>Kontak Kami - LaraPress</title>
  </head>
  <body>
      <h1>Kontak LaraPress</h1>
      <p>Nama : Muhammad Zaidan Ahbab</p>
      <p>NPM : 4523210081</p>
      <p>Email : jedan4523081@univpancasila.ac.id</p>
      <p>No.Hp : 085813334673</p>
      <a href="/">Kembali ke Halaman Utama</a>
      <a href="/tentang-kami">Lihat Halaman Tentang Kami</a>
  </body>
  </html>
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ce54956e-3f14-4692-ae7b-43251d1336d9" />


<H1>Muhammad Zaidan Ahbab 4523210081</H1>
<h2>Laporan PRAK 1 - GIT & GITHUB</h2>
<h3>1. Download dan Install Git Dari Link Berikut https://git-scm.com/download/win</h3>
<img width="1920" height="1080" alt="Screenshot 2025-09-26 093006" src="https://github.com/user-attachments/assets/c0b16972-45b5-42e6-a619-6be5b15b1031" />

- jalankan file .exe yang sudah didownload

- ikuti settingan default, klik "next" hingga selesai

- buka git bash, cek versi git "git --version"
<img width="581" height="370" alt="Screenshot 2025-09-26 093812" src="https://github.com/user-attachments/assets/404ef774-0b37-484e-9163-9a138527773a" />

<h3>2. Konfigurasi Awal (Wajib)</h3>
- masih di Git Bash, jalankan perintah berikut untuk menghubungkan ke github, sesuaikan username dan email dengan github masing-masing

git config --global user.name "Nama Kamu"

git config --global user.email "email@kamu.com"

<h3>3. Kerja Dasar GIT (Lokal)</h3>
- pilih folder dimana ingin menyimpan folder praktikum

- membuat folder, "mkdir proyek-web"

- masuk ke folder proyek web, "cd proyek-web"

- inisialisasi git, "git init"

- buat file, contoh index.html dan style.css

- cek status, "git status", akan merah

- "git add ."

- "git status", akan hijau

- "git commit -m 'pesan commit'"

- buat branch baru, "git checkout -b fitur-kontak"

- buat file baru, contoh kontak.html

- "git add ."

- "git commit -m 'pesan commit'"

- kembali ke branch awal, di kasus saya master "git checkout master"

- satukan kedua branch, "git merge fitur-kontak"

<h3>4. Integrasi dengan GitHub</h3>
- Buat repository baru, copy link repo yang berakhiran .git

- git remote add origin https://github.com/NamaUserKamu/proyek-web-pertama.git <- link ini sesuaikan dengan link yang dicopy

- git branch -M main

- git push -u origin main
<img width="1920" height="1080" alt="Screenshot 2025-09-26 092658" src="https://github.com/user-attachments/assets/24ab91ac-6141-4256-a39c-684861f3a0e7" />

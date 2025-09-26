<h1>MUHAMMAD ZAIDAN AHBAB 4523210081</h1>

<h2>Laporan Instalasi GIT Pertemuan Pertama</h2>

<h3>1. Download GIT dari link berikut https://git-scm.com/download/win</h3>

<img width="1920" height="1080" alt="Screenshot 2025-09-26 093006" src="https://github.com/user-attachments/assets/7995963e-9f2d-440a-b1bd-09fd12d3f03a" />

- jalankan file .exe
- biarkan pengaturan default lalu klik "next" sampai selesai
- buka Git Bash, cek versi git, "git --version"

<img width="581" height="370" alt="image" src="https://github.com/user-attachments/assets/cb1541b2-4681-4a50-8553-82fc3a08e003" />

<h3>2. Config Awal (wajib)</h3>

- masih di Git Bash, jalankan perintah berikut dengan username dan email sesuai dengan github masing-masing

git config --global user.name "Nama Kamu"

git config --global user.email "email@kamu.com"

<img width="581" height="370" alt="image" src="https://github.com/user-attachments/assets/c870d8a3-f506-4f09-b175-1de904bc9bb5" />

<h3>3. Membuat Folder Lokal di Git Bash</h3>

- masuk ke folder dimana folder praktikum ingin dibuat, berpindah folder di Git Bash menggunakan cd

- kemudian membuat folder, mkdir proyek-web

- masuk ke dalam folder proyek-web, cd proyek-web

- git init, untuk inisialisasi git agar terhubung ke folder tersebut

- buat beberapa file, contohnya index.html dan style.css

- git add .

- git commit -m "pesan commit"

- git checkout -b fitur-kontak, untuk bikin branch baru

- setiap ada perubahan, lakukan git add . dan git commit -m "pesan commit"

- git checkout master, balik ke branch utama yaitu master

- git merge fitur-kontak, untuk menyatukan kedua branch

<h3>4. Buat Repository di Github, dan Hubungkan dengan Git</h3>

- git remote add origin https://github.com/NamaUserKamu/proyek-web-pertama.git <- ini dari link git repository masing masing

- git branch -M master

- git push -u origin master

<img width="1920" height="1080" alt="Screenshot 2025-09-26 092658" src="https://github.com/user-attachments/assets/77daa871-38d4-4cb8-a02d-2f8ebef88aa4" />


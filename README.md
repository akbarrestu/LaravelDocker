# LaravelDocker
Disini saya akan mendemokan build aplikasi web <b>Laravel</b> dengan database dan webserver yang akan dijalankan melalui <b>Docker</b> 

## Build app

Kita mempunyai 3 images didalam file <b>docker-compose.yml</b> yaitu :
- app (Aplikasi)
- mysql:5.7 (Database)
- nginx:alpine (Webserver)

Kita menggunakan perintah <b>docker-compose build app</b> untuk menjalankan semua image atau container secara bersamaan.
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/1.png"/>
## Jalankan Environment dibelakang layar

Agar Container berjalan dibelakang layar kita gunakan perintah <b>docker-compose up -d</b>

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/2.png"/>

## Melihat Service yang sedang berjalan

Kita gunakan perintah <b>docker-compose ps</b> untuk melihat service yang sedang berjalan.

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/3.png"/>

Untuk melihat service yang berjalan, kita juga bisa melihat langsung pada aplkasi docker desktop

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/a.png"/>

## Eksekusi perintah dalam Container

<b>docker-compose exec app ls -l</b>

Kita dapat menggunakan perintah <b>docker-compose exec</b> untuk mengeksekusi perintah didalam container.  kemudian dapat kita tambahkan <b>ls -l</b> untuk menampilkan informasi detail tentang file di direktori aplikasi.

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/4.png"/>

## Composer Install

<b>docker-compose exec app composer install</b>

<b>Composer install</b> digunakan untuk menginstal dependensi aplikasi. Digunakan oleh developer saat membuat web dengan Laravel

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/5.png"/>

## Membuat Key

<b>docker-compose exec app php artisan key:generated</b>

Pada Laravel, Key di generated untuk enkripsi session pengguna dan data sensitif
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/6.png"/>

## Jalankan Aplikasi

Disini kita menjalankan aplikasi sesuai dengan port yang ada pada webserver yaitu localhost:5000
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/7.png"/>



<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/8.png"/>

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/9.png"/>

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/10.png"/>

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/11.png"/>

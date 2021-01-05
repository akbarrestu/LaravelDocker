# LaravelDocker
Saya membangun aplikasi web <i>Laravel</i> dengan menggunakandatabase dan webserver yang akan dijalankan melalui <i>Docker</i> 

## Build app

Saya mempunyai 3 images didalam file <b>docker-compose.yml</b> yaitu :
- app (Aplikasi)
- mysql:5.7 (Database)
- nginx:alpine (Webserver)

Untuk menjalankan semua image atau container secara bersamaan gunakan perintah <b>docker-compose build app</b>.
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/1.png"/>
## Jalankan Environment dibelakang layar

Gunakan <b>docker-compose up -d</b> untuk menjalankan container di latar belakang

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/2.png"/>

## Melihat Service yang sedang berjalan

Untuk melihat service yang sedang berjalan gunakan perintah <b>docker-compose ps</b>.

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/3.png"/>

Untuk melihat service yang berjalan, kita juga bisa melihat langsung pada aplkasi docker desktop

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/a.png"/>

## Eksekusi perintah dalam Container

<b>docker-compose exec app ls -l</b>

Gunakan perintah <b>docker-compose exec</b> untuk mengeksekusi perintah didalam container.  
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/4.png"/>

## Composer Install

<b>docker-compose exec app composer install</b>

Gunakan <b>Composer install</b> untuk menginstal dependensi aplikasi. Digunakan oleh user saat membuat web dengan Laravel

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/5.png"/>

## Membuat Key

<b>docker-compose exec app php artisan key:generated</b>

Pada Laravel, Key di generated digunakan untuk enkripsi session pengguna .
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/6.png"/>

## Jalankan Aplikasi

Jalankan aplikasi sesuai dengan port yang ada pada webserver yaitu localhost:5000
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/7.png"/>


## tampilan muka
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/8.png"/>

## create data
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/9.png"/>

## edit data
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/12.png"/>

## tampil data
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/13.png"/>

## push docker hub
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/14.png"/>

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/15.png"/>

<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/16.png"/>

## tampilan pada repository docker
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/17.png"/>

## Tampilan pull di kata koda
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/18.png"/>





# LaravelDocker
Disini saya akan mendemokan build aplikasi web <b>Laravel</b> dengan database dan webserver yang akan dijalankan melalui <b>Docker</b> 

## Build app

Kita mempunyai 3 images didalam file <b>docker-compose.yml</b> yaitu :
- app (Aplikasi)
- mysql:5.7 (Database)
- nginx:alpine (Webserver)

Kita menggunakan perintah <b>docker-compose build app</b> untuk menjalankan semua image atau container secara bersamaan.
<img src="https://github.com/akbarrestu/LaravelDocker/blob/master/1.png"/>

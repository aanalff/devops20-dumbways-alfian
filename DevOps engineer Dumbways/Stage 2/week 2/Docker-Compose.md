1. Docker and Docker Compose

Description

Sebelum mengerjakan tugas, mohon persiapkan :

- Akun Github dan buat repository dengan judul "devops20-dumbways-<nama kalian>"
- Gunakan file README.md untuk isi tugas kalian
- Buatlah langkah-langkah pengerjaan tugas beserta dokumentasinya
- Gunakan vm Appserver kalian diskusikan saja ingin menggunakan vm siapa di dalam team

Repository && Reference:
- Housy Backend
- Housy Frontend
- Certbot
- PM2 Runtime With Docker
- Cloudflare
- Wildcard SSL

# Tasks :
[ Docker ]

- Jelasakan langkah-langkah melakukan rebuild server BiznetGio, dan ubah menggunakan os ubuntu 22
- Setelah server sudah selesai ter rebuild, buatlah suatu user baru dengan nama team kalian
- Buatlah bash script se freestyle mungkin untuk melakukan installasi docker.
- Deploy aplikasi Web Server, Frontend, Backend, serta Database on top docker compose
- Buat suatu docker compose yang berisi beberapa service kalian
 Web Server
 Frontend
 Backend
 Database
- Di dalam docker-compose file buat suatu custom network dengan nama team kalian, lalu pasang ke setiap service yang kalian miliki.
- Deploy database terlebih dahulu menggunakan mysql dan jangan lupa untuk pasang volume di bagian database.
- Untuk building image frontend dan backend sebisa mungkin buat dockerized dengan image sekecil mungkin. dan jangan lupa untuk sesuaikan configuration dari backend ke database maupun frontend ke backend sebelum di build menjadi docker images.
- Untuk Web Server buatlah configurasi reverse-proxy menggunakan nginx on top docker.
- SSL CLOUDFLARE OFF!!!
- Gunakan docker volume untuk membuat reverse proxy
- SSL sebisa mungkin gunakan wildcard
- Untuk DNS bisa sesuaikan seperti contoh di bawah ini
- Frontend team1.studentdumbways.my.id
- Backend api.team1.studentdumbways.my.id
- Push image ke docker registry kalian masing".
Aplikasi dapat berjalan dengan sesuai seperti melakukan login/register.

# Answer

![alt text](https://github.com/aanalff/Task-Photo/blob/main/m1.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m2.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m3.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m4.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m5.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m6.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m7.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m8.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m9.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m10.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m11.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m12.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m13.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m14.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m15.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m16.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m17.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m18.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m19.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m20.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m21.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m22.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m23.jpg?raw=true)


![alt text](https://github.com/aanalff/Task-Photo/blob/main/m24.jpg?raw=true)


![alt text](?raw=true)


![alt text](?raw=true)

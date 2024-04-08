# Task :
1. Jelaskan apa itu Web server dan gambarkan bagaimana cara webserver bekerja.
2. Buatlah Reverse Proxy untuk aplilkasi yang sudah kalian deploy kemarin. (wayshub), untuk domain nya sesuaikan nama masing" ex: alvin.xyz .
3. Jelaskan apa itu load balance.
4. implementasikan loadbalancing kepada aplikasi wayshub yang telah kalian gunakan.

Repository
```https://github.com/dumbwaysdev/wayshub-frontend```

Cara Run Aplikasi :
`npm run start`

# Answer

## 1. Jelaskan apa itu Web server dan gambarkan bagaimana cara webserver bekerja.

Bayangkan sebuah web server seperti seorang pelayan di sebuah restoran. Ketika kita pergi ke restoran dan memesan makanan, pelayan itu bertindak sebagai perantara antara kita (pelanggan) dan dapur (sumber makanan).

Dalam hal ini:
- **Anda** adalah pengguna yang menggunakan browser web.
- **Pelayan** adalah web server.
- **Dapur** adalah server di mana situs web atau aplikasi Anda di-host.

Prosesnya berjalan seperti ini:
1. **Pemesanan (Permintaan):** Anda memberi tahu pelayan (web server) apa yang Anda inginkan (misalnya, membuka halaman web tertentu).
   
2. **Penyampaian Pesanan (Pemrosesan Permintaan):** Pelayan (web server) menerima pesanan Anda dan memeriksa menu (konten situs web atau aplikasi) untuk memahami apa yang Anda minta.

3. **Penyajian (Menyampaikan Respons):** Pelayan (web server) memberi tahu dapur (server) apa yang Anda inginkan, kemudian dapur menyiapkan makanan (halaman web atau konten) yang Anda pesan.

4. **Pengantaran Makanan (Mengirimkan Respons):** Setelah makanan (halaman web atau konten) siap, pelayan (web server) membawanya kepada Anda (pengguna) melalui meja Anda (browser web).

5. **Penyelesaian Pesanan (Penyelesaian Permintaan):** Setelah Anda menerima makanan (halaman web atau konten), pelayan (web server) menyelesaikan pesanan Anda dan siap untuk melayani pelanggan lain.

Jadi, web server adalah bagian penting dari proses menyajikan konten web kepada pengguna. Ini menerima permintaan dari browser, mengirimkannya ke server yang tepat untuk memproses, dan kemudian mengirimkan respons kembali ke browser sehingga Anda bisa melihat halaman web yang diminta.

## 2. Buatlah Reverse Proxy untuk aplilkasi yang sudah kalian deploy kemarin. (wayshub), untuk domain nya sesuaikan nama masing" ex: alvin.xyz .

1. reverse proxy. masuk file nginx di folder etc ( berisi konfigurasi )

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/step%201%20reverse%20proxy.%20masuk%20file%20nginx%20di%20folder%20etc%20(%20berisi%20konfigurasi%20).jpeg?raw=true)

2. nginx kepemilikan root, sudo jgn lupa

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/nginx%20kepemilikan%20root%2C%20sudo%20jgn%20lupa.jpeg?raw=true)

3. lalu buat directory (apps) dan file konfigurasi ( reverse-proxy.conf)

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/lalu%20buat%20directory%20(apps)%20dan%20file%20konfigurasi%20(%20reverse-proxy.conf).jpeg?raw=true)

4. isi file configurasi, location berarti lokasi domain ( / ) berarti di root proxy pass : diarahkan ke tujuan server kita

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/isi%20file%20configurasi.jpeg?raw=true)

5. lalu tambahkan konfigurasi di file nginx.conf

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/lalu%20tambahkan%20konfigurasi%20di%20file%20nginx.conf.jpeg?raw=true)

6. lalu tambahkan perintah include /etc/nginx/apps/reverse-proxy.conf

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/lalu%20tambahkan%20perintah%20include%20etcnginxappsreverse-proxy.conf.jpeg?raw=true)

7. lalu cek apakah konfigurasi reverse proxy berhasil dengan sudo nginx -t jika keterangan syntax is ok berarti konfigurasi berhasil

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/lalu%20cek%20apakah%20konfigurasi%20reverse%20proxy%20berhasil%20dengan%20sudo%20nginx%20-t%20jika%20keterangan%20syntax%20is%20ok%20berarti%20konfigurasi%20berhasil.jpeg?raw=true)

8. lalu reload konfigurasi nginx dan cek status apakah ada yg error atau tidak

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/lalu%20reload%20konfigurasi%20nginx%20dan%20cek%20status%20apakah%20ada%20yg%20error%20atau%20tidak.jpeg?raw=true)

9. cara membuat domain di ubuntu server dengan menambahkan domain di file tersebut

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/cara%20membuat%20domain%20di%20ubuntu%20server%20dengan%20menambahkan%20domain%20di%20file%20tersebut.jpeg?raw=true)

10. lalu masukan ip server kita dan domain yg tadi kita buat

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/lalu%20masukan%20ip%20server%20kita%20dan%20domain%20yg%20tadi%20kita%20buat.jpeg?raw=true)

11. membuat host domain ( windows )

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/membuat%20host%20domain%20(%20windows%20).jpeg?raw=true)

12. reverse proxy berhasi dibuat

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/reverse%20proxy2.jpeg?raw=true)

## 3. Jelaskan apa itu load balance.

Load balancing pada server adalah teknik yang digunakan untuk mendistribusikan lalu lintas atau beban kerja di antara beberapa server secara merata. Tujuannya adalah untuk mencegah satu server menjadi terlalu terbebani sementara yang lainnya kosong, sehingga meningkatkan kinerja, ketersediaan, dan skalabilitas sistem secara keseluruhan. Dengan load balancing, permintaan dari pengguna diproses oleh berbagai server, memastikan bahwa tidak ada satu titik kegagalan tunggal dan menjamin pengalaman pengguna yang lebih baik.

## 4. implementasikan loadbalancing kepada aplikasi wayshub yang telah kalian gunakan.


1. konfigurasi load balance domain adalah variable dari ke dua ip

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/konfigurasi%20load%20balance%20domain%20adalah%20variable%20dari%20ke%20dua%20ip.jpeg?raw=true)

2. keadaan kedua server hidup

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/keadaan%20kedua%20server%20hidup.jpeg?raw=true)

3. keadaaan 1 server mati (alfian_dw)

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/keadaaan%201%20server%20mati%20(alfian_dw).jpeg?raw=true)

4. keadaan server ke dua mati (ubuntu1)

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/keadaan%20server%20ke%20dua%20mati%20(ubuntu1).jpeg?raw=true)

5. keadaan ke dua server mati, menandakan load balance berhasil

![alt text](https://github.com/aanalff/task-foto-W3/blob/main/keadaan%20ke%20dua%20server%20mati%2C%20menandakan%20load%20balance%20berhasil.jpeg?raw=true)


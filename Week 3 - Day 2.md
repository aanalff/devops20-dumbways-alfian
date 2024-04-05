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

## 3. Jelaskan apa itu load balance.

Load balancing pada server adalah teknik yang digunakan untuk mendistribusikan lalu lintas atau beban kerja di antara beberapa server secara merata. Tujuannya adalah untuk mencegah satu server menjadi terlalu terbebani sementara yang lainnya kosong, sehingga meningkatkan kinerja, ketersediaan, dan skalabilitas sistem secara keseluruhan. Dengan load balancing, permintaan dari pengguna diproses oleh berbagai server, memastikan bahwa tidak ada satu titik kegagalan tunggal dan menjamin pengalaman pengguna yang lebih baik.

## 4. implementasikan loadbalancing kepada aplikasi wayshub yang telah kalian gunakan.



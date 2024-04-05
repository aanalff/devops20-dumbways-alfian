Task :
1. Perbandingan antara Monolith & Microservices
2. Deploy Aplikasi wayshub-frontend (NodeJS)
3. Deploy Golang & Python dengan menampilkan nama masing-masing

Repository
```https://github.com/dumbwaysdev/wayshub-frontend```

Cara Run Aplikasi :
`npm run start`

# Answer


Tugas Anda terdiri dari tiga bagian:

Membandingkan Monolith dan Microservices.
Mendeploy aplikasi wayshub-frontend (Node.js).
Mendeploy aplikasi Golang dan Python yang menampilkan nama masing-masing.
Mari kita mulai dengan poin pertama:

1. Perbandingan antara Monolith dan Microservices:

Tentu, berikut adalah perbandingan antara Monolith dan Microservices:

**Monolith:**
1. **Struktur Tunggal:** Monolith adalah aplikasi yang terdiri dari satu unit atau monolit besar yang mencakup semua komponen seperti logika bisnis, antarmuka pengguna, dan akses database.
2. **Kohesif:** Semua bagian dari aplikasi ditempatkan bersama dalam satu kode sumber dan biasanya dikelola dalam repositori tunggal.
3. **Ketergantungan yang Tinggi:** Perubahan pada salah satu bagian aplikasi dapat memengaruhi seluruh aplikasi. Ini karena semua komponen berbagi kode dan sumber daya yang sama.
4. **Pengembangan Awal yang Cepat:** Memiliki keuntungan dalam memulai pengembangan dengan cepat karena semua komponen dapat dibangun secara bersamaan.
5. **Skalabilitas Terbatas:** Sulit untuk mengelompokkan dan menyebarluaskan aplikasi secara horizontal karena semua komponen harus diperlakukan sebagai satu kesatuan.

**Microservices:**
1. **Arsitektur Terdistribusi:** Microservices adalah arsitektur di mana aplikasi dibagi menjadi serangkaian layanan independen yang berjalan secara terpisah.
2. **Pemisahan Fungsionalitas:** Setiap layanan bertanggung jawab atas tugas atau fungsi tertentu, seperti manajemen pengguna, pengolahan pembayaran, atau pengiriman email.
3. **Kemandirian Layanan:** Setiap layanan dapat dikembangkan, dikelola, dan diperbarui secara independen tanpa memengaruhi layanan lainnya.
4. **Skalabilitas Lebih Baik:** Memungkinkan skalabilitas horizontal yang lebih baik karena Anda dapat menambah atau mengurangi instance dari layanan tertentu sesuai dengan kebutuhan.
5. **Kompleksitas Pengelolaan:** Meskipun memungkinkan fleksibilitas dan skalabilitas yang lebih besar, arsitektur Microservices dapat meningkatkan kompleksitas dalam manajemen, pemantauan, dan pengujian aplikasi.

Pemilihan antara Monolith dan Microservices tergantung pada kebutuhan spesifik proyek, tingkat kompleksitas aplikasi, persyaratan skalabilitas, dan kemampuan tim pengembangan. Monolith cocok untuk aplikasi kecil hingga menengah yang memerlukan pengembangan cepat dan manajemen sederhana, sementara Microservices lebih cocok untuk aplikasi besar dengan persyaratan skalabilitas dan perubahan yang kompleks.

## 2. Deploy Aplikasi wayshub-frontend (NodeJS)

Untuk mendeploy aplikasi wayshub-frontend (Node.js) di sebuah server Ubuntu, Anda bisa mengikuti langkah-langkah berikut:

1. **Persiapkan Server:**
   - Pastikan server Ubuntu Anda telah terpasang Node.js dan npm. Jika belum, Anda dapat menginstalnya dengan menjalankan perintah:

     ```bash
     sudo apt update
     sudo apt install nodejs npm
     ```

2. **Unduh dan Persiapkan Kode Aplikasi:**
   - Unduh repositori wayshub-frontend dari GitHub:

     ```bash
     git clone https://github.com/dumbwaysdev/wayshub-frontend
     ```

   - Masuk ke direktori proyek:

     ```bash
     cd wayshub-frontend
     ```

   - Install dependensi aplikasi:

     ```bash
     npm install
     ```

3. **Konfigurasi Aplikasi:**
   - Jika diperlukan, sesuaikan konfigurasi aplikasi seperti port yang akan digunakan atau URL backend jika ada.

4. **Menjalankan Aplikasi:**
   - Jalankan aplikasi menggunakan perintah:

     ```bash
     npm run start
     ```

   - Aplikasi akan berjalan dan Anda akan dapat mengaksesnya melalui browser di alamat IP server Anda pada port yang telah ditentukan (biasanya port 3000 jika tidak diubah).

5. **Mengatur Proses agar Berjalan di Latar Belakang:**
   - Jika Anda ingin menjalankan aplikasi secara terus-menerus tanpa bergantung pada sesi terminal, Anda dapat menggunakan alat seperti `pm2`:

     - Instal `pm2` secara global jika belum terpasang:

       ```bash
       npm install -g pm2
       ```

     - Jalankan aplikasi dengan `pm2`:

       ```bash
       pm2 start npm --name "wayshub-frontend" -- start
       ```

     - Anda juga dapat menjalankan aplikasi secara otomatis saat sistem boot:

       ```bash
       pm2 startup systemd
       pm2 save
       ```

Dengan langkah-langkah di atas, aplikasi wayshub-frontend (Node.js) harus berjalan dan dapat diakses melalui web browser pada server Ubuntu Anda. Pastikan untuk melakukan konfigurasi keamanan yang sesuai, seperti mengatur firewall dan mengamankan koneksi menggunakan HTTPS jika diperlukan.

3. Deploy Golang & Python dengan menampilkan nama masing-masing

- Golang
Pertama 2 kita butuh instalsi enggine nya terlebih dahulu dengan cara

`wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz && sudo su`

`rm -rf /usr/local/go && tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz && exit`

Selanjutnya masukkan path go pada .bashrc
`sudo nano .bashrc`

lalu masukan perintah berikut dipaling bawah
`export PATH=$PATH:/usr/local/go/bin`

Jika sudah sekarang dapat verifikasi go dengan cara berikut
`go version`

Sekarang kita akan membuat aplikasi sederhana menggunakan go. Kalian dapat menjalankan beberapa perintah berikut ini.

Buat sebuah file dengan nama `index.go`

Setelah itu masukkan script dibawah ini.

index.go
package main

import "fmt"

func main() {
    fmt.Println("Alfian Dumbways")
}

Sekarang jalankan aplikasi go dengan menggunakan perintah berikut.

`go run index.go`

Jika aplikasi kalian ingin di build, maka jalankan perintah berikut ini.

`go build index.go`

Jika sudah jalankan aplikasi dengan menggunakan perintah berikut.

`./index`

## phyton

-Pertama-tama kita harus install terlebih dahulu Pyhton3. Untuk instalasi ikuti beberapa perintah di bawah ini.
`sudo apt update; sudo apt upgrade`

-Python3 sudah ada secara default, untuk melakukan pengecekan jalankan perintah berikut.
`python3 -v`

-Sekarang kita install package manager dari python3. Kalian dapat menggunakan perintah berikut ini.
`sudo apt install python3-pip

-Sekarang kita akan membuat aplikasi sederhana menggunakan Python3
`nano index.py`

-Jika sudah sekarang jalankan aplikasi dengan menggunakan perintah berikut ini.

`python3 index.py`




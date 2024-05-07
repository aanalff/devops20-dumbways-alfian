# Task :
1. Perbandingan antara Monolith & Microservices
2. Deploy Aplikasi wayshub-frontend (NodeJS)
3. Deploy Golang & Python dengan menampilkan nama masing-masing

Repository
```https://github.com/dumbwaysdev/wayshub-frontend```

Cara Run Aplikasi :
`npm run start`

# Answer


## 1. Perbandingan antara Monolith dan Microservices:

Berikut adalah perbandingan antara Monolith dan Microservices:

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
   - Pastikan server Ubuntu telah terpasang Node.js dan npm. Jika belum, Anda dapat menginstalnya dengan menjalankan perintah:

     ```bash
     sudo apt update
     sudo apt install nodejs npm
     ```

2. **Unduh dan Persiapkan Kode Aplikasi:**
   - Unduh repositori wayshub-frontend dari GitHub:

     ```bash
     git clone https://github.com/dumbwaysdev/wayshub-frontend
     ```

![alt text](https://github.com/aanalff/photo-week-3/blob/main/Unduh%20dan%20Persiapkan%20Kode%20Aplikasi.jpeg?raw=true)

   - Masuk ke direktori proyek:

     ```bash
     cd wayshub-frontend
     ```

![alt text](https://github.com/aanalff/photo-week-3/blob/main/masuk%20ke%20directory%20project.jpeg?raw=true)

   - Install dependensi aplikasi:

     ```bash
     npm install
     ```

![alt text](https://github.com/aanalff/photo-week-3/blob/main/instalasi%20nvm.jpeg?raw=true)

3. **Konfigurasi Aplikasi:**
   - Jika diperlukan, sesuaikan konfigurasi aplikasi seperti port yang akan digunakan atau URL backend jika ada.

![alt text](https://github.com/aanalff/photo-week-3/blob/main/buat%20konfigurasi%20aplikasi.jpeg?raw=true)

![alt text](https://github.com/aanalff/photo-week-3/blob/main/buat%20isi%20aplikasi%20contohnya%20%20Alfian%20Dumbways%20talent.jpeg?raw=true)

4. **Menjalankan Aplikasi:**
   - jika sudah selesai konfigurasi aplikasi cek ip dulu agar step selanjutnya berjalan lancar, lalu gunakan node index.js (nama file index.js bisa yg lain) untuk menjalankan apliaksi

     ```bash
     npm run start
     ```

![alt text](https://github.com/aanalff/photo-week-3/blob/main/jika%20sudah%20selesai%20konfigurasi%20aplikasi%20cek%20ip%20dulu%20agar%20step%20selanjutnya%20berjalan%20lancar%2C%20lalu%20gunakan%20node%20index.js%20(nama%20file%20index.js%20bisa%20yg%20lain)%20untuk%20menjalankan%20apliaksi.jpeg?raw=true)

   - Aplikasi akan berjalan dan Anda akan dapat mengaksesnya melalui browser di alamat IP server Anda pada port yang telah ditentukan (biasanya port 3000 jika tidak diubah).

![alt text](https://github.com/aanalff/photo-week-3/blob/main/setelah%20itu%20kita%20coba%20cek%20melali%20web%20dengan%20memasukan%20ip%20dan%20host%20nodejs%203000.jpeg?raw=true)


## 3. Deploy Golang & Python dengan menampilkan nama masing-masing

### Golang
Pertama 2 kita butuh instalsi enggine nya terlebih dahulu dengan cara

`wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz && sudo su`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/instalasi%20tools%20golang.jpeg?raw=true)

`rm -rf /usr/local/go && tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz && exit`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/instalasi%20golang%20step%202.jpeg?raw=true)

Selanjutnya masukkan path go pada .bashrc
`sudo nano .bashrc`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/Selanjutnya%20masukkan%20path%20go%20pada%20.bashrc.jpeg?raw=true)

lalu masukan perintah berikut dipaling bawah
`export PATH=$PATH:/usr/local/go/bin`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/Selanjutnya%20perintah%20.bashrc.jpeg?raw=true)

Jika sudah sekarang dapat verifikasi go dengan cara berikut
`go version`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/go%20version.jpeg?raw=true)

Sekarang kita akan membuat aplikasi sederhana menggunakan go. Kalian dapat menjalankan beberapa perintah berikut ini.

Buat sebuah file dengan nama `index.go`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/buat%20file%20go.jpeg?raw=true)

Setelah itu masukkan script dibawah ini.

index.go
package main

import "fmt"

func main() {
    fmt.Println("Alfian Dumbways")
}

![alt text](https://github.com/aanalff/photo-week-3/blob/main/Buat%20script%20seperti%20ini.jpeg?raw=true)

Sekarang jalankan aplikasi go dengan menggunakan perintah berikut.

`go run index.go`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/go%20run%20index.go.jpeg?raw=true)

Jika aplikasi kalian ingin di build, maka jalankan perintah berikut ini.

`go build index.go`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/go%20build%20index.go.jpeg?raw=true)

Jika sudah jalankan aplikasi dengan menggunakan perintah berikut.

`./index`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/.index.jpeg?raw=true)


### phyton

-Pertama-tama kita harus install terlebih dahulu Pyhton3. Untuk instalasi ikuti beberapa perintah di bawah ini.
`sudo apt update; sudo apt upgrade`

-Python3 sudah ada secara default, untuk melakukan pengecekan jalankan perintah berikut.
`python3 -v`

-Sekarang kita install package manager dari python3. Kalian dapat menggunakan perintah berikut ini.
`sudo apt install python3-pip

-Sekarang kita akan membuat aplikasi sederhana menggunakan Python3
`nano index.py`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/nano%20index.py.jpeg?raw=true)
-Jika sudah sekarang jalankan aplikasi dengan menggunakan perintah berikut ini.

`python3 index.py`

![alt text](https://github.com/aanalff/photo-week-3/blob/main/python3%20index.py.jpeg?raw=true)

Tampilan python3 di web

![alt text](https://github.com/aanalff/photo-week-3/blob/main/tampilan%20python3.jpeg?raw=true)



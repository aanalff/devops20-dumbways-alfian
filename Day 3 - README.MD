Task :
1. Cari perbedaan antara distro Ubuntu dan CentOS!
2. Apa perbedaan dari CLI & GUI?
3. Di VM masing-masing :
- Install nginx, lalu akses melalui browser/ `curl <ip kalian>`
- Ganti IP address kalian (bebas) lalu akses kembali nginx (`/etc/netplan`)
4. Terangkan fungsi systemctl dan contoh commandnya (gunakan nginx)

Answer: 

1. Cari perbedaan antara distro Ubuntu dan CentOS!

Berikut beberapa perbedaan utama dari CentOS juga Ubuntu.

- CentOS merupakan sistem operasi berbasis Red Hat Enterprise Linux (RHEL), sedangkan Ubuntu merupakan sistem operasi berbasis Debian. Hal ini tentunya mempengaruhi software package management system yang digunakan. CentOS menggunakan format RPM dan Yum management tool, sedangan Ubuntu menggunakan format .deb dan APT-GET management tool.

- CentOS memiliki siklus rilis yang lebih lama, dikarenakan update yang terbilang jarang dilakukan atau tidak rutin. Berbeda dengan Ubuntu yang rutin melakukan update setiap 6 bulan sekali.  

- Ubuntu lebih mudah digunakan oleh pemula, sedangkan CentOS jauh lebih sulit untuk dipelajari dan digunakan.

- Ubuntu memiliki dukungan komunitas yang lebih besar dibandingkan CentOS.

- Dukungan komunitas tersebut berpengaruh pada hasil dokumentasi dan panduan dasar yang disediakan oleh Ubuntu, sehingga dokumentasi yang dimiliki jauh lebih lengkap dibandingkan dengan CentOS.

- Ubuntu memiliki fitur yang lebih banyak dibandingkan dengan CentOS, tetapi hal ini membuat Ubuntu memakan lebih banyak resource dan lebih berat untuk dijalankan.

- CentOS kompatibel dengan beberapa control panel yang umum digunakan dalam web hosting, yaitu cPanel dan InterWorx, sedangkan Ubuntu tidak kompatibel dengan control panel tersebut.


2. Apa perbedaan dari CLI & GUI?

Perbedaan antara GUI dan CLI:
1. Dari segi fungsi, GUI lebih multi-fungsi dibandingkan CLI.
2. GUI lebih mudah diadaptasi karena tampilannya yang menarik, sementara CLI sulit karena hanya berupa teks.
3. Interaksi dengan CLI hanya menggunakan keyboard, sedangkan GUI memungkinkan pengguna berinteraksi dengan berbagai perangkat.
4. GUI lebih mudah dalam konektivitas dengan perangkat lain di jaringan yang sama, sementara CLI lebih rumit.
5. GUI menyediakan elemen-elemen interaktif, sementara CLI hanya menampilkan teks.
   
Kesimpulan:
GUI dan CLI memiliki kelebihan dan kekurangan masing-masing. CLI dianggap lebih sulit bagi pengguna awam, namun dengan pengetahuan dasar tentang bahasa pemrograman, CLI dapat dijalankan dengan mudah. Pemilihan antara GUI dan CLI tergantung pada kenyamanan pengguna, namun belajar CLI dapat memperluas pengetahuan tentang teknologi dan sistem operasi.

3. Di VM masing-masing :
- Install nginx, lalu akses melalui browser/ `curl <ip kalian>`
- Ganti IP address kalian (bebas) lalu akses kembali nginx (`/etc/netplan`)

Instal nginx menggunakan command sudo apt install nginx 
setelah itu cek status jika nginx sudah active dengan command systemctl status nginx
lalu cek ip untuk akses nginx melalui browser dengan command ifconfig
![alt text](https://github.com/aanalff/Task-Photo/blob/main/A-1.jpeg?raw=true)

Berikut tampilan nginx jika berhasil diakses melalui browser
![alt text](https://github.com/aanalff/Task-Photo/blob/main/A-2.jpeg?raw=true)


4. Terangkan fungsi systemctl dan contoh commandnya (gunakan nginx)

Berikut adalah beberapa contoh command systemctl beserta fungsinya:

1. Start: Memulai sebuah layanan.
   sudo systemctl start nginx

2. Stop: Menghentikan sebuah layanan.
   sudo systemctl stop nginx

3. Restart: Menghidupkan kembali sebuah layanan.
   sudo systemctl restart nginx

4. Enable: Mengaktifkan sebuah layanan agar berjalan saat sistem boot.
   sudo systemctl enable nginx

5. Disable: Menonaktifkan sebuah layanan agar tidak berjalan saat sistem boot.
   sudo systemctl disable nginx

6. Status: Melihat status dari sebuah layanan.
   sudo systemctl status nginx

7. List-Units: Melihat daftar unit-unit yang sedang berjalan.
   systemctl list-units

8. List-Unit-Files: Melihat daftar unit files yang tersedia.
   systemctl list-unit-files

9. Mask: Menyembunyikan sebuah layanan, mencegahnya untuk dijalankan.
   sudo systemctl mask nginx

10. Unmask: Membuka kembali sebuah layanan yang telah di-mask.
    sudo systemctl unmask nginx

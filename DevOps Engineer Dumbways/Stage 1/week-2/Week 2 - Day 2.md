# TASK Manage Server in Terminal
- Buat 3 directory yang masing-masing berisi 2 file dan rapihkan sebaik mungkin!
- Penjelasan text manipulation beserta step by step
- Penjelasan tool htop atau nmon
- buatlah BASH Script untuk instalasi nginx

# ANSWER
## 1. Buat 3 directory yang masing-masing berisi 2 file dan rapihkan sebaik mungkin!
1. Pertama buat buat 3 directory sekaligus dengan command **mkdir nama_directory nama_directory nama_directory** setelah itu ls untuk melihat list directory yang sudah dibuat seperti hero, item dan team.

![alt text](https://github.com/aanalff/Task-Photo/blob/main/22.1.png?raw=true)

2. Setelah directory terbuat lanjut untuk membuat file didalam masing-masing directory seperti berikut:
Pertama masuk ke directory yang mau dibuatkan file didalamnya contohnya directory hero, dengan cara **cd hero** cd = change directory
setelah masuk directory hero untuk membuat file menggunakan command **touch nama_file nama_file** contohnya meepo dan slark. setelah itu ls untuk melihat list file yang ada didalam directory hero. jika sudah gunakan **cd ..** untuk keluar dari directory saat ini. lalu ulangi cara ini untuk membuat directory dan file yang diinginkan.
 
![alt text](https://github.com/aanalff/Task-Photo/blob/main/22.2.png?raw=true)

![alt text](https://github.com/aanalff/Task-Photo/blob/main/22.3.png?raw=true)

![alt text](https://github.com/aanalff/Task-Photo/blob/main/22.4.png?raw=true)


## 2. Penjelasan text manipulation beserta step by step

Manipulasi teks di Ubuntu adalah tentang cara mengubah atau memproses kata-kata dan kalimat dalam file teks menggunakan command yang ada di Ubuntu. Misalnya, bisa mencari kata-kata tertentu, mengganti kata-kata dengan yang lain, atau mengekstrak informasi tertentu dari teks.

Beberapa command yang sering digunakan untuk hal ini adalah:

1. **grep**: Ini berguna untuk mencari kata-kata dalam teks.
2. **sed**: Digunakan untuk mengubah atau menghapus bagian-bagian tertentu dari teks.
3. **cat**: Menggabungkan teks dari beberapa file.
4. **sort**: Digunakan untuk mengurutkan baris ascending atau descending dalam teks.
5. **echo**: dapat digunakan untuk Menampilkan Pesan di Layar, Menyimpan Pesan dalam Variabel, Menyimpan Pesan ke File, Menambahkan Pesan ke File
6. **cut**: Untuk memotong bagian-bagian tertentu dari teks.
7. **uniq**: Ini menghilangkan baris duplikat dari teks.
8. **tr**: Berguna untuk mengganti atau menghapus karakter dalam teks.
9. **paste**: Menggabungkan teks dari beberapa file menjadi satu baris.
10. **join**: Digunakan untuk menggabungkan teks dari dua file berdasarkan kesamaan.
11. **head** dan **tail**: Menunjukkan sebagian awal atau akhir dari teks.
12. **awk**: Alat ini membantu Anda memproses dan mengatur teks dalam format yang berbeda.
13. **wc**: Menghitung jumlah kata atau baris dalam teks.
14. **fmt**: Untuk memformat teks agar lebih mudah dibaca.
15. **tee**: Menyalurkan teks ke beberapa file.

Dengan menggunakan command tersebut dan beberapa trik, kita bisa melakukan banyak hal dengan teks di Ubuntu, seperti otomatisasi tugas atau pemrosesan data, berikut beberapa contoh penggunaan `grep` `sed` `cat` `sort` `echo`

- grep

grep digunakan untuk mencari kata didalam file

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/grep.jpeg?raw=true)

- sed

sed digunakan untuk mengubah atau menghapus bagian-bagian tertentu dari teks.

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/sed.jpeg?raw=true)

- cat

cat memiliki beberapa fungsi contohnya:

cat buat dan isi file

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/cat%20buat%20dan%20isi%20file.jpeg?raw=true)

cat untuk menggabungkan atau mengganti isi beberapa file ke file lain

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/cat%20untuk%20menggabungkan%20atau%20mengganti%20isi%20beberapa%20file%20ke%20file%20lain.jpeg?raw=true)

- sort

sort digunakan untuk mengurutkan baris ascending atau descending dalam teks

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/sort%20untuk%20mengurutkan%20nomer.jpeg?raw=true)

- echo dapat digunakan untuk Menampilkan Pesan di Layar, Menyimpan Pesan dalam Variabel, Menyimpan Pesan ke File, Menambahkan Pesan ke File

echo untuk menampilkan pesan

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/echo%20untuk%20menampilkan%20pesan.jpeg?raw=true)

echo untuk menampilkan variabel

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/echo%20untuk%20menampilkan%20variabel.jpeg?raw=true)

echo untuk menambahkan text ke file yg sudah ada

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/echo%20untuk%20menambahkan%20text%20ke%20file%20yg%20sudah%20ada.jpeg?raw=true)

echo untuk membuat file baru beserta isinya dan untuk mengganti isi didalam file

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/echo%20untuk%20membuat%20file%20baru%20beserta%20isinya%20dan%20untuk%20mengganti%20isi%20didalam%20file.jpeg?raw=true)

## 3. Penjelasan tool htop atau nmon


1. **htop**:

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/htop.jpeg?raw=true)

   - **Deskripsi**: `htop` adalah alat untuk melihat apa yang sedang dilakukan oleh komputer Anda. Ini memberikan tampilan yang lebih bagus dan mudah digunakan.
   - **Fitur Utama**:
     - Menampilkan daftar proses dengan warna-warna yang membantu.
     - Dapat mengurutkan proses berdasarkan hal-hal seperti seberapa banyak CPU yang digunakan.
     - Menunjukkan grafik untuk melihat seberapa banyak CPU dan memori yang digunakan.
     - Dapat membantu kita menghentikan proses yang menyebabkan masalah.
   - **Cara Menggunakannya**: Anda hanya perlu menjalankan `htop` di terminal untuk memulainya, dan kemudian Anda bisa melihat apa yang terjadi di komputer Anda.

2. **nmon** (Nigel's Monitor):

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/nmon.jpeg?raw=true)
   - **Deskripsi**: `nmon` adalah alat untuk melihat bagaimana komputer kita menggunakan sumber daya seperti CPU, memori, dan disk.
   - **Fitur Utama**:
     - Menampilkan informasi tentang CPU, memori, disk, dan jaringan.
     - Dapat menampilkan grafik untuk memudahkan kita melihat bagaimana penggunaannya dari waktu ke waktu.
     - Dapat menyimpan informasi untuk dilihat nanti.
     - Memiliki tombol-tombol khusus untuk membantu menjelajahi informasi.
   - **Cara Menggunakannya**: kita hanya perlu menjalankan `nmon` di terminal, dan kemudian kita bisa melihat informasi tentang apa yang sedang dilakukan oleh komputer kita.

Kedua alat ini membantu kita untuk melihat bagaimana komputer sedang digunakan dan memantau kinerjanya. Ini bisa membantu kita menemukan masalah atau mengetahui apakah komputer sedang bekerja keras atau tidak. Pilihan antara `htop` dan `nmon` tergantung pada preferensi masing-masing dan apa yang kita cari dalam tools pemantauan.

## 4. buatlah BASH Script untuk instalasi nginx

![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/bash%20script%20nginx.jpeg?raw=true)
![alt text](https://github.com/aanalff/photo-task-w-2/blob/main/nginx%20installed.jpeg?raw=true)

Berikut Langkah-langkahnya:

1. Skrip dimulai dengan `#!/bin/bash`, yang menandakan bahwa ini adalah skrip Bash.
2. Kemudian, skrip memeriksa apakah pengguna yang menjalankan skrip adalah root atau bukan. Hal ini penting karena penginstalan perangkat lunak biasanya memerlukan izin root.
3. Selanjutnya, repositori paket diperbarui dengan menjalankan `apt update`.
4. Nginx diinstal menggunakan `apt install -y nginx`.
5. Layanan Nginx kemudian dijalankan menggunakan `systemctl start nginx`.
6. Terakhir, Nginx diaktifkan untuk memulai secara otomatis saat boot dengan perintah `systemctl enable nginx`.
7. Skrip mencetak pesan yang memberi tahu pengguna bahwa instalasi Nginx telah selesai.

Simpan skrip di file dengan ekstensi `.sh`, misalnya `install_nginx.sh`. Berikan izin eksekusi dengan menjalankan `chmod +x install_nginx.sh`, dan kemudian jalankan skrip dengan perintah `./install_nginx.sh`. Skrip ini akan menjalankan seluruh proses instalasi Nginx secara otomatis.



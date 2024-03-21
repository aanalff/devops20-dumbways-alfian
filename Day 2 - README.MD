week 1 day 2

Task :
1.	Perbedaan antara IP Private & Public, serta IP Dynamic & Static!
2.	Buat penjelasan singkat tentang Virtualization!
3.	Buat rancangan sebuah jaringan dengan spesifikasi sebagai berikut!
o	CIDR Block : 192.168.1.xxx/24
o	Subnet : 255.255.255.0
o	Gateway : 192.168.1.1 (Gunakan app.diagrams.net untuk membuat diagramnya, Referensi gambar sudah disertakan)
4.	Buat step-by-step untuk menginstall Virutal Machine via VMware, Virtualbox atau VM pilihan kalian!

Answer

  1. Perbedaan antara IP Private & Public, serta IP Dynamic & Static

    IP Private & IP Public:
   - IP Private: Ini seperti alamat rumahmu di dalam jaringanmu sendiri. Hanya bisa digunakan untuk komunikasi di dalam jaringanmu sendiri, seperti di rumah atau kantor.
   - IP Public: Ini seperti alamat rumahmu di dunia internet. Bisa digunakan untuk komunikasi dengan perangkat di seluruh dunia. 

     IP Dynamic & IP Static:
   - IP Dynamic: Alamat yang berubah-ubah seperti nomor parkiran yang berubah setiap kali kamu datang ke tempat yang sama. Ini diberikan secara otomatis oleh jaringan setiap kali perangkat terhubung.
   - IP Static: Alamat yang tetap seperti nomor parkiran yang selalu sama setiap kali kamu datang ke tempat yang sama. Kamu menetapkannya secara manual untuk perangkatmu, dan tidak berubah kecuali kamu mengubahnya sendiri.

     2. Buat penjelasan singkat tentang Virtualization
Virtualitzation adalah operation system yang terinstall operation system lagi didalamnya, seperti rumah didalam rumah.

  3. Buat rancangan sebuah jaringan dengan spesifikasi sebagai berikut:
o	CIDR Block : 192.168.1.xxx/24
o	Subnet : 255.255.255.0
o	Gateway : 192.168.1.1 (Gunakan app.diagrams.net untuk membuat diagramnya, Referensi gambar sudah disertakan)
![alt text](https://github.com/aanalff/Task-Photo/blob/main/Simulasi%20jaringan.jpeg?raw=true)

4.	Buat step-by-step untuk menginstall Virutal Machine via VMware, Virtualbox atau VM pilihan kalian!

- Buka virtual box, lalu klik NEW untuk membuat vm baru.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/1-1.jpeg?raw=true)

- Lalu cari file iso ubuntu dan buka filenya, lalu Next.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/1-2.jpeg?raw=true)

- Beri nama vm ubuntu ( UBUNTU DW ) dan pilih skip unattended instalation, lalu Next.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/1-3.jpeg?raw=true)

- Atur Base memory (4 Gb) dan  Prosessors (2 core) (opsional tergantung kebutuhan), lalu Next.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/1-4.jpeg?raw=true)

- Atur Disk (20 Gb) (sesuai kebutuhan), lalu Next.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/1-5.jpeg?raw=true)

- Setelah semua selesai cek kembali spesifikasi vm yang ingin dibuat, jika sudah sesuai klik Finish. dan vm ubuntu telah selesai dibuat.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/1-6.jpeg?raw=true)

- Setelah ubuntu berhasil terinstal di vm seting untuk Networknya ganti dari NAT menjadi Bridged Adapter
![alt text](https://github.com/aanalff/Task-Photo/blob/main/1-7.jpeg?raw=true)

- Setelah Ubuntu server berhasil dibuka lanjut untuk instalasi ubuntu server. disini pilih bahasa lalu tekan enter.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/1.jpeg?raw=true)

- Pilih continue whitout updating
![alt text](https://github.com/aanalff/Task-Photo/blob/main/2.jpeg?raw=true)

- Configurasi keyboard tidak perlu di ubah jika tidak dibutuhkan, langsung done.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/3.jpeg?raw=true)

- Network connection pilih Eps0s3 eth untuk custom network
![alt text](https://github.com/aanalff/Task-Photo/blob/main/4.jpeg?raw=true)

- Pilih edit IPv4
![alt text](https://github.com/aanalff/Task-Photo/blob/main/5.jpeg?raw=true)

- Pilih Manual
![alt text](https://github.com/aanalff/Task-Photo/blob/main/6.jpeg?raw=true)

- Isi sesuai ip, jika sudah save & done
![alt text](https://github.com/aanalff/Task-Photo/blob/main/7.jpeg?raw=true)

- Configure Proxy langsung done.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/8.jpeg?raw=true)

- Configure ubuntu arcive mirror langsung done.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/9.jpeg?raw=true)

- Configure storage pilih Custom Storage Layout
![alt text](https://github.com/aanalff/Task-Photo/blob/main/10.jpeg?raw=true)

- Klik pada Free space lalu atur 10 Gb (sesuai kebutuhan), pilh format ext4 dan mount / (untuk Repository)
![alt text](https://github.com/aanalff/Task-Photo/blob/main/11.jpeg?raw=true)

- lalu pilih free space lagi atur 2 Gb (sesuai kebutuhan), pilih format swap (untuk memory cadangan)
![alt text](https://github.com/aanalff/Task-Photo/blob/main/12.jpeg?raw=true)

- cek kembali partition yang telah dibuat jika sudah oke, pilih done.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/13.jpeg?raw=true)

- Pilih continue untuk memastikan.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/14.jpeg?raw=true)

- Profile setup isi sesuai yang dibutuhkan (ubuntu_dw)
![alt text](https://github.com/aanalff/Task-Photo/blob/main/15.jpeg?raw=true)

- Pilih Instal OpenSSH server
![alt text](https://github.com/aanalff/Task-Photo/blob/main/16.jpeg?raw=true)

- Langsung done disini
![alt text](https://github.com/aanalff/Task-Photo/blob/main/17.jpeg?raw=true)

- Tunggu proses installing system
![alt text](https://github.com/aanalff/Task-Photo/blob/main/18.jpeg?raw=true)

- jika Installing system telah selesai akan muncul perintah reboot. lalu pilih reboot now.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/19.jpeg?raw=true)

- Proses instalasi Ubuntu server telah selesai.
![alt text](https://github.com/aanalff/Task-Photo/blob/main/20.jpeg?raw=true)

![alt text](?raw=true)







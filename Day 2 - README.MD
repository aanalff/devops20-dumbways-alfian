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
![alt text](?raw=true)
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





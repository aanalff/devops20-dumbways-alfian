Task :
1. Cari perbedaan antara distro Ubuntu dan CentOS!
2. Apa perbedaan dari CLI & GUI?
3. Di VM masing-masing :
- Install nginx, lalu akses melalui browser/ `curl <ip kalian>`
- Ganti IP address kalian (bebas) lalu akses kembali nginx (`/etc/netplan`)
4. Terangkan fungsi systemctl dan contoh commandnya (gunakan nginx)

Perbedaan CentOS dan Ubuntu
Berikut beberapa perbedaan utama dari CentOS juga Ubuntu.

- CentOS merupakan sistem operasi berbasis Red Hat Enterprise Linux (RHEL), sedangkan Ubuntu merupakan sistem operasi berbasis Debian. Hal ini tentunya mempengaruhi software package management system yang digunakan. CentOS menggunakan format RPM dan Yum management tool, sedangan Ubuntu menggunakan format .deb dan APT-GET management tool.

- CentOS memiliki siklus rilis yang lebih lama, dikarenakan update yang terbilang jarang dilakukan atau tidak rutin. Berbeda dengan Ubuntu yang rutin melakukan update setiap 6 bulan sekali.  

- Ubuntu lebih mudah digunakan oleh pemula, sedangkan CentOS jauh lebih sulit untuk dipelajari dan digunakan.

- Ubuntu memiliki dukungan komunitas yang lebih besar dibandingkan CentOS.

- Dukungan komunitas tersebut berpengaruh pada hasil dokumentasi dan panduan dasar yang disediakan oleh Ubuntu, sehingga dokumentasi yang dimiliki jauh lebih lengkap dibandingkan dengan CentOS.

- Ubuntu memiliki fitur yang lebih banyak dibandingkan dengan CentOS, tetapi hal ini membuat Ubuntu memakan lebih banyak resource dan lebih berat untuk dijalankan.

- CentOS kompatibel dengan beberapa control panel yang umum digunakan dalam web hosting, yaitu cPanel dan InterWorx, sedangkan Ubuntu tidak kompatibel dengan control panel tersebut.

Untuk memudahkanmu dalam memahami perbedaan antara dua sistem operasi distribusi Linux, berikut dibuat tabel mengenai perbedaan antara CentOS dan Ubuntu. Yuk mari kita lihat perbedaan keduanya!

<!DOCTYPE html>
<html>
<head>
	<title> Belajar Tabel HTML</title>
	<meta charset="utf-8">
</head>
<body>
 
 <table>
 	<tr>
 		<td> Baris 1 Kolom 1</td>
 		<td> Baris 1 Kolom 2</td>
 	</tr>
 	<tr>
 		<td> Baris 2 Kolom 1</td>
 		<td> Baris 2 Kolom 2</td>
 	</tr>
 </table>

</body>
</html>

 	CentOS	Ubuntu
System core	Berbasis Red Hat Enterprise Linux (RHEL)	Berbasis Debian
Cycle release	Jarang dilakukan update	Update dilakukan setiap 6 bulan
Package command	RPM dan YUM	APT-GET
Ease of use	Expert level, sulit untuk digunakan oleh pemula	User-friendly, dapat digunakan oleh pemula
Software	Software yang dimiliki tidak sebanyak OS lain, tetapi mendukung cPanel	Memiliki banyak software tetapi tidak mendukung cPanel

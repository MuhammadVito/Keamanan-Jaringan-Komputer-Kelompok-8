# Keamanan-Jaringan-Komputer-Kelompok-8

## A. Anggota kelompok yang berkontribusi dalam pengerjaan tugas
1. Muhammad Vito Susilo Putra (21050974041)
2. Febrian Afandi (21050974012)
3. Muhammad Husein Febriansyah (21050974062)
4. Fhadluna Arum Dhany (20050974027)

## B. Cara Instalasi Ubuntu Server pada Virtual Box
1. Buka VirtualBox
2. Pada Tab Option Machine Pilih New.
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/18635e33-944b-4a5d-a544-58a1d50ee865" width=60% height=60%>

2. Maka akan muncul halaman Create Virtual Machine : Name and Operating System
- Dibagian Name masukkan nama untuk VM yang akan dibuat.
- Dibagian Type pilih Linux
- Dibagian Version pilih Ubuntu (64 Bit)
- Setelah itu pilih Next
3. Maka akan muncul halaman Create Virtual Machine : Memory Size
- Dibagian Memory Size ukuran RAM yang digunakan 1024 MB
- Lalu pilih Next
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/287447ad-6da6-49e1-bc89-387a77c77c9f" width=60% height=60%>

4. Maka akan muncul halaman Create Virtual Machine : Hard Disk
- Dibagian ini centang option Create a virtual hard disk now
- Lalu pilih Create
5. Maka akan muncul halaman Create Virtual Hard Disk : Hard disk file type
- Pilih VDI (VirtualBox Disk Image)
- Lalu pilih Next
6. Maka akan muncul halaman Create Virtual Hard Disk : Storage on physical hard disk
- Pilih Dynamically allocated
- Lalu pilih Next
7. Maka akan muncul halaman Create Virtual Hard Disk : File location and size
- Tidak ada perubahan pada halaman ini, biarkan default dengan penggunaan disk 10,00 GB
- Lalu pilih Create
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/eca74432-ba73-4e48-9fed-f68cbd071ebb" width=60% height=60%>

8. Kemudian akan kembali ke halaman utama dari VirtualBox.
9. Di halaman utama VirtualBox ini pilih VM yang telah kita buat sebelumnya, kemudian pada option Storage -> Optical Drive arahkan ke file ISO Linux Ubuntu Server yang telah di download sebelumnya.
10. Kemudian pada option Network ganti dari NAT ke Bridge Adapter.  
- kemudian di Bridge Adapter pilih Interface yang digunakan untuk koneksi ke internet.
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/97804d20-e80a-4e7b-bc89-5f9fc1b7a653" width=60% height=60%>

11. Setelah option storage di arahkan ke file ISO Ubuntu Server dan option network di setting ke Bridge Adapter. 
12. Selanjutnya proses instalasi Ubuntu Server akan dilakukan dengan pilih Start.
13. Maka kan muncul halaman console ke VM ubuntu yang kita jalankan.  
- Tunggu hingga Halaman proses instalasi Linux Ubuntu Server tampil.
- Pada bagian halaman proses instalasi bagian pemilihan bahasa pilih  English.
14. Lalu pada halaman Installer update available pilih continue without updating
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/72acc92d-32c5-4c8f-9442-63ea96d607a8" width=60% height=60%>

15. Pada halaman Keyboard configuration  biarkan default pilih Done
16. Pada halaman Network Connection  biarkan default pilih Done
- Pada bagian ini Ubuntu server yang kita install akan mendapatkan IP secara DHCP karena sebelumnya telah disetting option networknya ke Bridge Adapter yang menyediakan secara default Service DHCP.
17. Pada halaman Configure Proxy  biarkan default pilih Done
18. Pada halaman Configure ubuntu archive mirror  biarkan default pilih Done
19. Pada halaman Filesystem Setup  pilih Use An Entire Disk
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/e213206e-50bf-4e7d-8eee-f7c4bfdef979" width=60% height=60%>

20. Pada halaman Filesystem Setup selanjutnya pilih Disk yang tersedia
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/d6ebcb20-5d88-471a-873a-15538bdfc5e2" width=60% height=60%>

21. Pada halaman Filesystem Setup  selanjutnya pilih Done 
- Pada bagian ini secara otomatis akan di buat partisi sesuai kebutuhan dari Ubuntu Server
22. Pada halaman Filesystem Setup  selanjutnya kan muncul pop-up konfirmasi pilih Continue
23. Pada halaman Profile Setup masukkan informasi hostname, username dan password yang akan digunakan, kemudian pilih Done.
24. Pada halaman SSH Setup  centang option Install OpenSSH Server dengan menekan spasi lalu pilih Done
25. Pada halaman Featured Server Snaps  biarkan default pilih Done
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/6585484e-bcb7-43c6-8bbc-73fefdd32880" width=60% height=60%>

26. maka akan muncul halaman Installing system . Pada halaman ini kita tunggu proses instalasi berjalan.
27. Jika proses instalasi telah selesai pilih Reboot kemudian pada prompt Remove the installation media tekan Enter.
28. Setelah reboot VM Linux Ubuntu Server yang kita install dapat di gunakan.
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/e007465f-1365-4ae1-bb6b-b271c0317b4b" width=60% height=60%>

29. Untuk Proses Post-Install lakukan verifikasi koneksi ke internet dengan ping ke IP 8.8.8.8 dan Domain google.com.
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/8fe3373b-6508-4974-85da-94f9d3c6339d" width=60% height=60%>

## C. Cara Instalasi dan Konfigurasi Firewall UFW pada Ubuntu Server
1. Pertama buka Ubuntu dan buka terminal. Kemudian pastikan UFW sudah terinstall. Untuk distro Ubuntu sebenarnya sudah terinstal secara default, namun kalau belum terinstall, silahkan install terlebih dahulu dengan menggunakan perintah sudo apt-get install ufw, seperti gambar dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/b6760f9c-f7aa-4fba-9b4b-59ceb24c5766" width=60% height=60%>

Jika sudah diinstall, maka UFW sudah siap untuk dikonfigurasikan. Berikut langkah-langkah konfigurasi firewall dengan menggunakan UFW.

2. Pertama, konfigurasi UFW untuk IPV6, tujuannya tentu saja agar firewall dapat mengelola rule untuk IPV6. Jalankan perintah sudo nano /etc/default/ufw masuk ke direktori dan  ubah IPV6=no menjadi IPV6=yes kemudian tekan CTRL+X dan tekan Y, lalu tekan enter untuk menyimpan perubahan tersebut. konfigurasi nya seperti gambar dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/4d589681-0492-47e9-9103-6cc6d6963869" width=60% height=60%>

3. Selanjutnya cek status UFW apakah sudah aktif atau belum. Jalankan perintah sudo ufw status verbose. Jika status nya inactive seperti tampilan gambar dibawah ini, berarti UFW belum diaktifkan.
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/a15f8d20-4b90-4332-9c4d-e3aeebb9f0ab" width=60% height=60%>


4. Aktifkan UFW dengan menggunakan perintah ufw enable, kemudian akan muncul tampilan seperti dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/2f00113a-3a86-4d2a-a50f-7848c9e670a8" width=60% height=60%>

5. Selanjutnya gunakan pengaturan default untuk firewall dengan perintah sudo ufw default deny incoming & sudo ufw default allow outgoing seperti dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/4f12df1a-d8b2-4f2c-9779-6bbe6880110d" width=60% height=60%>

6. Berikutnya buat rule untuk mengatur segala koneksi. Rule yang kita digunakan bertujuan untuk mengizinkan service ssh dan telnet pada UFW, sehingga kedua service tersebut tidak akan di block. Untuk membuat rule, gunakan perintah seperti dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/3bd33c83-3a80-4465-897e-4239ddd4240b" width=60% height=60%>

7. Setelah itu, membuat allow koneksi untuk UFW. Berikut ini cara untuk menambahkan perizinan traffic pada rule, dan terdapat beberapa contoh service yang sangat umum atau yang disarankan dan perlu untuk diizinkan. Jika ada service lainya yang ingin diizinkan, bisa menambahkan rulenya lagi sesuai dengan servicenya.
8. Mengizinkan traffic HTTP port 80 untuk keperluan akses web server. Perintah nya seperti dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/f82c7e63-9249-48f1-b17d-47f4fa5aaee1" width=60% height=60%>


9. Mengizinkan koneksi FTP port 21 untuk proses upload / download file dari dan ke server menggunakan aplikasi FTP Client seperti FileZilla. Perintah nya seperti dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/853dddb9-ac9a-46c3-9f54-da4c4258d05d" width=60% height=60%>

10. Mengizinkan port range tertentu agar tidak terblok oleh firewall, misalnya kita ingin mengizinkan port dengan range 6000 sampai 6007 pada protocol TCP dan UDP, maka perintah nya seperti gambar dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/7138c6bc-f3fe-42be-965a-2680e56d9c4e" width=60% height=60%>

11. Mengizinkan IP Address tertentu agar dapat mengakses semua service yang ada pada server tanpa terblok oleh firewall. Perintah nya seperti gambar dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/88ba6c38-5854-42ca-a5b8-4a05e13c1db5" width=60% height=60%>

12. Atau mengizinkan IP Address tertentu untuk port atau service tertentu. Misalnya, kita menginginkan agar IP 192.100.10.10 hanya bisa mengakses port 80, maka perintah nya seperti gambar dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/e860edde-6ebb-4c3b-88cd-3136cfcefecf" width=60% height=60%>

13. Mengizinkan subnet untuk range IP Address tertentu. Jika kita ingin mengizinkan subnet IP Address, kita dapat melakukannya dengan menggunakan notasi CIDR untuk menentukan netmask. Misalnya, kita ingin mengizinkan semua alamat IP mulai dari 192.100.10.1 ke 192.100.10.254, kita bisa menggunakan perintah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/97d40dc3-75ac-4fef-af45-64ddbb6ffcfa" width=60% height=60%>

14. mengizinkan agar range IP tertentu hanya bisa mengakses service tertentu saja. Misalnya range IP 192.100.10.0/24 hanya bisa mengakses service yang ada di port 80, kita bisa gunakan perintah seperti dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/5ad3fe62-72d4-44d5-a1b9-03c613ef80cc" width=60% height=60%>

15. Deny digunakan untuk memblok koneksi yang masuk dengan UFW. Berikut merupakan cara untuk memblokir koneksi dimana koneksi tersebut tidak akan bisa diakses sesuai dengan perintah yang digunakan. Jika kita ingin memblok koneksi dari HTTP, maka perintah nya seperti berikut:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/2afd14d6-b4b1-42f3-8726-185a3213fb1c" width=60% height=60%>

16. jika ingin memblok koneksi dari IP Address tertentu, maka perintahnya seperti berikut:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/c3b8d0de-8443-4184-bec7-3391106de2aa" width=60% height=60%>

17. Berikut merupakan cara untuk mereject koneksi yang digunakan, hampir sama seperti deny connection hanya saja menggunakan perintah yang berbeda.
Jika kita ingin mereject koneksi dari HTTP, maka perintah nya seperti dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/cb89ba53-9885-41a4-a64f-d13bdca4fb89" width=60% height=60%>

18. Jika kita ingin mereject koneksi dari IP Address tertentu, maka perintah nya seperti dibawah ini:
<img src="https://github.com/MuhammadVito/Keamanan-Jaringan-Komputer-Kelompok-8/assets/152166427/b683fb71-a562-417e-ae4a-3de2a2b89c67" width=60% height=60%>

19. Untuk menghapus rule firewall pada UFW yang sudah tidak digunakan, kita  bisa menggunakan perintah sudo ufw delete allow 23 (untuk menghapus rule yang ada pada port 23).
20. Untuk mereset konfigurasi firewall pada UFW yang sudah dibuat, kita bisa membuatnya menjadi konfigurasi seperti semula dengan menggunakan perintah sudo ufw reset. Setelah UFW direset biasanya status nya otomatis akan kembali inactive, tapi kalau masih belum inactive, kita bisa gunakan perintah sudo ufw disable untuk menonaktifkannya.

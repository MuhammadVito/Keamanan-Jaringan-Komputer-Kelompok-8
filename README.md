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


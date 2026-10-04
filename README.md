# Tugas-1

I.	Tujuan Praktikum


•	Mengetahui prosedur instalasi pada sistem operasi Linux.


•	Mampu menjalankan instalasi sistem operasi Linux melalui Graphic User Interface (GUI).


•	Mampu menganalisis proses instalasi sistem operasi Linux.





II.	Alat dan Bahan / Perangkat Lunak


•	Laptop Lenovo dengan sistem operasi Windows.


•	Oracle VM VirtualBox.


•	Ubuntu 14.04.6 LTS Desktop 64-bit (ISO).



III.	Tujuan Penelitian

Sistem operasi merupakan perangkat lunak yang mengelola sumber daya perangkat keras dan menyediakan layanan bagi aplikasi. Linux merupakan sistem operasi yang dapat digunakan melalui Command Line Interface (CLI) maupun Graphical User Interface (GUI). Ubuntu merupakan salah satu distribusi Linux yang menyediakan lingkungan desktop.
	 
IV.	Langkah - Langkah Praktikum
1. Membuat Virtual Machine
Membuat virtual machine baru pada Oracle VM VirtualBox dengan nama Ubuntu 14.04.

<img width="621" height="334" alt="image" src="https://github.com/user-attachments/assets/b3496096-16fc-487a-994a-74763446edc0" />

2. Memulai instalasi
Menjalankan virtual machine dan memilih Install Ubuntu.
<img width="564" height="436" alt="image" src="https://github.com/user-attachments/assets/3dcdb6f8-d77c-49ab-9fb5-5261bf03b493" />
 

3. Jenis instalasi
Memilih Something else agar pembagian partisi dapat dilakukan secara manual.
<img width="561" height="421" alt="image" src="https://github.com/user-attachments/assets/1864e723-5d5d-4413-acd0-ca9bb865b533" />
 

4. Partisi swap
Membuat partisi sekitar 2 GB dan mengaturnya sebagai area swap.



5. Partisi /home
 <img width="495" height="371" alt="image" src="https://github.com/user-attachments/assets/87a7db56-6819-41a3-a19d-4618cc707506" />


6. Partisi root (/)
 <img width="498" height="374" alt="image" src="https://github.com/user-attachments/assets/0d1ac7be-0649-482a-ad2b-5950fbd92926" />


7. Zona waktu
Memilih Jakarta sebagai zona waktu karena menggunakan WIB.
<img width="396" height="297" alt="image" src="https://github.com/user-attachments/assets/11d6b887-63a1-4b17-a9da-26d951c25dd9" />
 

8. Papan ketik
Menggunakan layout keyboard English (US).


9. Membuat akun pengguna
Membuat akun pengguna dengan nama Adzka dan mengaktifkan pilihan memerlukan sandi untuk masuk.
 <img width="531" height="398" alt="image" src="https://github.com/user-attachments/assets/4fb221f9-1313-42e4-bc5b-2ca1b99db2b3" />


10. Proses pemasangan
Menunggu proses penyalinan berkas dan pemasangan Ubuntu ke hard disk virtual.
11. Restart dan login
Setelah pemasangan selesai, virtual machine dinyalakan ulang dan Ubuntu berhasil masuk ke desktop.
 <img width="564" height="423" alt="image" src="https://github.com/user-attachments/assets/0aee5057-f0d1-4d20-8669-a675195b6d87" />

12. Ubuntu siap digunakan
 <img width="514" height="386" alt="image" src="https://github.com/user-attachments/assets/325e1577-4a23-441e-9afc-291d25fbfb49" />



V.	Hasil Praktikum
Instalasi Ubuntu 14.04 LTS berhasil dilakukan menggunakan Oracle VM VirtualBox. Sistem berhasil melakukan boot dan pengguna berhasil masuk ke lingkungan desktop Ubuntu.

VI.	Jawaban Tugas
1.  Laporan proses instalasi dan screenshot


Proses instalasi Ubuntu 14.04 LTS dilakukan menggunakan Oracle VM VirtualBox. Virtual machine dikonfigurasi dengan RAM 2048 MB, 2 CPU, dan hard disk virtual sekitar 25 GB. Instalasi dilakukan secara manual dengan membuat partisi swap, /home, dan root (/). Setelah proses selesai, Ubuntu berhasil dijalankan dan masuk ke desktop.


2. Analisis mengapa perlu memilih / pada Mount Point

Mount Point / (root) merupakan direktori utama pada sistem Linux. Seluruh struktur direktori Linux berada di bawah root, seperti /etc, /usr, /var, dan /home. Partisi yang diberi Mount Point / digunakan sebagai filesystem utama tempat Ubuntu memasang file sistem, program, konfigurasi, dan komponen penting lainnya. Oleh karena itu, partisi root / diperlukan agar sistem operasi Ubuntu dapat diinstal dan dijalankan.


3. Penjelasan Ext4, Ext3, Swap, NTFS, FAT32, dan BT

Ext4: Filesystem Linux yang merupakan pengembangan dari Ext3. Ext4 mendukung journaling dan memiliki kemampuan pengelolaan penyimpanan yang lebih baik.
Ext3: Filesystem Linux yang merupakan pengembangan dari Ext2 dan memiliki fitur journaling untuk membantu menjaga konsistensi filesystem setelah gangguan sistem.
Swap: Ruang pada media penyimpanan yang digunakan Linux sebagai virtual memory ketika kebutuhan memori melebihi RAM yang tersedia.
NTFS: Filesystem yang umum digunakan oleh Windows. NTFS mendukung file dan volume berukuran besar serta fitur seperti permission dan journaling.
FAT32: Filesystem dengan kompatibilitas yang luas dan sering digunakan pada flashdisk serta kartu memori. Keterbatasan utamanya adalah ukuran maksimum satu file sekitar 4 GB.
BT: modern untuk Linux yang dirancang untuk pengelolaan penyimpanan yang lebih fleksibel. Btrfs mendukung fitur seperti snapshot, checksum untuk menjaga integritas data, compression, dan pengelolaan storage yang lebih fleksibel. Btrfs juga menggunakan struktur B-tree dalam pengelolaan data dan metadata.

VII.	Kesimpulan

Praktikum instalasi sistem operasi Linux Ubuntu 14.04 LTS berhasil dilakukan menggunakan Oracle VM VirtualBox. Instalasi dilakukan secara manual dengan membuat partisi swap, /home, dan root (/). Mount Point / berfungsi sebagai filesystem utama sistem Linux, sedangkan Ext4 digunakan sebagai filesystem untuk partisi sistem dan /home.

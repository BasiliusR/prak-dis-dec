[Kembali](README.md)<br>
Praktikum Sistem Terdistribusi Dan Terdesentralisasi <br>
Modul 04<br>
Nama: Basilius Rivalno<br>
NIM: 255410027<br>
Dosen: Dr. Bambang Purnomosidi D. P<br>

<b>Pengujian replikasi</b>

1. Menguji apakah status replica dalam server standby
![standby](Images/modul04_11.png)
Tanda huruf t (True) artinya replica dalam mode standby yang hanya berfungsi untuk mereplikasi data dan menyediakan akses read bagi data

2. Menguji koneksi antara primary dan replica
![koneksi](Images/modul04_12.png)
Hasilnya menunjukkan primary memiliki koneksi aktif dengan replica

3. Melakukan pemeriksaan data pada primary dan replica
![periksa](Images/modul04_13.png)
Hasil pemeriksaan menunjukkan dua baris yang sama ditampilkan pada primary dan replica yang artinya dua server tersebut saling terhubung

4. Menambahkan data baru pada primary
![tambah](Images/modul04_14.png)
Menambahkan baris data atau baris ketiga pada server primary

5. Memeriksa data baru pada kedua server
![data](Images/modul04_15.png)
Hasil menunjukkan penambahan data baru pada primary juga akan ditampilkan juga pada replica yang artinya data dari server primary berhasil diteruskan ke server replica menggunakan mekanisme <i>streaming replication</i>

6. pemeriksaan akhir status replica
![status](Images/modul04_16.png)
Server replica masih dalam mode standby selama replikasi data

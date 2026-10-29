[Kembali](README.md)<br>
Praktikum Sistem Terdistribusi Dan Terdesentralisasi <br>
Modul 04<br>
Nama: Basilius Rivalno<br>
NIM: 255410027<br>
Dosen: Dr. Bambang Purnomosidi D. P<br>

<b>High Availability</b><br>
Jika salah satu atau primary server dalam kondisi down, maka salah satu replica bisa menggantikannya

1. Mematikan atau menghentikan primary server yang sudah ada
![shut down](Images/modul04_17.png)

2. Mempromosikan server replica agar menjadi primary
![promote](Images/modul04_18.png)
Server replica yang telah dipromosikan kondisi nya telah berubah dari yang hanya bisa akses read menjadi read and write

3. Menuliskan data pada replica yang sudah menjadi primary
![input](Images/modul04_19.png)

4. Mengecek apakah data sudah terisi pada primary baru
![cek](Images/modul04_20.png)

5. Mengecek status container
![status](Images/modul04_21.png)
statsu menunjukkan server replica sudah dipromosikan menjadi server primary dan memiliki kondisi healthy


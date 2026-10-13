PRAKTIKUM SISTEM TERDESENTRALISASI DAN TERDISTRIBUSI <br>
Minggu 02<br>
Nama: Basilius Rivalno<br>
NIM: 255410027<br>
Dosen: Dr. Bambang Purnomosidi D. P.<br>

A. Proses<br>
Proses merupakan hasil dari eksekusi program / aplikasi yang bersifat *executable*.
Proses dikelola oleh sistem operasi dan terdiri atas *executable code*, data, *resources*, serta
informasi tentang *state* (*stack* dan *heap*). Setiap aplikasi yang dijalankan akan menjadi
proses.

B. Komunikasi antar proses pada sistem terdistribusi
Komunikasi antar proses pada satu node relatif sederhana karena semua
dikendalikan dan dikelola oleh sistem operasi. Semua proses berjalan pada clock yang
sama dan bisa digunakan shared memory sehingga tidak perlu dilakukan sinkronisasi dan
semua proses akan terurut dan terkendali dengan baik (jika sistem operasi mengelola
proses dengan baik).
Hal ini berbeda dengan pengelolaan proses yang berada pada lebih dari satu node di
sistem terdistribusi. Antar node tidak berada pada clock yang sama dan tidak
memungkinkan penggunaan shared memory (setiap node mengelola memory sendiri dan
tidak dimungkinkan mengakses sampai shared memory karena alasan keamanan). Dengan
demikian, harus ada cara khusus untuk komunikasi antar proses yang berada pada ndoe
yang berbeda. Pada dasarnya, kita bisa menggunakan banyak cara untuk melakukan
komunikasi antar proses pada sistem terdistribusi. Salah satu yang bisa digunakan adalah
GraphQL. Dengan menggunakan GraphQL, bisa dibuat server yang akan melayani query
dari client dengan menggunakan spesifikasi GraphQL. Dengan demikian bisa terjadi
komunikasi antar proses di client (yang meminta layanan) dengan server (yang melayani
permintaan layanan). Peranti pengembangan di kedua sisi tersebut bisa berbeda. Pada
praktikum ini, kita akan menggunakan Python (paket Strawberry - https://strawberry.rocks/)
untuk membuat server.


1.[Tugas01](tugas1.md)<br>
2.[Tugas02](tugas2.md)
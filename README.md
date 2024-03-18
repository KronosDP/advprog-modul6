## Refleksi 1

handle*connection adalah sebuah fungsi yang mengambil `TcpStream` sebagai argumen yang adalah mutable. Secara keseluruhan dia digunakan untuk mengurus \_client* yang masuk kedalam koneksi.

Pertama kita membuat `BufReader`. Hal ini sesuai namanya digunakan untuk menambahkan buffering pada tugas-tugas _read_. Hal ini untuk memperbaiki isu performa.

Lines berguna untuk memisahkan setiap data yang memiliki new line. Kemudian kita menggunakan map untuk melakukan unwrap sebagai string. Take while kemudian akan berjalan selagi line nya tidak kosong. Terakhir pada collect, semuanya akan dikumpulkan dan dalam kasus ini hasilnya akan digabungkan menjadi vektor.

Terakhir, hasilnya akan di print denan println.

## Refleksi 2

![commit 2 ss](./README/reflection2.png)

Ingat bahwa kode status 200 berarti semuanya sudah baik dijalankan. Selanjutnya contents adalah untuk membaca file yang ada yang dalam kasus ini adalah hello.html yang kemudian akan kita ubah menjadi string. Kemudian pada length akan kita dapatkan panjang stringnya. Kemudian responsenya adalah string formatting dimana Context Length adalah panjang file hello.html.

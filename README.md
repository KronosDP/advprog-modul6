## Refleksi 1

handle*connection adalah sebuah fungsi yang mengambil `TcpStream` sebagai argumen yang adalah mutable. Secara keseluruhan dia digunakan untuk mengurus \_client* yang masuk kedalam koneksi.

Pertama kita membuat `BufReader`. Hal ini sesuai namanya digunakan untuk menambahkan buffering pada tugas-tugas _read_. Hal ini untuk memperbaiki isu performa.

Lines berguna untuk memisahkan setiap data yang memiliki new line. Kemudian kita menggunakan map untuk melakukan unwrap sebagai string. Take while kemudian akan berjalan selagi line nya tidak kosong. Terakhir pada collect, semuanya akan dikumpulkan dan dalam kasus ini hasilnya akan digabungkan menjadi vektor.

Terakhir, hasilnya akan di print denan println.

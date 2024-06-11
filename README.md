

Nama: Muhamad Farras Jasir

NIM: 312210361

Kelas: TI.22.A5

Membuat REST Controller
Pada tahap ini, kita akan membuat file REST Controller yang berisi fungsi untuk menampilkan,
menambah, mengubah dan menghapus data. Masuklah ke direktori app\Controllers dan buatlah file
baru bernama Post.php. Kemudian, salin kode di bawah ini ke dalam file tersebut:

![Screenshot (565)](https://github.com/muhamadfarrasjasir12/praktikum7/assets/150880443/d88684c8-3e3d-4d0a-a946-a75e4a3ccc00)



![Screenshot (566)](https://github.com/muhamadfarrasjasir12/praktikum7/assets/150880443/c84bc3dd-fce6-45e8-8839-183eee4caa1c)


Kode diatas berisi 5 method, yaitu:

• index() – Berfungsi untuk menampilkan seluruh data pada database.

• create() – Berfungsi untuk menambahkan data baru ke database.

• show() – Berfungsi untuk menampilkan suatu data spesifik dari database.

• update() – Berfungsi untuk mengubah suatu data pada database.

• delete() – Berfungsi untuk menghapus data dari database.

# Membuat Routing REST API

Untuk mengakses REST API CodeIgniter, kita perlu mendefinisikan route-nya terlebih dulu.
Caranya, masuklah ke direktori app/Config dan bukalah file Routes.php. Tambahkan kode
di bawah ini:

$routes->resource('post');

Untuk mengecek route nya jalankan perintah berikut:

php spark routes

Selanjutnya akan muncul daftar route yang telah dibuat.

![Screenshot (567)](https://github.com/muhamadfarrasjasir12/praktikum7/assets/150880443/1024fc42-fdc9-476c-8361-2c8671b8118b)

# Testing REST API CodeIgniter

Buka aplikasi postman dan pilih create new → HTTP Request

Menampilkan Semua Data

Pilih method GET dan masukkan URL berikut:

http://localhost:8080/post

Lalu, klik Send. Jika hasil test menampilkan semua data artikel dari database, maka pengujian
berhasil.



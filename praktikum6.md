Pastikan terdapat tabel users yang dibuat menggunakan migration pada bab sebelumnya.
![Alt text](screenshot6/image-10.png)

Bersihkan isi User.php yang ada sebelumnya dan isi dengan baris kode berikut
![Alt text](screenshot6/image-9.png)

Controller
Buatlah salinan ExampleController.php pada folder app/Http/Controllers dengan nama HomeController.php dan buatlah fungsi index()
![Alt text](screenshot6/image-11.png)

Ubah route / pada file routes/web.php menjadi seperti ini
![Alt text](screenshot6/image-12.png)

Jalankan aplikasi
![Alt text](screenshot6/image-13.png)

Request Handler
Lakukan import library Request dengan menambahkan baris berikut di bagian atas file
![Alt text](screenshot6/image-14.png)

Ubah fungsi index menjadi
![Alt text](screenshot6/image-15.png)

Jalankan aplikasi
![Alt text](screenshot6/image-16.png)

Response Handler
Lakukan import library Response dengan menambahkan baris berikut di bagian atas file
![Alt text](screenshot6/image-18.png)

Jalankan aplikasi
![Alt text](screenshot6/image-17.png)

Penerapan
Lakukan import model User dengan menambahkan baris berikut di bagian atas file
![Alt text](screenshot6/image-19.png)

Jalankan aplikasi pada route /users/default menggunakan Postman
![Alt text](screenshot6/image-20.png)

Jalankan aplikasi pada route /users/new dengan mengisi body
![Alt text](screenshot6/image-21.png)

Jalankan aplikasi pada route /users/all
![Alt text](screenshot6/image-22.png)
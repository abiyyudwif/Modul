Register
Pastikan terdapat tabel users yang dibuat menggunakan migration pada bab 3 Basic Routing dan Migration.
![Alt text](image-41.png)

Pastikan terdapat model User.php yang digunakan pada bab 5 Model, Controller dan Request-Response Handler.
![Alt text](image-42.png)

Buatlah file AuthController.php dan isilah dengan baris kode berikut
![Alt text](image-43.png)

Tambahkan baris berikut pada routes/web.php
![Alt text](image-44.png)

Jalankan aplikasi pada endpoint /auth/register dengan body berikut
![Alt text](image-45.png)

Authentication
Buatlah fungsi login(Request $request) pada file AuthController.php
![Alt text](image-46.png)

Tambahkan baris berikut pada routes/web.php
![Alt text](image-47.png)

Jalankan aplikasi pada endpoint /auth/login dengan body berikut
![Alt text](image-48.png)

Token
Jalankan perintah berikut untuk membuat migrasi baru
![Alt text](image-49.png)

Tambahkan baris berikut pada migration yang baru terbuat
![Alt text](image-50.png)

Tambahkan atribut token di $fillable pada User.php
![Alt text](image-51.png)

Tambahkan baris berikut pada file AuthController.php
![Alt text](image-52.png)

Jalankan perintah di bawah untuk menjalankan migrasi terbaru
![Alt text](image-53.png)

Jalankan aplikasi pada endpoint /auth/login dengan body berikut. Salinlah token yang didapat ke notepad
![Alt text](image-54.png)

Authorization
Buatlah file Authorization.php pada folder App/Http/Middleware dan isilah dengan baris berikut
![Alt text](image-55.png)

Tambahkan middleware yang baru dibuat pada bootstrap/app.php.
![Alt text](image-56.png)

Buatlah fungsi home() pada HomeController.php
![Alt text](image-57.png)

Tambahkan baris berikut pada routes/web.php
![Alt text](image-58.png)

Jalankan aplikasi pada endpoint /home dengan melampirkan nilai token yang didapat setelah login pada header
![Alt text](image-59.png)
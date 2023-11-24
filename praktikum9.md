Lakukan perubahan pada length kolom token dengan menghapus parameter 72 di belakangnya
![Alt text](image-60.png)

Jalankan perintah di bawah untuk memperbaharui migrasi dan menghapus data yang lama
![Alt text](image-61.png)

Jalankan aplikasi pada endpoint /auth/register dengan body berikut.
![Alt text](image-62.png)

JWT Manual
Tambahkan ketiga fungsi berikut pada AuthController.php
![Alt text](image-63.png)

Lakukan perubahan pada fungsi login
![Alt text](image-64.png)

Tambahkan keempat fungsi berikut pada Middleware/Authorization.php
![Alt text](image-65.png)

Lakukan perubahan pada fungsi handle
![Alt text](image-66.png)

Jalankan aplikasi pada endpoint /auth/login dengan body berikut. Salinlah token yang didapat ke notepad
![Alt text](image-67.png)

Jalankan aplikasi pada endpoint /home dengan melampirkan nilai token yang didapat setelah login pada header
![Alt text](image-68.png)

JWT Library
Lakukan generate jwt key secara online menggunakan website Djecrety ― Django Secret Key Generator
![Alt text](image-69.png)

Lakukan instalasi package jwt firebase dengan menggunakan command berikut
![Alt text](image-70.png)

Tambahkan fungsi berikut pada file AuthController
![Alt text](image-71.png)

Lakukan perubahan pada fungsi login menjadi seperti berikut
![Alt text](image-72.png)

Buatlah file JwtMiddleware.php dan isikan baris code berikut
![Alt text](image-73.png)

Daftarkan middleware yang telah dibuat pada bootstrap/app.php
![Alt text](image-74.png)

Tambahkan baris berikut pada file web.php
![Alt text](image-75.png)

Jalankan aplikasi pada endpoint /auth/login dengan body berikut. Salinlah token yang didapat ke notepad
![Alt text](image-76.png)
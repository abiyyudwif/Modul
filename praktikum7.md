Sebelum membuat migrasi database atau membuat tabel pastikan server database aktif kemudian pastikan sudah membuat database dengan nama lumenpost
![Alt text](image-9.png)

Setelah itu jalankan command berikut untuk membuat file migration
![Alt text](image-10.png)

Ubah fungsi up() pada file migrasi create_posts_table
![Alt text](image-11.png)

Ubah fungsi up() pada file create_comments_table
![Alt text](image-12.png)

Ubah fungsi up() pada file create_tags_table
![Alt text](image-13.png)

Ubah fungsi up() pada file create_post_tag_table
![Alt text](image-14.png)

Kemudian jalankan command
![Alt text](image-15.png)

Pembuatan Model
Buatlah file dengan nama Post.php dan isi dengan baris kode berikut
![Alt text](image-16.png)

Buatlah file dengan nama Comment.php dan isi dengan baris kode berikut
![Alt text](image-17.png)

Buatlah file dengan nama Tag.php dan isi dengan baris kode berikut
![Alt text](image-18.png)

Relasi One-to-Many
Tambahkan fungsi comments() pada file Post.php
![Alt text](image-19.png)

Tambahkan fungsi post() dan atribut postId pada $fillable pada file Comment.php
![Alt text](image-20.png)

Buatlah file PostController.php dan isilah dengan baris kode berikut 
![Alt text](image-21.png)

Buatlah file CommentController.php dan isilah dengan baris kode berikut
![Alt text](image-22.png)

Tambahkan baris berikut pada routes/web.php
![Alt text](image-23.png)

Buatlah satu post menggunakan Postman
![Alt text](image-24.png)

Buatlah satu comment menggunakan Postman
![Alt text](image-25.png)

Tampilkan post menggunakan Postman
![Alt text](image-26.png)

Relasi Many-to-Many
Tambahkan fungsi tags() pada file Post.php
![Alt text](image-27.png)

Tambahkan fungsi posts() pada file Tag.php
![Alt text](image-28.png)

Buatlah file TagController.php dan isilah dengan baris kode berikut
![Alt text](image-29.png)

Tambahkan fungsi addTag dan response tags pada PostController.php
![Alt text](image-30.png)

Tambahkan baris berikut pada routes/web.php
![Alt text](image-31.png)

Buatlah satu tag menggunakan Postman
![Alt text](image-32.png)

Tambahkan tag “jadul” pada post “disana engkau berdua”
![Alt text](image-33.png)

Tampilkan post “disana engkau berdua” menggunakan Postman
![Alt text](image-34.png)

Buatlah postingan “tanpamu apa artinya” menggunakan Postman
![Alt text](image-35.png)

Tambahkan tag “jadul” pada postingan “tanpamu apa artinya”
![Alt text](image-36.png)

Buatlah tag “lagu” menggunakan Postman
![Alt text](image-37.png)

Tambahkan tag “lagu” pada postingan “tanpamu apa artinya”
![Alt text](image-38.png)

Tampilkan post pertama
![Alt text](image-39.png)

Tampilkan post kedua
![Alt text](image-40.png)
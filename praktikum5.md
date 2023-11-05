Dynamic Route Dynamic route adalah route yang dapat berubah-ubah, contohnya pada saat kita membuka suatu halaman web, kadang kita melihat /users/1 atau /users/2 , hal ini yang dinamakan dynamic routes.

![Alt text](screenshot5/image-1.png)

![Alt text](screenshot5/image-2.png)

![Alt text](screenshot5/image-3.png)

Aliases Route Aliases Route digunakan untuk memberi nama pada route yang telah kita buat, hal ini dapat membantu kita, saat kita ingin memanggil route tersebut pada aplikasi kita.

![Alt text](screenshot5/image-4.png)

Group Route Pada lumen, kita juga dapat memberikan grouping pada routes kita agar lebih mudah pada saat penulisan route pada web.php kita.

![Alt text](screenshot5/image-5.png)

Middleware Middleware adalah penengah antara komunikasi aplikasi dan client. Middleware biasanya digunakan untuk membatasi siapa yang dapat berinteraksi dengan aplikasi kita dan semacamnya, kita dapat menambahkan middleware dengan menambahkan file pada folder app/Http/Middleware . Pada folder tersebut terdapat file ExampleMiddleware , kita dapat men- copy file tersebut untuk membuat middleware baru.

![Alt text](screenshot5/image-6.png)

![Alt text](screenshot5/image-7.png)

![Alt text](screenshot5/image-8.png)
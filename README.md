Lakukan koneksi ke MongoDB menggunakan connection string. 

![Alt text](MOD2_01.png)

Buat database dengan melakukan klik “Create Database”

![Alt text](MOD2_02.png)

Lakukan insert buku pertama dengan melakukan klik “Add Data”, pilih “Insert Document”, isi dengan data yang diinginkan dan klik “Insert”

![Alt text](MOD2_03.png)

Lakukan insert buku kedua dengan cara yang sama.

![Alt text](MOD2_04.png)

Lakukan pencarian buku dengan author “Osamu Dazai” dengan mengisi filter yang diinginkan dan klik “Find”

![Alt text](MOD2_05.png)

Lakukan perubahan summary pada buku “No Longer Human” menjadi “Buku yang bagus (,) dengan melakukan klik “Edit Document” (berlambang pensil), mengisi nilai summary yang baru, dan melakukan klik “Update”

![Alt text](MOD2_06.png)

Lakukan penghapusan pada buku “I Am a Cat” dengan melakukan klik “Remove Document” (berlambang tong sampah) dan melakukan klik “Delete”

![Alt text](MOD2_07.png)

Lakukan koneksi ke MongoDB Server dengan menjalankan command mongosh bagi yang menggunakan terminal build in OS sehingga tampilan terminal kalian akan menjadi seperti berikut

![Alt text](MOD2_08.png)

Mencoba melihat list database yang ada di server dengan menjalankan command show dbs.

![Alt text](MOD2_09.png)

Untuk berpindah ke database “bookstore” gunakan command use bookstore, kaliandapat memastikan telah berpindah ke database yang benar dengan melihat tulisansebelum tanda “>”

![Alt text](MOD2_10.png)

Cobalah untuk melihat collection yang ada pada database tersebut denganm enggunakan command show collections.

![Alt text](MOD2_11.png)

Lakukan insert buku “Overlord I” dengan menggunakan command db.books.insertOne() , setelah insert buku berhasil maka MongoDB akan mengembalikan pesan sebagai berikut

![Alt text](MOD2_12.png)

Lakukan insert buku “The Setting Sun” dan “Hujan” dengan insert many denganmenggunakan command db.books.insertMany(<data kalian>) , dan akan mengembalikan pesan sebagai berikut.

![Alt text](MOD2_13.png)

Lakukan pencarian buku dengan menggunakan command db.books.find() untuk melakukan pencarian semua buku.

![Alt text](MOD2_14.png)

Tampilkan seluruh buku dengan author “Osamu Dazai” dengan mengisi argument pada find() dengan menggunakan command db.books.find({<filter yang ingin diisi>})

![Alt text](MOD2_15.png)

Lakukan perubahan summary pada buku “Hujan” menjadi “Buku yang bagus (<NAMA>,<NIM>) dengan mengunakan command db.books.updateOne({<filter>}, {$set: {<data yang akan di update>}}) sehingga output yang dihasilkan oleh MongoDB akan menjadi seperti berikut.

![Alt text](MOD2_16.png)

Lakukan perubahan publisher menjadi “Yen Press” pada semua buku “Osamu Dazai” dengan menggunakan command db.books.updateMany({<filter>}, {$set: {<data yang akan di update>}})

![Alt text](MOD2_17.png)

Lakukan penghapusan pada buku “Overlord I” dengan menggunakan command db.books.deleteOne({})
![Alt text](MOD2_18.png)

Lakukan penghapusan pada semua buku “Osamu Dazai dengan menggunakan command db.books.deleteMany({})
![Alt text](MOD2_19.png)


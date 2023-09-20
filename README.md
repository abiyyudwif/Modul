Lakukan koneksi ke MongoDB menggunakan connection string. 
![MOD2_01](https://github.com/abiyyudwif/Modul2/assets/145477675/8915277a-08f6-4f76-8457-b9b031cf9918)
![Alt text](MOD2_01)

Buat database dengan melakukan klik “Create Database”
![MOD2_02](https://github.com/abiyyudwif/Modul2/assets/145477675/d5938838-6589-4362-86ea-fcb1c000869d)

Lakukan insert buku pertama dengan melakukan klik “Add Data”, pilih “Insert Document”, isi dengan data yang diinginkan dan klik “Insert”
![MOD2_03](https://github.com/abiyyudwif/Modul2/assets/145477675/688fafd7-1b27-4ed6-bd03-5377a60133ba)

Lakukan insert buku kedua dengan cara yang sama.
![MOD2_04](https://github.com/abiyyudwif/Modul2/assets/145477675/30b5292c-46ba-4b8c-a453-152feb3c5cf2)

Lakukan pencarian buku dengan author “Osamu Dazai” dengan mengisi filter yang diinginkan dan klik “Find”
![MOD2_05](https://github.com/abiyyudwif/Modul2/assets/145477675/bc5877ac-6655-4e59-bd21-f4deae9c6a1e)

Lakukan perubahan summary pada buku “No Longer Human” menjadi “Buku yang bagus (,) dengan melakukan klik “Edit Document” (berlambang pensil), mengisi nilai summary yang baru, dan melakukan klik “Update”
![MOD2_06](https://github.com/abiyyudwif/Modul2/assets/145477675/1e22aaef-abaa-4506-952f-459ce43980e9)

Lakukan penghapusan pada buku “I Am a Cat” dengan melakukan klik “Remove Document” (berlambang tong sampah) dan melakukan klik “Delete”
![MOD2_07](https://github.com/abiyyudwif/Modul2/assets/145477675/6cd8db44-fec6-429d-9f61-ff008d87d6cd)

Lakukan koneksi ke MongoDB Server dengan menjalankan command mongosh bagi yang menggunakan terminal build in OS sehingga tampilan terminal kalian akan menjadi seperti berikut
![MOD2_08](https://github.com/abiyyudwif/Modul2/assets/145477675/c204bc57-96ec-4d72-8b12-d5d8d4d7e305)

Mencoba melihat list database yang ada di server dengan menjalankan command show dbs.
![MOD2_09](https://github.com/abiyyudwif/Modul2/assets/145477675/ce262368-f0db-474f-aed1-4f414abccff7)

Untuk berpindah ke database “bookstore” gunakan command use bookstore, kaliandapat memastikan telah berpindah ke database yang benar dengan melihat tulisansebelum tanda “>”
![MOD2_10](https://github.com/abiyyudwif/Modul2/assets/145477675/b6a05960-e45a-437e-84d4-7a498d622eba)

Cobalah untuk melihat collection yang ada pada database tersebut denganm enggunakan command show collections.
![MOD2_11](https://github.com/abiyyudwif/Modul2/assets/145477675/274810ac-a147-4dea-8e74-0741ea15f03e)

Lakukan insert buku “Overlord I” dengan menggunakan command db.books.insertOne() , setelah insert buku berhasil maka MongoDB akan mengembalikan pesan sebagai berikut
![MOD2_12](https://github.com/abiyyudwif/Modul2/assets/145477675/4812cde7-0d6f-4390-81a7-63add0d9592e)

Lakukan insert buku “The Setting Sun” dan “Hujan” dengan insert many denganmenggunakan command db.books.insertMany(<data kalian>) , dan akan mengembalikan pesan sebagai berikut.
![MOD2_13](https://github.com/abiyyudwif/Modul2/assets/145477675/1e208646-648b-4313-8f2b-393521d6546d)

Lakukan pencarian buku dengan menggunakan command db.books.find() untuk melakukan pencarian semua buku.
![MOD2_14](https://github.com/abiyyudwif/Modul2/assets/145477675/7432b3b9-1eb2-4bc1-9459-105b48f5f91f)

Tampilkan seluruh buku dengan author “Osamu Dazai” dengan mengisi argument pada find() dengan menggunakan command db.books.find({<filter yang ingin diisi>})
![MOD2_15](https://github.com/abiyyudwif/Modul2/assets/145477675/4a1f3f74-8cc2-4149-8b7e-50dc7447ed35)

Lakukan perubahan summary pada buku “Hujan” menjadi “Buku yang bagus (<NAMA>,<NIM>) dengan mengunakan command db.books.updateOne({<filter>}, {$set: {<data yang akan di update>}}) sehingga output yang dihasilkan oleh MongoDB akan menjadi seperti berikut.
![MOD2_16](https://github.com/abiyyudwif/Modul2/assets/145477675/bac7d6e4-c911-420a-b009-128248fdf391)

Lakukan perubahan publisher menjadi “Yen Press” pada semua buku “Osamu Dazai” dengan menggunakan command db.books.updateMany({<filter>}, {$set: {<data yang akan di update>}})
![MOD2_17](https://github.com/abiyyudwif/Modul2/assets/145477675/d90978e9-a678-4b0a-95dd-ee68e88e6b6b)

Lakukan penghapusan pada buku “Overlord I” dengan menggunakan command db.books.deleteOne({})
![MOD2_18](https://github.com/abiyyudwif/Modul2/assets/145477675/4f035c2a-5baf-4464-a201-e0d592d898e2)

Lakukan penghapusan pada semua buku “Osamu Dazai dengan menggunakan command db.books.deleteMany({})
![MOD2_19](https://github.com/abiyyudwif/Modul2/assets/145477675/fec4fadb-4535-42a1-8e46-923c57cdaf4e)


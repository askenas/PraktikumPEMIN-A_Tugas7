# PraktikumPEMIN-A_Tugas7
1. Sebelum membuat migrasi database atau membuat tabel pastikan server database
aktif kemudian pastikan sudah membuat database dengan nama lumenpost
2. Kemudian ubah konfigurasi database pada file .env menjadi seperti berikut
   ![Screenshot 2023-11-07 190630](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/25200dd0-27dd-4f2c-8656-f0b9fbaf12b1)
3. Setelah mengubah konfigurasi pada file .env, kita juga perlu menghidupkan
beberapa library bawaan dari lumen dengan membuka file app.php pada folder
bootstrap dan mengubah baris ini
![Screenshot 2023-11-07 190932](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/c3fbd019-037d-4205-8c71-bd61fb72f768)
4. Setelah itu jalankan command berikut untuk membuat file migration![Screenshot 2023-11-07 191202](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/2b1db89f-112d-452f-a3f8-2e41ef2c572a)
![Screenshot 2023-11-07 191236](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/37cc34e7-8985-4e6a-ac17-b13a59986f42)
![Screenshot 2023-11-07 191305](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/89bac516-3f61-4970-a4a9-77c7a1642c7f)
![Screenshot 2023-11-07 191314](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/04ca1728-e792-4151-b081-524c46d32b2c)
5. Ubah fungsi up() pada file migrasi create_posts_table
   ![Screenshot 2023-11-07 191843](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/f0882a47-55cf-44ca-8913-08bf12256e7a)
6. Ubah fungsi up() pada file create_comments_table![Screenshot 2023-11-07 191907](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/5b9cbe4d-d9f1-47c5-9c1b-985acffa0ab5)
7. Ubah fungsi up() pada file create_tags_table
![Screenshot 2023-11-07 192111](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/a4c7f6df-d6a0-4c73-bf35-7cbfd07897da)
9. Kemudian jalankan command
![Screenshot 2023-11-07 192136](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/dcbd45d2-4cb7-4571-a73a-4aa464681c84)
# Pembuatan Model
1. Buatlah file dengan nama Post.php dan isi dengan baris kode berikut
![Screenshot 2023-11-07 192417](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/bfafdce3-ab72-4e82-b546-000006268394)
2. Buatlah file dengan nama Comment.php dan isi dengan baris kode berikut
![Screenshot 2023-11-07 193047](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/78b21337-3f71-419c-ad09-33bedb07492a)
3. Buatlah file dengan nama Tag.php dan isi dengan baris kode berikut
![Screenshot 2023-11-07 193052](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/3a4cb03f-3a36-4366-bdf3-90a4115a0911)
# Relasi One to Many
1. Tambahkan fungsi comments() pada file Post.php
![Screenshot 2023-11-07 193311](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/fb0fa212-0166-405b-9aec-03e7ec923d41)
2. Tambahkan fungsi post() dan atribut postId pada $fillable pada file Comment.php
4. Buatlah file CommentController.php dan isilah dengan baris kode berikut
![Screenshot 2023-11-07 193543](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/d8986d65-ba86-45ff-bb21-d7363077ded6)
5. Tambahkan baris berikut pada routes/web.php
![Screenshot 2023-11-07 194254](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/013515b0-9654-47b8-a871-fd310065f700)
# Relasi Many to Many
1. Tambahkan fungsi tags() pada file Post.php
![Screenshot 2023-11-07 194507](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/b0c5c7cd-c9ee-4497-aa43-7965e176cdf4)
2. Tambahkan fungsi posts() pada file Tag.php
![Screenshot 2023-11-07 194838](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/c9674112-c85c-4cf7-82da-0d4fbbfab981)
3. Buatlah file TagController.php dan isilah dengan baris kode berikut
4. Tambahkan fungsi addTag dan response tags pada PostController.php
5. Tambahkan baris berikut pada routes/web.php
![Screenshot 2023-11-07 200118](https://github.com/askenas/PraktikumPEMIN-A_Tugas7/assets/134838656/5d20076d-c97d-42a0-b271-e174ccaa5e14)




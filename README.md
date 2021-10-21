# **Cara Install Git dan Cara Menggunakan Git**

## **Install Git**

Instalasi Git di Windows memang tidak seperti di Linux yang ketik perintah langsung terinstal. Kita harus men-download dulu, kemudian melakukan ritual next>next>finish.

### **Download Git**

Silahkan buka website resminya Git : https://git-scm.com/

klik kanan dan run as administrator file instaler Git yang sudah diunduh.

![1](https://user-images.githubusercontent.com/92896798/138259599-f690a06c-8032-4873-94e1-593b1ebd0c30.jpg)

Maka akan muncul infomasi lisensi Git, klik Next > untuk melanjutkan.

![2](https://user-images.githubusercontent.com/92896798/138259866-da84e62a-a5a3-4ceb-a2b8-bc777e87177f.jpg)

Selanjutnya menentukan lokasi instalasi. Biarkan saja apa adanya, kemudian klik Next >> sampai muncul sebagai berikut:

Selanjutnya pemilihan emulator terminal. Pilih saja yang bawah, kemudian klik Next >.
![12](https://user-images.githubusercontent.com/92896798/138261619-8369590b-8df7-4be4-8812-8b64757d67dd.jpg)
Setelah selesai, kita bisa langsung klik finish.
![17](https://user-images.githubusercontent.com/92896798/138261943-8f490906-89ae-4ce2-8cd8-45f94840e919.jpg)

Selamat, Git sudah terinstal di Windows. Untuk mencobanya, silahkan buka CMD atau PowerShell, kemudian ketik perintah
```sh
git --version
```
![18](https://user-images.githubusercontent.com/92896798/138262180-3643fe72-2611-44d9-a892-9088ee8b09c8.jpg)
# **Cara penggunaan Git**

Setelah berhasil install ke Git, selanjutnya
## **Login Git**

masukkan username & email Git menggunakan perintah di bawah ini. Lalu tekan ENTER jika sudah benar.

```sh
git config --global user.name "zahrasyifaannisa"
git config --global user.email zahra.gugum@gmail.com
```
Selanjutnya untuk memastikan proses login berhasil, masukkan perintah berikut.
```sh
git config --list
```

![19](https://user-images.githubusercontent.com/92896798/138263897-2a706c5a-8063-4f8f-895f-c75c481e0350.jpg)

## **Login Github**

Langkah kedua menggunakan Git adalah harus login ke dalam website GitHub. Github dan Git memiliki hubungan khusus, yaitu Git yang berperan sebagai version control system dan Github menjadi hosting atau sebagai penyimpan kode pemrograman.

![36](https://user-images.githubusercontent.com/92896798/138262367-6ac41f18-8d7e-4eda-96e2-ee53f396f18d.PNG)

## **Buat Repository**

Setelah berhasil login ke GitHub, Anda bisa mulai membuat repository. Klik tombol New pada menu Repositories untuk membuat repository baru.

![32](https://user-images.githubusercontent.com/92896798/138264248-ae6d9f85-7cfe-4a7e-8ece-18cf5963d2a5.PNG)

Kemudian akan diarahkan pada halaman untuk membuat repository baru seperti gambar di bawah ini. perlu mengisi detail informasi berikut:

```Nama Repository``` : digunakan untuk identitas repository yang dibuat.
<br>
```Deskripsi Repository``` : berfungsi untuk deskripsi dari repository yang dibuat.
```Jenis Repository``` : jenis repository dibagi menjadi Public dan Private. Ketika Anda mengatur repository menjadi Public, orang lain dapat melihat repository yang Anda buat. Sebaliknya, jika Anda mengaturnya sebagai Private, repository tersebut hanya bisa diakses oleh Anda. Setelah mengisi detail informasi di atas,
<br>
klik ```Create Repository```.

## **Buat Folder pada Windows**
Selanjutnya, perlu membuat folder pada local disk komputer. Fungsinya adalah untuk menyimpan update file dari repository GitHub yang telah dibuat.
![35](https://user-images.githubusercontent.com/92896798/138264362-d92cc8b3-a061-47f1-b686-7b1fef1438ed.PNG)
## **Buka Folder Menggunakan Git Bash**
![38](https://user-images.githubusercontent.com/92896798/138264531-f7a37672-1db3-4791-8ad1-23e9e4d7f4c0.jpeg)

Setelah berhasil membuat folder pada local disk komputer, buka folder tersebut dengan cara klik kanan lalu pilih Git Bash Here. Setelah itu, Command Prompt akan muncul seperti di bawah ini.
![42](https://user-images.githubusercontent.com/92896798/138264618-c2b7fc6f-1c76-4621-a209-86d9e07435c4.PNG)
## **Ubah Folder Menjadi Repository**
Setelah itu, ubah folder tersebut menjadi repository menggunakan perintah berikut:
```sh
git init
```
![41](https://user-images.githubusercontent.com/92896798/138264712-21f4a6c3-7680-4c39-acfc-345e8af96ef1.PNG)

## **Tambahkan File ke Repository**
Untuk bisa menambahkan file ke repository GitHub,perlu menerapkan langkah-langkah di bawah ini:

Buat file di folder yang sudah dibuat (tugas3). Contohnya, di sini membuat file javascript : index.php 
Buka GitBash lalu masukkan perintah berikut:
```
git add index.php
```
Perintah tersebut tidak akan menghasilkan output apa pun.

## **Buat Commit**

Selanjutnya, perlu membuat Commit. Commit berfungsi untuk menambahkan update file serta komentar. Jadi setiap kontributor bisa memberikan konfirmasi update file di proyek yang sedang dikerjakan. Masukkan perintah berikut untuk membuat Commit:
```sh
git commit -m "first commit"
```
bebas membuat nama Commit apa saja.

![27](https://user-images.githubusercontent.com/92896798/138264781-fbde0548-c154-4f9e-8eb2-b78a654b4b57.jpg)

## **Remote Repository Github**

Remote repository berfungsi untuk mengupload file yang telah di buat sebelumnya di local disk. Masukkan perintah berikut ini untuk melakukan remote repository:
```sh
git branch -M main
git remote add origin https://github.com/zahrasyifaannisa/tugas3.git
```
Perintah di atas tidak akan menghasilkan output apa pun.

## **Push ke GitHub**

Langkah terakhir adalah push ke GitHub Push ini berfungsi untuk mengupload hasil akhir dari langkah-langkah di atas. Masukkan perintah berikut untuk melakukan push ke GitHub:
```sh
git push -u origin main
```
Perintah di atas akan menampilkan pop up sign in GitHub.
<br>
login untuk melanjutkan proses push ke GitHub.
<p>

Jika proses login berhasil, akan muncul tampilan Command Prompt seperti di bawah:

![28](https://user-images.githubusercontent.com/92896798/138266812-d50a7521-4092-4216-8f3f-308cc5c1d457.jpg)

## **Cek File**

Setelah itu, cek repository yang telah di buat. akan mendapati file-file yang telah ditambahkan sebelumnya. Pada tutorial ini kami menambahkan tiga file, yaitu index.php, ScreenShot/, dan README.md.

![45](https://user-images.githubusercontent.com/92896798/138266956-eefe36a6-fa27-4b91-a26f-bbc74081c0c9.PNG)

## **Kesimpulan**

Cara menggunakan Git ini wajib diketahui dan dikuasai oleh semua developer karena akan sangat membantu dalam mengerjakan project pembuatan website. Demikian penjelasan tentang cara menggunakan Git. Jika masih ada pertanyaan, jangan sungkan untuk meninggalkan di kolom komentar. Jangan lupa juga subscribe untuk mendapatkan informasi terbaru dari kami.

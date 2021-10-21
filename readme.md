Cara Install Git dan Cara Menggunakan Git

Install Git

Instalasi Git di Windows memang tidak seperti di Linux yang ketik perintah langsung terinstal. Kita harus men-download dulu, kemudian melakukan ritual next>next>finish.

Download Git

Silahkan buka website resminya Git : https://git-scm.com/

klik kanan dan run as administrator file instaler Git yang sudah diunduh.

![s](./1.jpg)
Maka akan muncul infomasi lisensi Git, klik Next > untuk melanjutkan.
![s](./2.jpg)

Selanjutnya menentukan lokasi instalasi. Biarkan saja apa adanya, kemudian klik Next >> sampai muncul sebagai berikut:

Selanjutnya pemilihan emulator terminal. Pilih saja yang bawah, kemudian klik Next >.
![s](./12.jpg)
Setelah selesai, kita bisa langsung klik finish.
![s](./17.jpg)
Selamat, Git sudah terinstal di Windows. Untuk mencobanya, silahkan buka CMD atau PowerShell, kemudian ketik perintah

git --version

![s](./18.jpg)

Cara penggunaan Git
Setelah berhasil install ke Git, selanjutnya

Login Git

masukkan username & email Git menggunakan perintah di bawah ini. Lalu tekan ENTER jika sudah benar.

git config --global user.name "zahrasyifaannisa"
git config --global user.email zahra.gugum@gmail.com

Selanjutnya untuk memastikan proses login berhasil, masukkan perintah berikut.

git config --list

![s](./19.jpg)

Login Github

Langkah kedua menggunakan Git adalah harus login ke dalam website GitHub. Github dan Git memiliki hubungan khusus, yaitu Git yang berperan sebagai version control system dan Github menjadi hosting atau sebagai penyimpan kode pemrograman.

![s](./36.png)

Buat Repository

Setelah berhasil login ke GitHub, Anda bisa mulai membuat repository. Klik tombol New pada menu Repositories untuk membuat repository baru.

![s](./32.png)
Kemudian akan diarahkan pada halaman untuk membuat repository baru seperti gambar di bawah ini. perlu mengisi detail informasi berikut:

Nama Repository : digunakan untuk identitas repository yang dibuat.
Deskripsi Repository : berfungsi untuk deskripsi dari repository yang dibuat.
Jenis Repository : jenis repository dibagi menjadi Public dan Private. Ketika Anda mengatur repository menjadi Public, orang lain dapat melihat repository yang Anda buat. Sebaliknya, jika Anda mengaturnya sebagai Private, repository tersebut hanya bisa diakses oleh Anda. Setelah mengisi detail informasi di atas,
klik Create Repository.

Buat Folder pada Windows

Selanjutnya, perlu membuat folder pada local disk komputer. Fungsinya adalah untuk menyimpan update file dari repository GitHub yang telah dibuat.

![s](./35.png)

Buka Folder Menggunakan Git Bash

![s](./38.jpeg)
Setelah berhasil membuat folder pada local disk komputer, buka folder tersebut dengan cara klik kanan lalu pilih Git Bash Here. Setelah itu, Command Prompt akan muncul seperti di bawah ini.

![s](./42.png)
Setelah itu, ubah folder tersebut menjadi repository menggunakan perintah berikut:

git init

![s](./41.png)

Tambahkan File ke Repository

Untuk bisa menambahkan file ke repository GitHub,perlu menerapkan langkah-langkah di bawah ini:

Buat file di folder yang sudah dibuat (tugas3). Contohnya, di sini membuat file javascript : index.php Buka GitBash lalu masukkan perintah berikut:

git add index.php

Perintah tersebut tidak akan menghasilkan output apa pun.

Buat Commit

Selanjutnya, perlu membuat Commit. Commit berfungsi untuk menambahkan update file serta komentar. Jadi setiap kontributor bisa memberikan konfirmasi update file di proyek yang sedang dikerjakan. Masukkan perintah berikut untuk membuat Commit:

git commit -m "first commit"

bebas membuat nama Commit apa saja.

![s](./27.jpg)

Remote Repository Github

Remote repository berfungsi untuk mengupload file yang telah di buat sebelumnya di local disk. Masukkan perintah berikut ini untuk melakukan remote repository:

git branch -M main
git remote add origin https://github.com/zahrasyifaannisa/tugas3.git

Perintah di atas tidak akan menghasilkan output apa pun.

Push ke GitHub

Langkah terakhir adalah push ke GitHub Push ini berfungsi untuk mengupload hasil akhir dari langkah-langkah di atas. Masukkan perintah berikut untuk melakukan push ke GitHub:

git push -u origin main

Perintah di atas akan menampilkan pop up sign in GitHub.
login untuk melanjutkan proses push ke GitHub.

Jika proses login berhasil, akan muncul tampilan Command Prompt seperti di bawah:

![s](./28.jpg)

Cek File

Setelah itu, cek repository yang telah di buat. akan mendapati file-file yang telah ditambahkan sebelumnya. Pada tutorial ini kami menambahkan tiga file, yaitu index.php, ScreenShot/, dan README.md.

Kesimpulan

Cara menggunakan Git ini wajib diketahui dan dikuasai oleh semua developer karena akan sangat membantu dalam mengerjakan project pembuatan website. Demikian penjelasan tentang cara menggunakan Git. Jika masih ada pertanyaan, jangan sungkan untuk meninggalkan di kolom komentar. Jangan lupa juga subscribe untuk mendapatkan informasi terbaru dari kami.
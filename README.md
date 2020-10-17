# LatihanVCS

### TUTORIAL MENGGUNAKAN GIT

### INSTALASI GIT
* Download **Git**, buka website resminya Git `(git-scm.com)`.
* Kemudian unduh Git sesuai dengan arsitektur komputer kita. Bisa 32Bit atau 64bit.
* Selamat, Git sudah terinstal di Windows. Untuk mencobanya,silahkan buka **CMD** atau **PowerShell**, kemudian ketik perintah

``git --version``

![version git](https://user-images.githubusercontent.com/72775624/96338210-a3046a80-10b6-11eb-9c35-d6883f0a5b59.PNG)


### Menambahkan Global Config
* Pada saat pertama kali menggunakan git, lakukanlah konfigurasi ``user.name dan user.email``
* konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.

* apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah `git commit`

* Config Global Repository

* Seperti pada gambar dibawah ini

![config](https://user-images.githubusercontent.com/72775624/96338194-9aac2f80-10b6-11eb-9ea5-2f6e8f90037f.PNG)


### Membuat Reposiory Local

* Buka direktory aktif, misal: **e:\latihanVCS** (buka menggunakan Windows Explorer)
* klik kanan pada direktory aktif tersebut, dan pilih menu **Git Bash**, sehingga muncul git bash commad
* Buat direktory project praktikum pertama dengan nama **latihanvcs**
``$ mkdir latihanvcs
$ cd latihanvcs``
* Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah **cd** ``(change directory)``
* direktory aktif menjadi: **e:\latihanVCS\latihanvcs seperti pada gambar dibawah ini

![mkdir](https://user-images.githubusercontent.com/72775624/96338206-a0097a00-10b6-11eb-8ef6-8e31900fc8aa.PNG)


### Membuat Reposiory Local

* Jalankan perintah **git init**, untuk membuat repository local.
`$ git init`
* Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .**git**
* Pada direktori tersebut, semua perubahan pada `working directory` akan disimpan.

![git init](https://user-images.githubusercontent.com/72775624/96338197-9c75f300-10b6-11eb-894a-f067de4f928a.PNG)




### Menambahkan File baru pada repository

* Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)
* disini kita akan coba buat satu file bernama README.md (text file)
`$ echo “# LatihanVCS” >> README.md`
* File **README.md** berhasil dibuat.


### Menambahkan File baru pada repository

* Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.
`$ git add README.md`
* File **README.md** berhasil ditambahkan.

![git readme](https://user-images.githubusercontent.com/72775624/96338199-9d0e8980-10b6-11eb-8191-04e9e40ff742.PNG)

### `Commit` (Menyimpan perubahan ke database)

* Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit”
`$ git commit -m “Latihan VCS”`
* Perubahan berhasil disimpan.

![20201016_163326 1](https://user-images.githubusercontent.com/66506609/96244442-43339400-0fd0-11eb-8fdb-45032a8ec449.png)


### Membuat repository server

* Server reopsitory yang akan kita gunakan adalah (http://github.com)
* Anda harus membuat akun terlebih dahulu.
* Pada laman github, klik tombol start a project, atau
* Dari menu (icon +) klik New Repository


### Membuat repository server

* Isi nama repositorynya, misal: labpy1.
* lalu klik tombol Create repository

![vcs1](https://user-images.githubusercontent.com/72775624/96338207-a13aa700-10b6-11eb-9137-0e6a6fc169d7.PNG)


### Menambahkan Remote Repository

* Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.
* Untuk menambahkan remote repository server, gunakan perintah **git remote add origin [url]**
`$ git remote add origin https://github.com/aningkinanti/vcs.git`


### Push (Mengirim perubahan ke server)

* Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.
`$ git push -u origin master`
* Perintah ini akan meminta memasukkan username dan password pada akun github.com

![git remote](https://user-images.githubusercontent.com/72775624/96338203-9e3fb680-10b6-11eb-9221-ebd05f18b9d3.PNG)


### Melihat hasilnya pada server repository

* Buka laman github.com, arahkan pada repositorinya.

* Yang apabila berhasil akan menjadi seperti dibawah ini

![vcs2](https://user-images.githubusercontent.com/72775624/96338209-a26bd400-10b6-11eb-96a1-13f4fb3a660f.PNG)




### Clone Repository

* Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).
* Untuk melakukan cloning, gunakan perintah `git clone [url]`

![clone](https://user-images.githubusercontent.com/72775624/96338193-9849d580-10b6-11eb-9670-250e69a763e9.PNG)





### Author : Aning Kinanti - 312010364





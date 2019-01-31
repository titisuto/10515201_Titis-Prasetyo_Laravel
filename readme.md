# ARTIKEL PROJECT LARAVEL
**Oleh: Titis Prasetyo (10515201)**
**Kelas: ECL-9**
## Awal Pembuatan Project
1. Project web dengan menggunakan *framework* laravel merupakan bagian dari pembelajaran mata kuliah E-Commerce Lanjut pada mahasiswa Sistem Informasi semester 7.
2. Dalam pembuatan project ini, dibutuhkan beberapa tools seperti:
* Web browser
* PHP 7.1.3 keatas
* MySql
* Composer

Hal penting dalam memulai pembuatan project menggunakan *framework* laravel ini:
1. Tambahkan PHP kedalam path System Environment Variables. 
2. File laravel 5.7 dan Composer
3. Template **Admin LTE 2.3.11**.

## Memulai Pembuatan Project
**1. Instal Laravel**
Dengan menggunakan folder *fresh* laravel (yang sudah ada folder *vendor*nya) kemudian di *copy-paste* pada htdocs.

**2. Integrasi Template**
Dengan mendownload file template Admin LTE 2.3.11 kemudian mengextract dan mengambil hanya 3 foldernya saja, yaitu folder *bootstrap,plugins dan dist*. Kemudian, file dari folder-folder tersebut diambil sebagai tampilan dalam project yang sedang kita buat. Adapun file tersebut yaitu : header.blade.php , footer.blade.php dan index.blade.php kemudian dimodifikasi sesuai dengan panduan dan kebutuhan.
Dengan memanfaatkan *Command Prompt*, kita dapat melakukan pembuatan controller baru, tabel baru dsb.

**3. CRUD Pada Kelas dan Siswa**
Dalam membuat CRUD, artinya kita berhubungan dengan yang namanya *database*. Maka dari itu, hal yang pertama dilakukan adalah memodifikasi db connection pada project laravel kita kemudian membuat *database*nya. Kemudian melakukan *migration* untuk membuat tabel menggunakan *Command Prompt* dan mengisi tabel tersebut sesuai kebutuhan kemudian di*migrate*.

1. CRUD - Create Data
Tahap *create* ini berfungsi untuk menambahkan data kedalam *database*. Dengan cara memodifikasi tampilan views dan controller serta mengatur routes agar dapat memasukan data kedalam *database*.
Agar tampilan menjadi lebih menarik, ditambahkan validation form sebagai pengingat kepada *user* agar isi *field* tertentu tidak boleh kosong.
2. CRUD - Read Data
Dengan menggunakan php artisan dengan membuat model. Setelah dibuat, modifikasi model, controller dan view tersebut agar bisa menampilkan data yang ada di *dabtabase*.
3. CRUD - Update Data
Dengan memodifikasi views, controller dan routes nya agar proses update dapat berjalan.
4. CRUD - Delete Data
Dalam proses delete data, hanya menggubah controllernya saja dengan menambahkan *function destroy*.

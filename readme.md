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
Dalam membuat CRUD, artinya kita berhubungan dengan yang namanya *database*. Maka dari itu, hal yang pertama dilakukan adalah memodifikasi db connection pada project laravel kita kemudian membuat *database*nya. Kemudian melakukan *migration* untuk membuat tabel menggunakan *Command Prompt* dan mengisi tabel tersebut sesuai kebutuhan kemudian di*migrate*. Sama halnya dengan tabel siswa, diperlukan relasi antara tabel siswa dengan tabel kelas. Dengan menggunakan laravel, tidak perlu menggunakan sintaks query join. Melainkan dengan memanfaatkan fitur laravel yaitu *Relationship Eloquent*.

1. CRUD - Create Data,
Tahap *create* ini berfungsi untuk menambahkan data kedalam *database*. Dengan cara memodifikasi tampilan views dan controller serta mengatur routes agar dapat memasukan data kedalam *database*.
Agar tampilan menjadi lebih menarik, ditambahkan validation form sebagai pengingat kepada *user* agar isi *field* tertentu tidak boleh kosong.
2. CRUD - Read Data,
Dengan menggunakan php artisan dengan membuat model. Setelah dibuat, modifikasi model, controller dan view tersebut agar bisa menampilkan data yang ada di *dabtabase*.
3. CRUD - Update Data,
Dengan memodifikasi views, controller dan routes nya agar proses update dapat berjalan.
4. CRUD - Delete Data,
Dalam proses delete data, hanya menggubah controllernya saja dengan menambahkan *function destroy*.

**4. Membuat Menu Login**
Login dibuat untuk memberikan hak akses terhadap seseorang untuk mengakses halaman web tersebut. Maka dari itu, hal pertama yang dimodifikasi yaitu views dengan mengambil file login.html pada folder **Admin LTE 2.3.11** dan ubah nama filenya menjadi login.blade.php. Setelah itu, mengubah ../.. menjadi {{ asset("assets") }}. Setelah selesai, maka:
1. Mengubah routes untuk membuat autentifikasi.
2. Membuat tabel login dengan memanfaatkan *Command Prompt* migration dan memodifikasi file yang sudah dibuat sesuai dengan panduan dan kebutuhan dan melakukan migrate agar masuk kedalam *database* yang telah dibuat.
3. Membuat model untuk *user*.
4. Membuat *user* admin melalui Seeder dan memodifikasi file Seeder tersebut untuk menentukan *username* dan *password*.
5. Mengubah Seeder *database* menjadi file Seeder *login* kemudian melakukan db:seed untuk memasukan kedalam *database* agar tampilan awalnya adalah tampilan *login*.
6. Memodifikasi *controller* login agar *username* yang masuk dapat diarahkan kedalam root yang sudah ditentukan.

Setelah login dibuat, kita membuat tombol logout dengan memodifikasi tampilan template header.

**5. Membuat Menu Upload File**
Tahap awal dalam membuat uplaod file yaitu dengan mengkonfigurasikan storage nya. Hal tersebut dilakukan agar kita dapat mengetahui tempat penyimpanan hasil uploadan tersebut. Setelah melakukan konfigurasi, dibuat folder khusus upload sebagai tempat penyimpanan upload.
1. Membuat form upload file pada views siswa dan menambahkan *enctype="multipart-form-data"*
2. Membuat tambahan field di tabel kelas yang sudah dibuat dengan melakukan migration pada *Command Prompt* kemudian dimodifikasi sesuai kebutuhan dan melakukan migrate.
3. Memodifikasi model siswa agar muncul foto.
4. Mengubah Controller siswa agar dapat menentukan jenis file dan ukuran filenya.
5. Menampilkan hasil upload file (foto) tersebut pada views siswa.

Setelah selesai, dilakukan pengecekan di *database* dan *storage* yang telah kita buat.

**Selesai**
* Credit: Terima Kasih Kepada Dosen Pembina, Bapak Ferry Stephanus Suwita, S.Kom, M.T dalam membimbing dan menerbitkan modul tutorial Laravel.

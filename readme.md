# SIAK OG-Modul Human Resource

Modul Human Resource adalah sistem yang terpisah dari SIAK, yang digunakan untuk pencatatan administrasi staf, baik dosen (staf akademik), maupun staf pendukung. Modul ini digunakan untuk menambahkan data staf baru, menghitung gaji dosen berdasarkan sks dan kehadiran di kelas, dan sebagainya.
, merupakan program yang menggunakan Spring Framework
### Petunjuk Instalasi
- Clone repo ini
- Start server XAMPP, aktifkan Apache dan MySQL
- Create Database tapsp,
- Masuk ke database tapsp
- Import database DumpSql.sql(yang ada di repo) pada database Anda melalui localhost/phpmyadmin atau cmd
- Buka Eclipse, klik kanan pada project TA-Kelompok1-HR-C dan run as spring boot app
- Buka browser Anda dan jalankan program pada browser melalui link localhost:9090
- Registrasikan diri Anda sesuai dengan form yang ditampilkan. Isi prodi dengan angka 1(dikarenakan yang staf ada di db hanya prodi tersebut)
- Setelah selesai registrasi, sign in ke dalam modul HR menggunakan username dan password yang telah Anda daftarkan.
##Fitur-Fitur yang ada
- Sudah ada unit testing
- Add staf
- Update Staf
- Lihat Staf
- Lihat staf dalam per prodi
- Lihat staf dalam per univ
- Lihat staf dalam per fakultas
- Lihat gaji staf per orang
- Lihat laporan pembayaran gaji staf-staf dalam rentang bulan dan tahun
- Hapus Staf
- Lihat gaji standar
- Update Gaji Standar
- Login Logout
- Validasi Page
- Rest Staf(get list dan model) dan kehadiran Dosen(add, update dan get)
- Register dan Bcrypt
- Css Template

*Note gaji dihitung berdasarkan gaji standar yang sesuai dengan role dia. Tetapi, jika role merupakan dosen maka gaji akan ditambahkan berdasarkan data
kehadiran sks * 50.000, yang kehadiran sks dihitung jika dia datang pada bulang tertentu(yang dalam db contoh kehadiran dosen yang ada hanya dosen dengan nama anto dengan role dosen, dimana kehadirannya ada pada bulan januari 2017, silahkan lihat perbedaan gaji pada waktu tersebut dengan waktu lainnya)
 
Gaji akan ada mulai dengan tahun 2016 bulan januari. Jika dilihat dalam view staf maka gaji akan diretrive dari tahun 2016 sampai sistem berjalan saat itu.
Tetapi, untuk dosen, jika ada kehadiran dosen yang diinput dari batas sistem berjalan, maka waktu akan diretrieve sampai waktu kehadiran dosen tersebut. 


Author: Kelompok 1D PSP 2016
- Afiq Rasyid Muhammad
- Clarissa Martalin
- Muhammad Luqman Hakim


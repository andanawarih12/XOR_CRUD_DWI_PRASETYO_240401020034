Nama		: Dwi Prasetyo Andana Warih
Kelas		: IF502
NIM		: 240401020034
Mata Kuliah	: Kriptografi dan Steganografi
PJJ S1 Informatika

Tugas ini saya memilih untuk menggunakan PHP + MySQL dengan tambahan fitur enkripsi XOR untuk menyimpan data ke database dalam bentuk terenkripsi.

1. untuk fitur aplikasinya:
	- Tambah data (Create)
	- Tampilkan data (Read)
	- Ubah data (Update)
	- Hapus data (Delete)
	- Enkripsi data sebelum masuk ke database (XOR)
	- Dekripsi data saat ditampilkan di halaman web
	- Pencatatan aktivitas enkripsi/dekripsi ke file log

2. List file:
	- index.php
	- create.php
	- update.php
	- delete.php
	- koneksi.php
	- rahasia_ilahi.php (fungsi XOR)
	- Aktivitas_Log.txt (tampilkan log yang terenkripsi/dekripsi)
	- tugas_dwi.sql (file export sql)

3. Penjelasan:
	rahasia_ilahi.php 
		- berisi fungsi xor_crypt untuk enkripsi dan dekripsi
		- fungsi write_log untuk mencatat log

	create.php
		- menerima input dari form
		- mengenkripsi input
		- menyimpan ke database

	index.php
		- mengambil data dari database
		- mendekripsi menggunakan fungsi xor_crypt
		- menampilkan ke halaman web

	update.php
		- menampilkan data yang sudah didekripsi
		- mengupdate data dengan terenkripsi

	delete.php
		- menghapus data berdasarkan id

	dump.sql
		- file hasil export database

4. panduan menjalankan aplikasi
	- install xampp, lalu jalankan apache dan MySQL sampai hijau
	
5. pada tugas ini saya membuat folder dwi_240401020034 untuk menyimpan file-file php saya di htdocs.
6. cara menjalankan MySQL nya dengan memanggil http://localhost/phpmyadmin/ di browser
7. setelah itu saya membuat database dengan nama : tugas_dwi
8. lalu saya membuat tabel dengan nama daftar_idola dengan isian tabel terdiri dari:
	- kolom id
	- kolom nama
	- kolom idola
9. lalu saya membuat file-file php yang dibutuhkan
10.setelah selesai semua saya menjalankan aplikasi saya dengan memanggil http://localhost/dwi_240401020034/create.php
11.setelah itu untuk mengecek isian tabel ada di link http://localhost/dwi_240401020034/index.php

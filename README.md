Modul Praktikum Flutter
Pembuatan Form Login dan Registrasi Interaktif

1. Validasi Input: Tambahkan validasi yang lebih baik. Misalnya, cek apakah email
memiliki format yang benar (mengandung ’@’) atau password memiliki panjang
minimal 6 karakter.
![7](https://github.com/user-attachments/assets/e98d3357-5826-4569-a873-22ea7e9b514f)
<img width="1660" height="1340" alt="carbon (4)" src="https://github.com/user-attachments/assets/affc1aea-e84c-460e-bf71-6d3188a6314d" />

- jika login gagal 
![8](https://github.com/user-attachments/assets/413c43aa-25d2-43f4-8b0b-c5230f7c977a)

2. Tampilkan/Sembunyikan Password: Tambahkan ikon mata pada TextField
password yang bisa ditekan untuk menampilkan atau menyembunyikan teks pass
word.
- Bagian login
<img width="1712" height="1192" alt="carbon (5)" src="https://github.com/user-attachments/assets/bb9948a8-2e11-4dfd-99fc-15131e83317e" />

hasil
![Uploading 7.jpg…]()

-Bagian regristrasi
<img width="1354" height="894" alt="carbon (6)" src="https://github.com/user-attachments/assets/7a66ce68-b98a-484f-af3f-27ae7f2514f9" />

hasil
![2](https://github.com/user-attachments/assets/80ce4e4b-a79b-46a3-86c7-a19295b393ca)

3. Animasi Sederhana: Tambahkan Hero widget pada ikon di halaman login dan
registrasi agar ada transisi animasi yang halus.
-hero diregrister
<img width="964" height="744" alt="carbon (7)" src="https://github.com/user-attachments/assets/681a77f6-9cac-4a47-b526-c1cf6f7b20f2" />

-hero di login
<img width="980" height="670" alt="carbon (8)" src="https://github.com/user-attachments/assets/1e6b8bd4-a3ac-4194-9c47-a8329cca64bd" />

4. Simpan Sesi Login: Coba gunakan package shared_preferences untuk me
nyimpan status login. Jadi, saat aplikasi ditutup dan dibuka lagi, pengguna tidak
perlu login ulang jika sesinya masih aktif.
-login
<img width="1508" height="520" alt="carbon (12)" src="https://github.com/user-attachments/assets/958fae48-15d3-4bda-ae7b-663db81a5a86" />

-main
<img width="1626" height="1712" alt="carbon (9)" src="https://github.com/user-attachments/assets/2705f0a6-e8be-45e5-9747-796cb43457a5" />

Untuk mengarahkan pengguna kembali ke halaman login dan mencegah mereka kembali ke halaman sebelumnya dengan tombol back, gunakan navigasi yang menghapus semua riwayat halaman, misalnya dengan pushNamedAndRemoveUntil. Dengan cara ini, saat pengguna logout atau sesi berakhir, halaman lama tidak tersisa di stack, sehingga tombol back tidak bisa membawa pengguna kembali ke halaman sebelumnya.
<img width="1456" height="744" alt="carbon (10)" src="https://github.com/user-attachments/assets/f6937227-2bc8-40ea-bb55-6b01980c23e0" />

Baris shared_preferences di dalam pubspec.yaml ditambahkan agar Flutter bisa menggunakan package tersebut untuk menyimpan data sederhana seperti status login ke penyimpanan lokal. Jika tidak dicantumkan, aplikasi tidak bisa mengakses library itu karena Flutter tidak tahu sumber dependensinya.
<img width="1508" height="1340" alt="carbon (11)" src="https://github.com/user-attachments/assets/1b4fa34a-c757-4148-abe0-1c0e24e639b1" />

hasil
![5](https://github.com/user-attachments/assets/a2e7a87a-7fa5-4e78-8af9-cf666c87d127)



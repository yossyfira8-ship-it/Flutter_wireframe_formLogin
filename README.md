Modul Praktikum Flutter
Pembuatan Form Login dan Registrasi Interaktif
Wireframe

1. Validasi Input: Tambahkan validasi yang lebih baik. Misalnya, cek apakah email
memiliki format yang benar (mengandung ’@’) atau password memiliki panjang
minimal 6 karakter.
-regristrasi gagal karna password yang kurang dari 6 karakter.
![6](https://github.com/user-attachments/assets/e6206957-d53a-48fe-84a2-494eb8c8be66)

- regristrasi berhasil karna sudah memiliki password panjang minimal 6 karakter
![3](https://github.com/user-attachments/assets/11ba3cf4-d704-4367-9227-80b4efda5d8a)

2. Tampilkan/Sembunyikan Password: Tambahkan ikon mata pada TextField
password yang bisa ditekan untuk menampilkan atau menyembunyikan teks pass
word.
- login
![4](https://github.com/user-attachments/assets/870a7c53-9c62-4c9f-8628-fcb79520eadd)

- sign up
![2](https://github.com/user-attachments/assets/88ebb95d-f2eb-4665-baa4-6e1632e20301)

3. Animasi Sederhana: Tambahkan Hero widget pada ikon di halaman login dan
registrasi agar ada transisi animasi yang halus.
<img width="726" height="596" alt="carbon (3)" src="https://github.com/user-attachments/assets/5d4af271-3aff-411e-bb1e-98ec64a1266b" />


5. Simpan Sesi Login: Coba gunakan package shared_preferences untuk me
nyimpan status login. Jadi, saat aplikasi ditutup dan dibuka lagi, pengguna tidak
perlu login ulang jika sesinya masih aktif.

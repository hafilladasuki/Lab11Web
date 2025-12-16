# Praktikum 12 – Autentikasi & Session (PHP OOP)

## Deskripsi Singkat

Praktikum ini membahas pembuatan **sistem login dan logout** menggunakan **session PHP** untuk membatasi akses ke halaman tertentu (modul artikel). Hanya user yang sudah login yang dapat mengakses halaman artikel.

---

## Tujuan

* Memahami konsep autentikasi
* Memahami penggunaan session di PHP
* Mengamankan halaman dengan login

---

## Struktur Folder Utama

```
lab11_php_oop/
├── index.php
├── config.php
├── class/
├── module/
│   ├── home/
│   ├── artikel/
│   └── user/
│       ├── login.php
│       └── logout.php
└── template/
```

---

## Database

Membuat tabel `users` untuk menyimpan data admin.

```sql
CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(50),
  password VARCHAR(255),
  nama VARCHAR(100)
);
```

Insert user admin dengan password terenkripsi.

---

## Alur Autentikasi

1. User membuka halaman artikel
2. Jika belum login → diarahkan ke halaman login
3. User login menggunakan akun admin
4. Jika berhasil → masuk ke halaman artikel
5. User dapat logout untuk mengakhiri session

---

## Login & Logout

* **Login**: validasi username dan password menggunakan `password_verify()`
* **Logout**: menghapus session dan kembali ke halaman login

---

## Pengujian

1. 

https://github.com/user-attachments/assets/0742a76c-9531-4974-8b79-666428e1fe83



dan di vidio tersebut beserta dengan tugas menambahkan fitur home untuk mengganti password

## Kesimpulan

Dengan autentikasi dan session, aplikasi menjadi lebih aman karena akses halaman admin dibatasi hanya untuk user yang sudah login.



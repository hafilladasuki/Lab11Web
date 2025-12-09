# Lab 11 web


#  **README — Praktikum 11: PHP OOP**

## **1. Deskripsi Singkat**

Project ini merupakan hasil Praktikum 11 Pemrograman Web yang membahas **PHP OOP**, **modularisasi**, dan **routing sederhana** menggunakan mini–framework buatan sendiri.
Semua halaman dibagi ke dalam modul, dan router mengarahkan URL ke file modul secara otomatis.

---

## **2. Struktur Folder**

```
lab11_php_oop/
├── assets/css/style.css
├── auth/
│   ├── login.php
│   └── logout.php
├── class/
│   ├── Database.php
│   └── Form.php
├── module/
│   ├── artikel/
│   │   ├── index.php
│   │   ├── tambah.php
│   │   └── ubah.php
│   └── home/index.php
├── template/
│   ├── header.php
│   ├── footer.php
│   └── sidebar.php
├── user/
│   ├── add.php
│   └── list.php
├── .htaccess
├── config.php
└── index.php
```

---

## **3. Cara Kerja Routing**

Router membaca URL:

```
/modul/halaman
```

Contoh:

* `/home/index` → `module/home/index.php`
* `/artikel/index` → `module/artikel/index.php`
* `/artikel/tambah` → `module/artikel/tambah.php`

Jika tidak ada path, otomatis membuka:

```
/home/index
```

---

## **4. File Penting**

* **index.php** → router utama
* **class/Database.php** → koneksi & query database
* **class/Form.php** → helper form OOP
* **template/** → header, footer, sidebar
* **module/** → isi halaman

---

## **5. Menjalankan Project**

1. Taruh folder dalam:

   ```
   C:/xampp/htdocs/lab11_php_oop/
   ```
2. Aktifkan Apache & MySQL.
3. Akses melalui browser:

```
http://localhost/lab11_php_oop/
```

---

## **6. Kesimpulan**

Praktikum ini berhasil membuat sistem modular sederhana menggunakan konsep PHP OOP, routing, template, dan class helper untuk form & database.

---

<p><img width="526" height="334" alt="Screenshot 2025-12-10 000125" src="https://github.com/user-attachments/assets/0dd46b3e-fbad-48ed-b8e9-0990fc6c38b3" />
</p>

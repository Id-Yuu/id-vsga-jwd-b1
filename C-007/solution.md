# Solution
Kisi-kisi tugas 7 dalam membuat website crud perpustakaan sederhana dengan sistem login.

## Structure Files 1
Kita bisa membuat struktur terpisah, untuk mempermudah pengeditan.
```sh
Course-007
 ┣ functions
 ┃ ┣ connection.php
 ┃ ┣ login.php
 ┃ ┗ logout.php
 ┣ pages
 ┃ ┣ anggota
 ┃ ┃ ┣ add_data.php
 ┃ ┃ ┣ delete_data.php
 ┃ ┃ ┣ edit_data.php
 ┃ ┃ ┗ m_anggota.php
 ┃ ┣ buku
 ┃ ┃ ┣ add_data.php
 ┃ ┃ ┣ delete_data.php
 ┃ ┃ ┣ edit_data.php
 ┃ ┃ ┗ m_buku.php
 ┃ ┗ transaksi
 ┃ ┃ ┣ add_data.php
 ┃ ┃ ┣ delete_data.php
 ┃ ┃ ┣ edit_data.php
 ┃ ┃ ┗ m_transaksi.php
 ┣ index.php
 ┗ main.php
```

## Structure Files 2
Atau kita bisa membuat 1 function `add_data`, `edit_data`, `delete_data` yang akan dipanggil sesuai dengan kondisi yang dibutuhkan.
```sh
Course-007
 ┣ db
 ┃ ┗ connection.php
 ┣ functions
 ┃ ┣ add_data.php
 ┃ ┣ delete_data.php
 ┃ ┣ edit_data.php
 ┃ ┣ login.php
 ┃ ┗ logout.php
 ┣ pages
 ┃ ┣ anggota
 ┃ ┃ ┗ m_anggota.php
 ┃ ┣ buku
 ┃ ┃ ┗ m_buku.php
 ┃ ┗ transaksi
 ┃ ┃ ┗ m_transaksi.php
 ┣ index.php
 ┗ main.php
```

## Ketentuan
| File | Keterangan |
| ------------- | ------------- |
|index|Untuk login|
|main|Untuk dashboard|

## Ketentuan Lain
- `m_anggota`, `m_buku`, `m_transaksi` akan menampilkan tabel berisi data dari database, dan <br>
menampilkan tombol aksi `edit` & `delete`,
- Masing-masing pages memiliki tombol `add` pada atas tabel,
- Masing-masing pages menggunakan fungsi php `Session`, 
- Database memiliki relasi antar tabel pada `m_transaksi`, <br>
gunakan `Primary key` & `Foreign Key` pada database.

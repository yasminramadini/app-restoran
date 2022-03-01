## Aplikasi pesan makanan restoran dengan Vue JS dan Laravel 8

Aplikasi ini memungkinkan pelanggan untuk memesan makanan melalui website restoran. Pelanggan dapat melihat daftar menu, membaca detail menu, kemudian memesannya dan akan muncul di halaman pesanan. Lalu user dengan tipe koki dapat melihat daftar pesanan baru dan menandainya sudah diantar setelah pesanannya diantar pada pelanggan. Lalu user bertipe admin dapat mengelola data menu, kategori, satuan, dan user. 

## Teknologi yang dipakai
- frontend: Vue CLI
- backend: Laravel 8

## Cara menggunakan projek
- clone repository ini
- masuk folder backend, lalu lakukan:
  - ketik cp .env.example .env
  - ketik composer install
  - ketik php artisan key:generate
  - buka .env, setting sesuai database kamu
  - jalankan migrasi dengan mengetik php artisan migrate
  - jalankan server dengan php artisan serve
- masuk folder frontend, lalu lakukan:
  - ketik npm run serve untuk menjalankan aplikasi Vue Js
  - akses halaman register: http://localhost:8080/register
  - untuk membuat akun admin pertama kali harus ubah manual di database. buka table users lalu ubah rolenya jadi 1. lalu buka table personal_access_tokens lalu ubah abilities-nya jadi ["admin"]

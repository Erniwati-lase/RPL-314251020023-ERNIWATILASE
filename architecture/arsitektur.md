# Arsitektur Sistem Akademik Kampus

## Pola/Gaya Arsitektur yang Digunakan
 Sistem Akademik Kampus menggunakan Layered Architecture (Arsitektur Berlapis) dengan pola Client-Server.

### Layered Architecture
Arsitektur ini membagi sistem ke dalam beberapa lapisan (layer) yang memiliki tanggung jawab berbeda:

  * Presentation Layer (UI/Front-End). 
Antarmuka web yang digunakan mahasiswa, dosen, dan admin untuk berinteraksi dengan sistem.

  * Application Layer (Business Logic)  
Menangani aturan bisnis kampus, seperti validasi KRS, perhitungan IPK, dan pengelolaan jadwal kuliah.

  * Data Access Layer  
Bertugas menghubungkan aplikasi dengan database, termasuk query data mahasiswa, mata kuliah, dan nilai.

  * Database Layer  
Menyimpan seluruh data akademik secara terstruktur (misalnya menggunakan MySQL/PostgreSQL).



### Client-Server
  * Client: Browser mahasiswa, dosen, dan admin yang mengakses sistem melalui antarmuka web.

  * Server: Menjalankan aplikasi utama, memproses permintaan, dan mengelola data di database.



### Alasan Pemilihan
  * Keterpisahan Tanggung Jawab: Layered architecture memudahkan pengembangan dan pemeliharaan karena setiap lapisan memiliki fungsi spesifik.

  * Skalabilitas: Sistem dapat dikembangkan lebih lanjut, misalnya menambahkan modul keuangan atau integrasi dengan sistem e-learning.

  * Keamanan: Dengan client-server, data sensitif tetap tersimpan di server, bukan di perangkat pengguna.

  * Kemudahan Akses: Mahasiswa dan dosen cukup menggunakan browser tanpa perlu instalasi aplikasi tambahan.

  * Fleksibilitas Pengembangan: Layered architecture memungkinkan tim IT kampus untuk memperbarui satu lapisan tanpa mengganggu lapisan lain.
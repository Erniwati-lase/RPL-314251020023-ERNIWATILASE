# Physical View – Sistem Akademik Kampus

## Gambaran Infrastruktur Fisik / Deployment

### Server

1. Application Server  
Menjalankan aplikasi utama (business logic, API, autentikasi).
Bisa berupa server fisik di data center kampus atau VM di cloud (misalnya AWS/Google Cloud/Azure).
2. Web Server  
Menangani permintaan HTTP/HTTPS dari browser mahasiswa, dosen, dan admin.
Biasanya menggunakan reverse proxy (misalnya Nginx/Apache) untuk load balancing.

### Database
1. Database Server  
Menyimpan data akademik (mahasiswa, dosen, mata kuliah, KRS, nilai).
Menggunakan RDBMS seperti MySQL/PostgreSQL.
2. Backup Database  
Server cadangan untuk replikasi data dan pemulihan jika terjadi kegagalan.

### Jaringan
1. LAN Kampus  
Menghubungkan komputer dosen/admin ke server internal.
2. Internet  
Mahasiswa mengakses sistem melalui jaringan publik dengan protokol HTTPS.
3. Firewall & Security Gateway  
Melindungi server dari serangan eksternal.
4. VPN (opsional)  
Untuk akses aman bagi staf kampus dari luar jaringan kampus.

### 4. Komponen Tambahan
1. Load Balancer  
Membagi beban trafik ke beberapa server aplikasi agar sistem tetap responsif.
2. File Storage Server  
Menyimpan dokumen akademik (misalnya transkrip, laporan, materi kuliah).
3. Monitoring & Logging Server  
Memantau performa sistem, mencatat aktivitas, dan mendeteksi anomali.


## Hubungan Antar Komponen
* Client (Browser Mahasiswa/Dosen/Admin) → mengakses Web Server melalui internet/LAN.
* Web Server → meneruskan permintaan ke Application Server.
* Application Server → berinteraksi dengan Database Server untuk membaca/menulis data.
* Database Server → melakukan sinkronisasi dengan Backup Database.
* Load Balancer → mendistribusikan trafik ke beberapa Application Server.
* Firewall → mengontrol akses dari luar ke dalam sistem.
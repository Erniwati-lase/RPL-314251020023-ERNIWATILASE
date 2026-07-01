# Quality Attributes – Sistem Akademik Kampus

## Performance (Kinerja)
1. Sistem harus mampu merespons cepat saat ribuan mahasiswa mengakses jadwal, KRS, atau nilai secara bersamaan.
2. Optimasi query database dan caching diperlukan agar waktu respon tetap rendah.

## Security (Keamanan)
1. Data pribadi mahasiswa dan dosen harus terlindungi dari akses tidak sah.
2. Diperlukan autentikasi peran (mahasiswa, dosen, admin) dan enkripsi komunikasi antar server.

## Scalability (Skalabilitas)
1. Sistem harus dapat diperluas untuk menampung jumlah pengguna yang meningkat setiap tahun.
2. Arsitektur modular dan dukungan cloud memungkinkan penambahan server tanpa gangguan layanan.

## Usability (Kemudahan Penggunaan)
1. Antarmuka harus intuitif agar mahasiswa dan dosen dapat menggunakan sistem tanpa pelatihan khusus.
2. Navigasi sederhana dan konsisten meningkatkan efisiensi penggunaan.

## Reliability (Keandalan)
1. Sistem harus tetap berfungsi dengan baik selama periode penting seperti pengisian KRS dan input nilai.
2. Mekanisme backup dan recovery diperlukan untuk mencegah kehilangan data.

## Maintainability (Kemudahan Pemeliharaan)
1. Struktur kode dan dokumentasi harus jelas agar tim pengembang kampus mudah melakukan perbaikan atau penambahan fitur.
2. Penggunaan layered architecture membantu isolasi perubahan antar komponen.

## Availability (Ketersediaan)
1. Sistem harus online 24/7, terutama saat masa registrasi akademik.
2. Diperlukan redundansi server dan monitoring otomatis untuk menjaga uptime tinggi
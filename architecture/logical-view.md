

# Logical View – Sistem Akademik Kampus

 ## Gambaran Komponen/Modul Logis

Sistem Akademik Kampus dibagi menjadi beberapa komponen logis yang saling berhubungan:

### User Interface (UI)

 * Antarmuka web untuk mahasiswa, dosen, dan admin.
 * Menyediakan form login, menu KRS, jadwal kuliah, input nilai, dan laporan.

### Authentication & Authorization Module

 * Mengelola login dan hak akses.
 * Mahasiswa, dosen, dan admin memiliki peran berbeda.

### Academic Management Module

 * KRS Management: Mahasiswa memilih mata kuliah.
 * Course Validation: Sistem memvalidasi ketersediaan mata kuliah.
 * Schedule Management: Admin mengatur jadwal kuliah.

### Grading Module

 * Dosen menginput nilai.
 * Sistem menghasilkan transkrip otomatis.

### Reporting Module

 * Menyediakan laporan akademik untuk admin kampus (jumlah mahasiswa aktif, IPK rata-rata, dsb.).

### Database Module

 * Menyimpan data mahasiswa, dosen, mata kuliah, nilai, dan jadwal.
 * Berkomunikasi dengan modul lain melalui Data Access Layer.

## Hubungan Antarmodul
 * UI ↔ Authentication Module → Validasi login dan hak akses.
 * UI ↔ Academic Management Module → Mahasiswa/dosen/admin berinteraksi dengan fitur akademik.
 * Academic Management Module ↔ Database Module → Query data mahasiswa, mata kuliah, jadwal.
 * Grading Module ↔ Database Module → Input nilai dan generate transkrip.
 * Reporting Module ↔ Database Module → Menarik data untuk laporan.
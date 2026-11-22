GULO - GERAKAN UMKM LOKAL
Browser Edition v2.0 - Developed by GFLM

CARA MENJALANKAN
1. Ekstrak ZIP.
2. Buka index.html menggunakan Chrome atau Edge terbaru.
3. Login dengan akun Administrator yang sudah Anda miliki.
4. Backup data lokal sebelum mengganti file aplikasi.

PEMBARUAN
- Perombakan tampilan Daftar Akun UMKM: banner, kartu statistik, tabel, filter, status, dan tombol tindakan.
- Layout responsif desktop dan ponsel.
- Tabel mobile berubah menjadi kartu informasi.
- Keamanan browser-side diperkuat: PBKDF2-HMAC-SHA256 310.000 iterasi untuk password baru.
- Hash lama (120.000 iterasi) diperbarui otomatis ke 310.000 iterasi setelah login berhasil.
- Salt acak baru untuk password baru dan migrasi hash.
- Content Security Policy meta, referrer policy, dan pembatasan permission browser.
- Nilai teks pengguna di-escape saat ditampilkan pada daftar/detail.
- Karakter em dash/en dash diganti tanda hubung biasa.

BATASAN KEAMANAN PENTING
Browser Edition adalah aplikasi lokal satu perangkat. Data disimpan di localStorage/sessionStorage dan kode HTML/JavaScript dapat diperiksa atau dimodifikasi oleh pemilik perangkat. Admin role, daftar akun, dan lisensi lokal tidak dapat dianggap aman terhadap pengguna yang memiliki akses DevTools atau file aplikasi.
Jangan gunakan versi ini untuk layanan publik multi-pelanggan atau menyimpan data keuangan sensitif yang memerlukan jaminan keamanan. Untuk produksi, wajib migrasi autentikasi, otorisasi, lisensi, dan database ke backend server; gunakan HTTPS, password hashing Argon2id/bcrypt pada server, rate limiting, session cookie HttpOnly/Secure/SameSite, validasi server-side, audit log, backup terenkripsi, dan pemisahan tenant di database.

DATA
Data akun dan workspace tersimpan di browser yang sama. Hapus cache/site data dapat menghilangkan data. Gunakan fitur backup aplikasi sebelum update.

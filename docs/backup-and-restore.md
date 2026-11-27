# Backup dan restore

Backup di AturMyDuit adalah snapshot file database, bukan sinkronisasi ke
server. Semua proses berjalan lokal.

## Membuat backup

1. Buka **Pengaturan**, lalu **Backup & Restore**.
2. Tekan **Buat backup**.
3. Pilih lokasi penyimpanan lewat dialog file sistem.
4. Tunggu sampai muncul pesan berhasil.

Backup memakai `VACUUM INTO`, sehingga file yang dihasilkan konsisten walau
database sedang dipakai. Jangan menyalin file database yang sedang terbuka
secara manual.

## Memulihkan backup

1. Buka **Backup & Restore**.
2. Tekan **Restore dari file**.
3. Pilih file backup `.sqlite`.
4. Konfirmasi.

Urutan yang dijalankan aplikasi:

1. File dibaca ke folder sementara.
2. Isi SQLite, integritas, dan versi schema divalidasi.
3. Snapshot pengaman database lama dibuat.
4. Database ditutup, lalu file backup menggantikan database aktif.
5. File pendamping database dihapus, database dibuka, dan migrasi dijalankan.
6. Provider data dimuat ulang.

Kalau restore gagal setelah penggantian, aplikasi mengembalikan snapshot
pengaman. File yang bukan backup AturMyDuit atau schema-nya terlalu baru akan
ditolak.

## Riwayat backup

Halaman Backup menampilkan riwayat keberhasilan dan kegagalan. Gunakan riwayat
ini untuk memastikan backup terakhir benar-benar dibuat.

## Saran

- Backup rutin, misalnya tiap akhir bulan.
- Simpan salinan di penyimpanan lain, bukan hanya di HP.
- Beri nama file yang mudah dikenali. Aplikasi memakai pola
  `aturmyduit-backup-YYYYMMDD-HHmmss.sqlite`.
- Jangan mengunggah file backup ke issue publik. File itu berisi seluruh data
  keuanganmu.
- Backup belum terenkripsi. Simpan di tempat yang aman.

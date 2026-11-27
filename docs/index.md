# Panduan AturMyDuit

AturMyDuit adalah pencatat keuangan pribadi untuk Android yang bekerja
sepenuhnya di perangkatmu. Tidak ada akun, tidak ada server, dan fitur inti
tetap jalan tanpa internet.

Panduan ini menjelaskan cara memakai setiap fitur di versi 1.0.0, dari
pemasangan sampai backup data.

## Daftar isi

1. [Memulai](getting-started.md)
2. [Kantong dan saldo](wallets.md)
3. [Transaksi](transactions.md)
4. [Budget dan tagihan](budget-and-bills.md)
5. [Laporan dan grafik](reports.md)
6. [Backup dan restore](backup-and-restore.md)
7. [Pengaturan](settings.md)
8. [Pertanyaan umum](faq.md)

## Prinsip aplikasi

- **Local-first.** Semua transaksi, kantong, budget, dan tagihan disimpan di
  database SQLite di HP-mu.
- **Saldo dari ledger.** Saldo kantong dihitung dari jumlah duit masuk
  dikurangi duit keluar, bukan angka yang diketik manual.
- **Tanpa akun.** Profil hanya nama dan foto yang tersimpan lokal.
- **Dua bahasa.** Indonesia dan English, bisa mengikuti bahasa sistem.
- **Offline.** Satu-satunya akses jaringan adalah pemeriksaan versi terbaru
  di halaman rilis.

## Butuh bantuan?

Buka [issue](https://github.com/s4ndrism/AturMyDuit-App/issues) di repo publik.
Sertakan versi aplikasi dari Tentang Aplikasi, tipe HP, dan versi Android.
Jangan lampirkan data transaksi pribadi atau file backup ke issue publik.

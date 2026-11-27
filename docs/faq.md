# Pertanyaan umum

## Apakah data saya diunggah ke server?

Tidak. Semua transaksi, kantong, budget, tagihan, dan profil disimpan di
database lokal di HP-mu. Tidak ada akun dan tidak ada sinkronisasi server.

Satu-satunya akses jaringan adalah pemeriksaan versi terbaru. Aplikasi membaca
metadata rilis publik di `api.github.com`. Tidak ada transaksi, identitas, atau
analytics yang dikirim.

## Apakah aplikasi bisa dipakai offline?

Bisa. Semua fitur inti berjalan tanpa internet. Hanya cek pembaruan yang butuh
koneksi, dan kegagalannya tidak menghalangi pemakaian.

## Kenapa saldo kantong tidak cocok?

Saldo dihitung dari ledger. Periksa:

1. transaksi pemasukan dan pengeluaran di kantong itu;
2. transfer masuk dan keluar, termasuk biaya admin;
3. baris penyesuaian "Saldo awal" dan koreksi saldo.

Kalau perlu, buat koreksi baru lewat halaman transaksi. Jangan mengedit riwayat
lama.

## Apakah transfer dihitung sebagai pengeluaran?

Tidak. Principal transfer hanya memindahkan duit antar kantong. Yang dihitung
sebagai pengeluaran adalah biaya admin.

## Bagaimana kalau duit tidak cukup?

Kantong menolak transaksi yang membuat saldo negatif, kecuali opsi **Izinkan
duit minus** diaktifkan.

## Bagaimana cara mengamankan data?

Buat backup lokal secara rutin lewat **Pengaturan > Backup & Restore**, lalu
simpan salinannya di tempat lain. Backup belum terenkripsi.

## Apakah APK tersedia di Play Store?

Untuk 1.0.0, APK dibagikan lewat halaman rilis GitHub. Unduh dari repo publik
`AturMyDuit-App`, cocokkan checksum, lalu pasang manual.

## Kenapa ada peringatan sumber tidak dikenal?

Android menampilkan peringatan itu untuk APK yang dipasang di luar Play Store.
Izinkan pemasangan dari sumber tidak dikenal hanya untuk aplikasi yang kamu
percaya.

## Apakah aplikasi ini gratis?

AturMyDuit gratis untuk pemakaian pribadi dan non-komersial. Kode sumber
bersifat proprietary. Donasi lewat Trakteer tidak wajib.

## Bagaimana cara melaporkan bug?

Buka [issue](https://github.com/s4ndrism/AturMyDuit-App/issues). Sertakan versi
aplikasi, tipe HP, versi Android, dan langkah untuk mereproduksi masalah.
Jangan lampirkan data transaksi pribadi atau file backup.

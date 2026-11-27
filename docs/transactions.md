# Transaksi

AturMyDuit mencatat tiga jenis transaksi: pemasukan, pengeluaran, dan
transfer. Semua perubahan langsung memperbarui saldo kantong terkait.

## Mencatat transaksi

1. Tekan tombol **+** di tengah navbar.
2. Pilih **Pemasukan**, **Pengeluaran**, atau **Transfer**.
3. Isi nominal, kantong, kategori, tanggal, dan catatan bila perlu.
4. Periksa pratinjau, lalu simpan.

Nominal selalu berupa rupiah penuh. AturMyDuit tidak memakai desimal.

## Pemasukan dan pengeluaran

- **Pemasukan** menambah saldo kantong. Contoh: gaji, bonus, freelance.
- **Pengeluaran** mengurangi saldo kantong. Contoh: makan, transport, listrik.
- Kategori memisahkan pemasukan dan pengeluaran. Kategori bisa ditambah,
  diurutkan, dan diarsipkan di Pengaturan.
- Kategori sistem **Biaya Admin** dipakai otomatis oleh transfer dan tidak
  bisa dihapus.

## Transfer

Transfer memindahkan duit antar kantong dalam satu operasi:

- Dua baris principal dibuat dengan satu grup: keluar dari kantong asal dan
  masuk ke kantong tujuan.
- Biaya admin, kalau ada, dicatat sebagai pengeluaran terpisah.
- Semua baris ditulis dalam satu database transaction, jadi tidak ada transfer
  setengah jadi.

Detail aturan ada di [Kantong dan saldo](wallets.md).

## Melihat dan mencari transaksi

Tab **Transaksi** menampilkan semua catatan duit:

- Cari berdasarkan nama transaksi, tempat, atau kategori.
- Filter berdasarkan kantong, kategori, dan periode (minggu ini, bulan ini,
  tahun ini, atau semua waktu).
- Ketuk satu transaksi untuk melihat detail.

## Edit, hapus, dan urungkan

- Transaksi bisa diedit dari halaman detail. Saldo kantong ikut disesuaikan.
- Menghapus transaksi akan mengembalikan saldo kantong.
- Penghapusan menyediakan tombol **Urungkan** sebelum data benar-benar hilang.
- Data terhapus tetap tersimpan sebagai soft delete sampai kamu membersihkannya
  lewat Pengaturan.

## Pembayaran tagihan

Pembayaran tagihan muncul sebagai transaksi pengeluaran. Kalau pembayaran
dibatalkan, transaksi ikut dihapus dan tagihan kembali berstatus belum dibayar.

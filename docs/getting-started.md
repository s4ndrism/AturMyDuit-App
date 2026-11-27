# Memulai

## Pasang aplikasi

1. Buka [halaman rilis](https://github.com/s4ndrism/AturMyDuit-App/releases/latest).
2. Unduh `AturMyDuit-1.0.0.apk` dan `SHA256SUMS.txt`.
3. Izinkan pemasangan dari sumber tidak dikenal di pengaturan Android.
4. Buka file APK, lalu selesaikan pemasangan.
5. Kalau mau, cocokkan checksum APK dengan isi `SHA256SUMS.txt`:

   ```powershell
   Get-FileHash AturMyDuit-1.0.0.apk -Algorithm SHA256
   ```

AturMyDuit hanya tersedia untuk Android. APK ditandatangani dengan keystore
rilis, jadi pembaruan berikutnya bisa dipasang di atas versi lama.

## Pertama kali dibuka

Saat pertama dibuka, AturMyDuit membuat satu kantong bernama **Cash** dengan
saldo nol. Kamu bisa langsung memakainya atau menambah kantong lain.

Urutan yang disarankan:

1. Buka **Kantong**, lalu isi duit awal di kantong yang kamu pakai.
2. Catat pemasukan atau pengeluaran pertama lewat tombol **+**.
3. Tentukan budget bulanan di tab **Budget**.
4. Tambahkan tagihan rutin kalau ada.
5. Atur profil, tema, dan bahasa di **Pengaturan**.

## Mengenal layar utama

- **Home**: sapaan, Total Duit, ringkasan transaksi, budget, dan tagihan.
- **Grafik**: laporan pemasukan dan pengeluaran.
- **Budget**: budget dan daftar tagihan.
- **Transaksi**: riwayat semua transaksi.
- **Tombol +** di tengah navbar: mencatat pemasukan, pengeluaran, atau
  transfer.
- **Ikon profil** di Home: membuka Pengaturan.

## Duit awal

Duit awal bukan kolom terpisah. Saat kamu mengisi saldo pertama, AturMyDuit
membuat baris penyesuaian bernama "Saldo awal". Koreksi saldo berikutnya juga
dibuat sebagai baris penyesuaian baru, jadi riwayat lama tidak berubah.

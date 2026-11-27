<div align="center">
  <img src="screenshots/app_logo.png" width="120" alt="Logo AturMyDuit" />

  <h1>AturMyDuit</h1>

  <p>
    <strong>Catat duit, atur kantong, dan pahami ke mana uangmu pergi.</strong><br />
    Local-first untuk Android. Tanpa akun, tanpa server, tetap jalan offline.
  </p>

  <p>
    <a href="https://github.com/s4ndrism/AturMyDuit-App/releases/latest"><img src="https://img.shields.io/github/v/release/s4ndrism/AturMyDuit-App?label=rilis&color=2ea44f" alt="Rilis terbaru" /></a>
    <a href="https://github.com/s4ndrism/AturMyDuit-App/releases"><img src="https://img.shields.io/github/downloads/s4ndrism/AturMyDuit-App/total?label=unduhan" alt="Unduhan" /></a>
    <img src="https://img.shields.io/badge/platform-Android-3DDC84?logo=android&logoColor=white" alt="Android" />
    <img src="https://img.shields.io/badge/bahasa-Indonesia%20%2F%20English-blue" alt="Bahasa" />
    <a href="LICENSE"><img src="https://img.shields.io/badge/lisensi-proprietary-red" alt="Lisensi" /></a>
    <a href="https://github.com/s4ndrism/AturMyDuit-App/stargazers"><img src="https://img.shields.io/github/stars/s4ndrism/AturMyDuit-App?style=flat" alt="Stars" /></a>
    <a href="https://github.com/s4ndrism/AturMyDuit-App/forks"><img src="https://img.shields.io/github/forks/s4ndrism/AturMyDuit-App?style=flat" alt="Forks" /></a>
    <a href="https://trakteer.id/s4ndrism"><img src="https://img.shields.io/badge/dukung-Trakteer-be1e2d" alt="Dukung lewat Trakteer" /></a>
  </p>

  <p>
    <a href="https://github.com/s4ndrism/AturMyDuit-App/releases/latest"><strong>Unduh APK</strong></a>
    ·
    <a href="docs/index.md"><strong>Panduan</strong></a>
    ·
    <a href="docs/en/index.md"><strong>English guide</strong></a>
    ·
    <a href="https://trakteer.id/s4ndrism"><strong>Trakteer</strong></a>
  </p>
</div>

## Kenapa AturMyDuit

- **Data milikmu.** Semua transaksi tersimpan di SQLite di HP-mu, bukan di
  server orang lain.
- **Saldo terhitung.** Saldo kantong berasal dari seluruh transaksi, bukan
  angka yang diketik manual.
- **Tetap jalan offline.** Fitur inti tidak butuh internet.
- **Tanpa akun.** Tidak ada login, tidak ada email, tidak ada profil di cloud.
- **Dua bahasa.** Indonesia dan English, bisa mengikuti bahasa sistem.

## Fitur

| Fitur | Yang bisa kamu lakukan |
|---|---|
| Kantong | Tambah bank, e-wallet, investasi, cash, atau kantong custom. Saldo dihitung dari riwayat transaksi. |
| Transaksi | Catat pemasukan, pengeluaran, dan transfer antar kantong lengkap dengan biaya admin. |
| Budget | Tentukan batas pengeluaran keseluruhan atau per kategori, lalu pantau realisasinya. |
| Tagihan | Atur tagihan harian, mingguan, bulanan, atau tahunan, dengan pengingat H-24 dan bayar otomatis. |
| Laporan | Lihat tren pemasukan dan pengeluaran, komposisi kategori, dan filter per kantong atau periode. |
| Backup | Buat snapshot database lokal, validasi saat restore, dan rollback kalau restore gagal. |
| Profil | Atur nama dan foto tanpa login Google. |
| Cek pembaruan | Dapat notifikasi versi baru di halaman rilis. Pemasangan APK tetap manual. |

## Dokumentasi

Panduan lengkap tersedia di dalam repo dan di dalam aplikasi, bisa dibuka
offline.

| Topik | Indonesia | English |
|---|---|---|
| Daftar isi | [index.md](docs/index.md) | [index.md](docs/en/index.md) |
| Memulai | [getting-started.md](docs/getting-started.md) | [getting-started.md](docs/en/getting-started.md) |
| Kantong dan saldo | [wallets.md](docs/wallets.md) | [wallets.md](docs/en/wallets.md) |
| Transaksi | [transactions.md](docs/transactions.md) | [transactions.md](docs/en/transactions.md) |
| Budget dan tagihan | [budget-and-bills.md](docs/budget-and-bills.md) | [budget-and-bills.md](docs/en/budget-and-bills.md) |
| Laporan dan grafik | [reports.md](docs/reports.md) | [reports.md](docs/en/reports.md) |
| Backup dan restore | [backup-and-restore.md](docs/backup-and-restore.md) | [backup-and-restore.md](docs/en/backup-and-restore.md) |
| Pengaturan | [settings.md](docs/settings.md) | [settings.md](docs/en/settings.md) |
| Pertanyaan umum | [faq.md](docs/faq.md) | [faq.md](docs/en/faq.md) |

## Unduh dan pasang

1. Buka [halaman rilis terbaru](https://github.com/s4ndrism/AturMyDuit-App/releases/latest).
2. Unduh `AturMyDuit-*.apk` dan `SHA256SUMS.txt`.
3. Izinkan pemasangan dari sumber tidak dikenal di pengaturan Android.
4. Buka APK dan selesaikan pemasangan.
5. Cocokkan checksum bila perlu:

   ```powershell
   Get-FileHash AturMyDuit-1.0.0.apk -Algorithm SHA256
   ```

   Bandingkan hasilnya dengan isi `SHA256SUMS.txt`.

APK hanya tersedia untuk **Android**. Data tersimpan lokal, jadi tidak ada akun
yang perlu dibuat.

## Privasi dan data

AturMyDuit tidak mengirim transaksi ke server mana pun. Semua data berada di
database lokal di perangkatmu. Backup lokal membuat salinan database di
penyimpanan yang kamu pilih, dan kamu bertanggung jawab menjaga file itu.

Satu-satunya akses jaringan adalah pemeriksaan versi terbaru: aplikasi membaca
metadata rilis publik di `api.github.com`. Tidak ada transaksi, identitas, atau
analytics yang dikirim.

## Bantuan dan laporan bug

- Ada pertanyaan atau menemukan bug? Buka [issue](https://github.com/s4ndrism/AturMyDuit-App/issues).
- Sertakan versi aplikasi dari Tentang Aplikasi, tipe HP, dan versi Android.
- Jangan lampirkan data transaksi pribadi atau file backup ke issue publik.

## Dukung pengembang

AturMyDuit gratis dan dikembangkan di waktu luang. Kalau aplikasi ini membantu,
kamu bisa traktir pengembang lewat
**[Trakteer](https://trakteer.id/s4ndrism)**. Donasi tidak wajib dan tidak
mengunci fitur apa pun.

## Lisensi

AturMyDuit adalah perangkat lunak **proprietary**.

- Gratis dipakai untuk keperluan **pribadi dan non-komersial**.
- Dilarang menjual, mengubah, atau mendistribusikan ulang aplikasi tanpa izin.
- Source code privat dan tidak dilisensikan untuk umum. Repositori ini hanya
  memuat rilis APK dan dokumentasi pengguna.
- Penggunaan komersial atau lisensi khusus: hubungi [@s4ndrism](https://github.com/s4ndrism).

Ketentuan lengkap ada di [`LICENSE`](LICENSE) (Indonesia) dan
[`LICENSE.en`](LICENSE.en) (English). Aplikasi menampilkan versi sesuai bahasa
yang dipilih.

## Kredit

Dikembangkan oleh [@s4ndrism](https://github.com/s4ndrism).

Dibangun dengan Flutter dan Dart, Drift + SQLite, Riverpod, go_router, fl_chart,
intl, flutter_local_notifications, timezone, uuid, clock, crypto, path_provider,
image_picker, file_picker, camera, sqlite3, flutter_markdown_plus, dan Montserrat
(SIL Open Font License). Terima kasih kepada komunitas di balik tools dan library
tersebut.

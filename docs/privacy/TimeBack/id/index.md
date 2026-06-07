---
title: Kebijakan Privasi | TimeBack
description: Kebijakan Privasi TimeBack
lang: id
last_updated: 2026-06-06
---

# Kebijakan Privasi (TimeBack)

- **Nama aplikasi:** TimeBack
- **Pengembang:** frog-im
- **Hubungi:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tanggal efektif:** 03-06-2026
- **Terakhir diperbarui:** 06-06-2026

Kebijakan Privasi ini didasarkan pada penerapan aplikasi TimeBack saat ini. TimeBack menyediakan ulasan waktu layar, sasaran harian, catatan waktu yang diperoleh kembali, refleksi, tantangan, pemberitahuan, berbagi, dan fitur iklan.

## 1. Fitur

TimeBack menyediakan fitur-fitur berikut:

- Tinjauan waktu penggunaan aplikasi melalui izin akses penggunaan Android
- Sasaran penggunaan harian, pengingat, dan pemberitahuan penggunaan bilah status
- Pemberitahuan peringatan batas keras dan tampilan overlay
- Pilihan aplikasi pengecualian overlay
- Catatan aktivitas waktu reklamasi
- Catatan refleksi harian
- Tantangan kemajuan dan manajemen daftar periksa
- Berbagi gambar status penggunaan
- Iklan Google AdMob dan opsi privasi berbasis UMP

## 2. Informasi yang Kami Proses

### 2-1. Informasi Baca Melalui Izin Akses Penggunaan

Jika pengguna memberikan izin Android `PACKAGE_USAGE_STATS`, aplikasi dapat membaca informasi berikut dari perangkat:

- Nama paket aplikasi
- Nama aplikasi
- Waktu penggunaan aplikasi
- Rentang tanggal dan waktu yang digunakan untuk agregasi penggunaan

Informasi ini digunakan untuk menyediakan statistik penggunaan dan membandingkan penggunaan dengan tujuan pengguna.

### 2-2. Informasi yang Dimasukkan atau Dikonfigurasi oleh Pengguna

- Sasaran penggunaan harian
- Pengingat penggunaan mengaktifkan status dan interval
- Pengaturan tampilan penggunaan bilah status
- Kategori aktivitas waktu reklamasi, judul, waktu mulai, dan durasi
- Teks refleksi harian
- Tantangan kemajuan dan entri daftar periksa
- Daftar aplikasi pengecualian overlay

### 2-3. Informasi yang Tersimpan di Perangkat

Aplikasi ini dapat menyimpan informasi berikut dalam database SQLite lokal atau SharedPreferences:

- Catatan waktu penggunaan aplikasi
- Sasaran dan pengaturan harian
- Catatan aktivitas waktu reklamasi
- Catatan refleksi harian
- Tantangan kemajuan dan status daftar periksa
- Status penyelesaian orientasi
- Pengaturan seperti pengingat penggunaan, peringatan batas keras, tampilan bilah status, dan aplikasi pengecualian overlay
- Izin iklan lokal dan status opsi privasi

Berdasarkan implementasi saat ini, catatan lokal ini tidak secara otomatis diunggah ke server frog-im.

### 2-4. Data Periklanan dan Persetujuan

Saat Iklan Seluler Google SDK (AdMob) dan UMP digunakan, Google atau afiliasinya dapat memproses informasi seperti:

- Pengidentifikasi iklan, seperti Android AD_ID
- IP alamat dan informasi jaringan
- Informasi perangkat, versi OS, dan informasi aplikasi
- Tayangan iklan, klik, data pengukuran, dan sinyal kesalahan
- Persetujuan iklan dan status opsi privasi
- Perkiraan lokasi

## 3. Tujuan Pengolahan

Aplikasi memproses informasi untuk tujuan berikut:

- Membaca waktu penggunaan, menampilkan statistik, dan membandingkan penggunaan dengan sasaran
- Menyimpan catatan waktu reklamasi dan refleksi yang dimasukkan oleh pengguna
- Mengelola kemajuan tantangan
- Memberikan pengingat dan pemberitahuan bilah status
- Memberikan pemberitahuan peringatan batas keras, tampilan overlay, dan penanganan pengecualian overlay
- Berbagi gambar status penggunaan saat diminta oleh pengguna
- Menayangkan iklan, mengukur kinerja iklan, dan menerapkan pilihan izin iklan
- Menjaga stabilitas aplikasi dan merespons kesalahan

## 4. Penyimpanan Lokal dan Pemrosesan Eksternal

### 4-1. Penyimpanan Lokal

TimeBack menyimpan data pengguna terutama di penyimpanan internal aplikasi di perangkat. Berdasarkan implementasi saat ini, catatan penggunaan, tujuan, refleksi, dan informasi tantangan tidak secara otomatis diunggah ke server frog-im.

Penyimpanan lokal mungkin mencakup yang berikut ini.

| Penyimpanan | Barang yang disimpan | Tujuan | Metode penghapusan |
|---|---|---|---|
| SQL pangkalan data | Catatan penggunaan aplikasi, nama paket, nama aplikasi, waktu penggunaan, agregat berdasarkan tanggal | Tampilkan statistik penggunaan dan bandingkan penggunaan dengan sasaran | Fitur penghapusan dalam aplikasi, menghapus data aplikasi, atau mencopot pemasangan aplikasi |
| SQL pangkalan data | Aktivitas waktu yang diperoleh kembali, refleksi, kemajuan tantangan, entri daftar periksa | Tampilkan catatan dan kelola kemajuan | Fitur penghapusan dalam aplikasi, menghapus data aplikasi, atau mencopot pemasangan aplikasi |
| Preferensi Bersama | Status penyelesaian orientasi, pengaturan pengingat, pengaturan peringatan batas keras, pengaturan tampilan bilah status, daftar aplikasi pengecualian overlay, status persetujuan iklan lokal | Simpan pengaturan aplikasi | Menghapus data aplikasi atau mencopot pemasangan aplikasi |
| File/cache sementara | Gambar status penggunaan bersama dan file sementara serupa | Lakukan berbagi yang diminta oleh pengguna | Dihapus setelah dibagikan jika memungkinkan, atau sesuai dengan OS/kebijakan pembersihan aplikasi |

Saat pengguna menghapus data aplikasi atau mencopot pemasangan aplikasi, data yang disimpan di penyimpanan internal aplikasi biasanya akan terhapus. Namun, cadangan Android, cadangan pabrikan, cadangan cloud, atau file yang dibagikan secara langsung oleh pengguna dapat disimpan secara terpisah sesuai dengan kebijakan layanan tersebut.

Catatan penggunaan dan teks refleksi dapat mengungkapkan rutinitas atau minat pribadi. Pada perangkat bersama, pengguna harus menggunakan perlindungan yang sesuai seperti kunci perangkat atau akun OS terpisah.

### 4-2. Unggahan Server

Berdasarkan proyek saat ini, TimeBack tidak secara otomatis mengunggah catatan penggunaan, refleksi, atau catatan tantangan ke server frog-im. Jika pengguna menggunakan fitur berbagi, gambar statistik yang dihasilkan dapat ditransfer ke aplikasi atau layanan eksternal yang dipilih oleh pengguna.

### 4-3. Pemrosesan Periklanan

Google AdMob dan UMP digunakan untuk periklanan dalam aplikasi dan pengelolaan izin. Informasi terkait periklanan dapat diproses di infrastruktur Google.

## 5. Layanan dan Prosesor Pihak Ketiga

### 5-1. Google AdMob / UMP

Tujuan:

- Pengiriman iklan spanduk
- Persetujuan iklan dan penanganan opsi privasi
- Pengukuran kinerja iklan dan pencegahan penipuan

Informasi yang dapat diproses:

- Pengidentifikasi iklan
- Informasi perangkat dan jaringan
- Informasi interaksi iklan
- Status persetujuan dan opsi privasi

### 5-2. Berbagi Aplikasi atau Layanan Target

Jika pengguna secara langsung menggunakan fitur berbagi gambar status penggunaan, aplikasi atau layanan eksternal yang dipilih dapat memproses gambar yang dibagikan. Pemrosesan tersebut diatur oleh kebijakan privasi layanan yang dipilih.

## 6. Pemberitahuan Transfer Lintas Batas

Informasi dapat diproses di luar negara pengguna dalam kasus berikut.

| Barang | Detail |
|---|---|
| Penerima | Google LLC dan afiliasinya |
| Tujuan | Amerika Serikat dan negara/wilayah lain tempat infrastruktur Google berada |
| Waktu | Saat aplikasi berjalan, meminta iklan, menampilkan atau mengukur iklan, memproses klik, atau menangani persetujuan |
| Metode | Komunikasi jaringan terenkripsi (HTTPS/TLS) |
| Tujuan | Pengiriman iklan, penanganan status personalisasi, pengukuran, analitik, peningkatan stabilitas layanan, kepatuhan hukum |
| Data | Pengidentifikasi iklan, informasi perangkat/aplikasi/jaringan, informasi interaksi iklan, status izin, perkiraan lokasi, dll. |
| Penyimpanan | Sesuai dengan kebijakan Google dan hukum yang berlaku |

Untuk detailnya, silakan lihat [Cross-Border Transfer Notice](./policy/).

## 7. Daftar Aplikasi Terpasang dan Pengecualian Hamparan

Di Android, jika pengguna mengonfigurasi aplikasi pengecualian overlay, aplikasi dapat membaca nama paket dan nama aplikasi dari aplikasi yang dapat diluncurkan di perangkat untuk menampilkan daftar pilihan. Nama paket yang dipilih oleh pengguna sebagai pengecualian disimpan di SharedPreferences pada perangkat dan hanya digunakan untuk menghindari tampilan peringatan batas keras di atas aplikasi tersebut.

## 8. Retensi

Aplikasi ini menyimpan informasi berdasarkan standar berikut:

- Informasi penggunaan lokal, sasaran, refleksi, dan tantangan: hingga pengguna menghapusnya, menghapus data aplikasi, atau mencopot pemasangan aplikasi
- Setelan SharedPreferences: hingga pengguna menghapus data aplikasi atau mencopot pemasangan aplikasi
- File sementara untuk gambar yang dibagikan: sesuai kebutuhan untuk berbagi atau sesuai dengan kebijakan pembersihan OS
- Data terkait periklanan dan izin: sesuai dengan kebijakan Google dan pihak ketiga terkait lainnya

## 9. Izin

Aplikasi ini mungkin menggunakan izin berikut:

- `PACKAGE_USAGE_STATS`: membaca waktu penggunaan aplikasi
- `POST_NOTIFICATIONS`: tampilkan pengingat penggunaan dan pemberitahuan bilah status
- `SYSTEM_ALERT_WINDOW`: tampilkan hamparan peringatan batas keras
- `INTERNET`: berkomunikasi dengan iklan SDKs dan menampilkan halaman pemberitahuan hukum
- `ACCESS_NETWORK_STATE`: periksa status jaringan
- `com.google.android.gms.permission.AD_ID`: gunakan pengidentifikasi iklan

Izin hanya digunakan jika diperlukan untuk fitur aplikasi. Pengguna dapat mencabut izin di pengaturan perangkat, namun fitur terkait mungkin dibatasi.

## 10. Hak dan Pilihan Pengguna

Pengguna dapat:

- Lihat, edit, atau hapus catatan di dalam aplikasi
- Hapus informasi lokal dengan menghapus data aplikasi atau mencopot pemasangan aplikasi
- Ubah pengaturan akses penggunaan, notifikasi, dan pengidentifikasi iklan di pengaturan perangkat
- Cabut izin overlay dan ubah pengaturan aplikasi pengecualian overlay
- Ubah opsi privasi iklan
- Hubungi kami jika ada pertanyaan privasi atau permintaan penghapusan

Email kontak: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Tindakan Keamanan

Aplikasi ini menerapkan atau mungkin menerapkan perlindungan berikut:

- Komunikasi eksternal berbasis HTTPS/TLS
- Pemrosesan data yang mengutamakan lokal
- Permintaan izin minimum diperlukan untuk fitur aplikasi
- Penerapan negara persetujuan periklanan

Kondisi keamanan perangkat seperti rooting, jailbreaking, malware, atau penggunaan perangkat bersama dapat menimbulkan risiko tambahan.

## 12. Privasi Anak

TimeBack tidak dirancang terutama untuk anak-anak. Setelan terkait usia atau kebijakan platform Iklan Seluler Google SDK dan UMP mungkin berlaku selama pemrosesan periklanan dan persetujuan.

## 13. Perubahan

Kebijakan ini dapat diperbarui karena perubahan undang-undang, konfigurasi layanan pihak ketiga, atau fitur aplikasi. Perubahan materi akan diberitahukan melalui pemberitahuan dalam aplikasi atau dengan memperbarui halaman ini.

## 14. Kontak

- Pengembang: frog-im
- Surel: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---
title: Kebijakan Privasi | Lucky Pick Box
description: Lucky Pick Box Kebijakan Privasi
lang: id
last_updated: 2026-06-15
---

# Kebijakan Privasi (Lucky Pick Box / 뽑기박스)

- **Nama Aplikasi:** Lucky Pick Box / 뽑기박스
- **Pengembang:** frog-im
- **Petugas Perlindungan Informasi Pribadi / Narahubung:** frog-im
- **Kontak:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tanggal Berlaku:** 2026-06-12
- **Terakhir Diperbarui:** 2026-06-15

> Kebijakan ini disusun berdasarkan informasi yang diproses oleh aplikasi dan fitur-fitur terkaitnya.  
> Jika terdapat hukum atau peraturan yang bersifat wajib di negara atau wilayah tertentu, maka hukum atau peraturan tersebut dapat berlaku lebih dahulu.

---

## 1. Tujuan dan Ruang Lingkup

Lucky Pick Box adalah alat santai untuk pilihan acak, undian, pemilihan urutan, pembagian tim, dadu, koin, tangga, roda, dan permainan keputusan harian atau kelompok sejenis. Aplikasi tidak menyediakan perjudian uang sungguhan, taruhan, transaksi keuangan, hadiah uang tunai, atau imbalan setara uang.

### A. Fitur utama

- Input cepat: teks yang diketik pengguna atau dibaca dari gambar yang dipilih.
- Permainan pilihan acak: tangga, roda, plinko, undian sederhana, dadu, koin, angka acak, pembagi tim, pemilih urutan, kartu, bom, dan ya/tidak.
- Riwayat hasil: jenis permainan, judul, peserta/item, ringkasan hasil, dan waktu pembuatan dapat disimpan.
- Slot pengaturan: beberapa permainan dapat menyimpan peserta, daftar item, rentang angka, jumlah, tim, bobot, dan pengaturan serupa sampai 3 slot lokal.

Aplikasi tidak meminta pendaftaran atau login. Kami tidak mengoperasikan server yang menerima nama, nomor telepon, alamat email, kontak, entri permainan, gambar yang dipilih, atau hasil permainan dari aplikasi.

Untuk menyediakan fitur, aplikasi dapat menyimpan entri permainan, label peserta, hasil terbaru, pengaturan permainan tersimpan, pengaturan animasi, pilihan privasi iklan, dan status terkait persetujuan di penyimpanan lokal perangkat Anda. Riwayat hasil terbaru dibatasi oleh aplikasi dan tidak dikirim ke server yang dioperasikan pengembang.

---

## 2. Kategori Informasi Pribadi yang Diproses

### 2-1) Informasi yang Dimasukkan Langsung oleh Pengguna

Aplikasi tidak meminta pendaftaran atau login. Kami tidak mengoperasikan server yang menerima nama, nomor telepon, alamat email, kontak, entri permainan, gambar yang dipilih, atau hasil permainan dari aplikasi.

### 2-2) File yang Dipilih di Perangkat

Jika Anda memilih membaca teks dari gambar, aplikasi meminta Anda memilih gambar dari pustaka foto. Gambar yang dipilih digunakan untuk pengenalan teks di perangkat melalui pemilih gambar platform dan komponen Google ML Kit. Pengembang tidak mengunggah gambar ke server yang dioperasikan pengembang dan tidak menyimpannya di akun jarak jauh.

### 2-3) Data yang Disimpan Secara Lokal di Dalam Aplikasi

Untuk menyediakan fitur, aplikasi dapat menyimpan entri permainan, label peserta, hasil terbaru, pengaturan permainan tersimpan, pengaturan animasi, pilihan privasi iklan, dan status terkait persetujuan di penyimpanan lokal perangkat Anda. Riwayat hasil terbaru dibatasi oleh aplikasi dan tidak dikirim ke server yang dioperasikan pengembang.

### B. Data lokal di perangkat

| Lokasi atau kunci | Data | Tujuan | Penghapusan |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, jenis permainan, judul, peserta/item, ringkasan, waktu; hingga 50 hasil terbaru. | Menampilkan hasil terbaru dan riwayat. | Hapus riwayat di aplikasi, hapus data aplikasi, atau copot aplikasi |
| `game_settings.<gameId>.slot_<n>` | Pengaturan permainan, waktu simpan, daftar, rentang, jumlah, tim, bobot; hingga 3 slot. | Memuat kembali pengaturan permainan. | Kosongkan slot, hapus data, atau copot aplikasi |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Pengaturan animasi dan layar penuh. | Menyimpan preferensi tampilan. | Ubah pengaturan, hapus data, atau copot aplikasi |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Pilihan privasi iklan dan hitungan frekuensi iklan. | Menerapkan pilihan regional dan mengatur frekuensi. | Ubah pengaturan, hapus data, atau copot aplikasi |
| Pemilih gambar dan OCR | Jalur gambar yang dipilih dan teks yang dikenali dapat diproses sementara. | Menambahkan teks gambar ke input cepat. | Cache aplikasi/OS atau penghapusan data |

Teks input cepat tidak dikirim ke server pengembang. Teks tersebut hanya dapat menjadi data lokal jika digunakan dalam hasil permainan atau pengaturan yang disimpan.

### 2-4) Informasi yang Dapat Diproses Secara Otomatis Selama Pengelolaan Iklan dan Persetujuan

Pada platform yang didukung, saat ini Android, aplikasi menggunakan Google AdMob dan Google User Messaging Platform (UMP). Google dan mitra iklan dapat memproses pengenal iklan, pengenal instans aplikasi, alamat IP, perkiraan lokasi, informasi perangkat dan jaringan, versi aplikasi, sistem operasi, bahasa, impresi, klik dan interaksi iklan, diagnostik, status persetujuan, serta pengaturan privasi iklan regional untuk penayangan iklan, pembatasan frekuensi, pencegahan penipuan, pengelolaan persetujuan, pengukuran, analitik, keamanan, dan kepatuhan hukum.

Praktik privasi Google dijelaskan di https://policies.google.com/privacy dan https://policies.google.com/technologies/ads.

---

## 3. Tujuan Pemrosesan Informasi Pribadi

Lucky Pick Box adalah alat santai untuk pilihan acak, undian, pemilihan urutan, pembagian tim, dadu, koin, tangga, roda, dan permainan keputusan harian atau kelompok sejenis. Aplikasi tidak menyediakan perjudian uang sungguhan, taruhan, transaksi keuangan, hadiah uang tunai, atau imbalan setara uang.

### A. Fitur utama

- Input cepat: teks yang diketik pengguna atau dibaca dari gambar yang dipilih.
- Permainan pilihan acak: tangga, roda, plinko, undian sederhana, dadu, koin, angka acak, pembagi tim, pemilih urutan, kartu, bom, dan ya/tidak.
- Riwayat hasil: jenis permainan, judul, peserta/item, ringkasan hasil, dan waktu pembuatan dapat disimpan.
- Slot pengaturan: beberapa permainan dapat menyimpan peserta, daftar item, rentang angka, jumlah, tim, bobot, dan pengaturan serupa sampai 3 slot lokal.

Pada platform yang didukung, saat ini Android, aplikasi menggunakan Google AdMob dan Google User Messaging Platform (UMP). Google dan mitra iklan dapat memproses pengenal iklan, pengenal instans aplikasi, alamat IP, perkiraan lokasi, informasi perangkat dan jaringan, versi aplikasi, sistem operasi, bahasa, impresi, klik dan interaksi iklan, diagnostik, status persetujuan, serta pengaturan privasi iklan regional untuk penayangan iklan, pembatasan frekuensi, pencegahan penipuan, pengelolaan persetujuan, pengukuran, analitik, keamanan, dan kepatuhan hukum.

Praktik privasi Google dijelaskan di https://policies.google.com/privacy dan https://policies.google.com/technologies/ads.

---

## 4. Jangka Waktu Penyimpanan dan Retensi Informasi Pribadi

Riwayat lokal dan pengaturan dapat tetap berada di perangkat hingga Anda menghapus riwayat, menghapus data aplikasi, atau mencopot aplikasi. Anda dapat mengubah pilihan privasi iklan yang tersedia di pengaturan aplikasi, membuka opsi privasi Google bila diperlukan, dan mengelola atau mereset pengenal iklan di pengaturan privasi perangkat. Penyimpanan informasi yang diproses Google diatur oleh kebijakan dan kewajiban hukum Google.

### B. Data lokal di perangkat

| Lokasi atau kunci | Data | Tujuan | Penghapusan |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, jenis permainan, judul, peserta/item, ringkasan, waktu; hingga 50 hasil terbaru. | Menampilkan hasil terbaru dan riwayat. | Hapus riwayat di aplikasi, hapus data aplikasi, atau copot aplikasi |
| `game_settings.<gameId>.slot_<n>` | Pengaturan permainan, waktu simpan, daftar, rentang, jumlah, tim, bobot; hingga 3 slot. | Memuat kembali pengaturan permainan. | Kosongkan slot, hapus data, atau copot aplikasi |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Pengaturan animasi dan layar penuh. | Menyimpan preferensi tampilan. | Ubah pengaturan, hapus data, atau copot aplikasi |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Pilihan privasi iklan dan hitungan frekuensi iklan. | Menerapkan pilihan regional dan mengatur frekuensi. | Ubah pengaturan, hapus data, atau copot aplikasi |
| Pemilih gambar dan OCR | Jalur gambar yang dipilih dan teks yang dikenali dapat diproses sementara. | Menambahkan teks gambar ke input cepat. | Cache aplikasi/OS atau penghapusan data |

Teks input cepat tidak dikirim ke server pengembang. Teks tersebut hanya dapat menjadi data lokal jika digunakan dalam hasil permainan atau pengaturan yang disimpan.

---

## 5. Prosedur dan Metode Penghapusan Informasi Pribadi

Riwayat lokal dan pengaturan dapat tetap berada di perangkat hingga Anda menghapus riwayat, menghapus data aplikasi, atau mencopot aplikasi. Anda dapat mengubah pilihan privasi iklan yang tersedia di pengaturan aplikasi, membuka opsi privasi Google bila diperlukan, dan mengelola atau mereset pengenal iklan di pengaturan privasi perangkat. Penyimpanan informasi yang diproses Google diatur oleh kebijakan dan kewajiban hukum Google.

### C. Izin, SDK, cadangan, dan keamanan

Aplikasi dapat menggunakan `INTERNET`, `ACCESS_NETWORK_STATE`, dan `com.google.android.gms.permission.AD_ID` untuk iklan dan pemberitahuan hukum. Akses foto atau pemilih gambar hanya digunakan saat pengguna memilih membaca teks dari gambar.

Google Mobile Ads SDK dapat memproses alamat IP, interaksi iklan, diagnostik, dan pengenal perangkat/akun untuk iklan, analitik, dan pencegahan penipuan. UMP dapat memproses status persetujuan dan pilihan privasi.

Data lokal dapat dihapus melalui fitur aplikasi, penghapusan data aplikasi di sistem operasi, atau pencopotan aplikasi. Cadangan sistem, tangkapan layar, atau file yang dibagikan pengguna dapat tetap ada sesuai kebijakan penyedia. Hindari memasukkan data sensitif di kolom teks bebas.

---

## 6. Penyediaan kepada Pihak Ketiga, Penugasan Pemrosesan, dan Transfer Lintas Batas

Kami tidak menjual entri permainan, label peserta, hasil permainan, atau gambar yang dipilih. Saat fitur iklan atau persetujuan diminta, Google LLC, afiliasi Google, dan penyedia layanannya dapat memproses informasi iklan dan persetujuan di negara di luar negara atau wilayah Anda. Lihat "Pemberitahuan Transfer Data Internasional" di aplikasi untuk detail.

| Item | Rincian |
|---|---|
| **Penerima / Pihak yang Ditunjuk** | Google LLC dan afiliasinya (operator AdMob / UMP) |
| **Negara Transfer** | Amerika Serikat dan wilayah tempat infrastruktur Google dioperasikan |
| **Waktu Transfer** | Secara berkelanjutan selama permintaan iklan, pemeriksaan status persetujuan, inisialisasi SDK, dan operasional |
| **Metode Transfer** | Pengiriman melalui komunikasi jaringan antara aplikasi dan server pihak ketiga |
| **Dasar Hukum untuk Transfer Lintas Batas** | Diproses dalam lingkup yang diperlukan untuk menyediakan layanan berdasarkan dasar hukum yang berlaku, atau jika diperlukan, berdasarkan persetujuan subjek data |
| **Tujuan** | Penayangan iklan, pengukuran iklan, pengelolaan persetujuan, pencegahan penipuan, dan kepatuhan terhadap kebijakan / hukum |
| **Kategori Data (Contoh)** | Pengenal iklan (AAID / IDFA), informasi IP / jaringan, informasi perangkat / aplikasi, informasi interaksi iklan, status persetujuan |
| **Masa Penyimpanan** | Tunduk pada kebijakan Google dan hukum yang berlaku |
| **Dampak Penolakan** | Iklan yang dipersonalisasi dapat dibatasi, iklan non-personalisasi dapat ditampilkan, atau beberapa fitur terkait iklan dapat dibatasi |

---

## 7. Informasi tentang Izin yang Digunakan

### C. Izin, SDK, cadangan, dan keamanan

Aplikasi dapat menggunakan `INTERNET`, `ACCESS_NETWORK_STATE`, dan `com.google.android.gms.permission.AD_ID` untuk iklan dan pemberitahuan hukum. Akses foto atau pemilih gambar hanya digunakan saat pengguna memilih membaca teks dari gambar.

Google Mobile Ads SDK dapat memproses alamat IP, interaksi iklan, diagnostik, dan pengenal perangkat/akun untuk iklan, analitik, dan pencegahan penipuan. UMP dapat memproses status persetujuan dan pilihan privasi.

Data lokal dapat dihapus melalui fitur aplikasi, penghapusan data aplikasi di sistem operasi, atau pencopotan aplikasi. Cadangan sistem, tangkapan layar, atau file yang dibagikan pengguna dapat tetap ada sesuai kebijakan penyedia. Hindari memasukkan data sensitif di kolom teks bebas.

---

## 8. Pemasangan, Pengoperasian, dan Penolakan terhadap Mekanisme Pengumpulan Otomatis

Pada platform yang didukung, saat ini Android, aplikasi menggunakan Google AdMob dan Google User Messaging Platform (UMP). Google dan mitra iklan dapat memproses pengenal iklan, pengenal instans aplikasi, alamat IP, perkiraan lokasi, informasi perangkat dan jaringan, versi aplikasi, sistem operasi, bahasa, impresi, klik dan interaksi iklan, diagnostik, status persetujuan, serta pengaturan privasi iklan regional untuk penayangan iklan, pembatasan frekuensi, pencegahan penipuan, pengelolaan persetujuan, pengukuran, analitik, keamanan, dan kepatuhan hukum.

Praktik privasi Google dijelaskan di https://policies.google.com/privacy dan https://policies.google.com/technologies/ads.

Riwayat lokal dan pengaturan dapat tetap berada di perangkat hingga Anda menghapus riwayat, menghapus data aplikasi, atau mencopot aplikasi. Anda dapat mengubah pilihan privasi iklan yang tersedia di pengaturan aplikasi, membuka opsi privasi Google bila diperlukan, dan mengelola atau mereset pengenal iklan di pengaturan privasi perangkat. Penyimpanan informasi yang diproses Google diatur oleh kebijakan dan kewajiban hukum Google.

---

## 9. Hak Pengguna dan Cara Menggunakannya

Riwayat lokal dan pengaturan dapat tetap berada di perangkat hingga Anda menghapus riwayat, menghapus data aplikasi, atau mencopot aplikasi. Anda dapat mengubah pilihan privasi iklan yang tersedia di pengaturan aplikasi, membuka opsi privasi Google bila diperlukan, dan mengelola atau mereset pengenal iklan di pengaturan privasi perangkat. Penyimpanan informasi yang diproses Google diatur oleh kebijakan dan kewajiban hukum Google.

---

## 10. Langkah-Langkah Keamanan

### C. Izin, SDK, cadangan, dan keamanan

Aplikasi dapat menggunakan `INTERNET`, `ACCESS_NETWORK_STATE`, dan `com.google.android.gms.permission.AD_ID` untuk iklan dan pemberitahuan hukum. Akses foto atau pemilih gambar hanya digunakan saat pengguna memilih membaca teks dari gambar.

Google Mobile Ads SDK dapat memproses alamat IP, interaksi iklan, diagnostik, dan pengenal perangkat/akun untuk iklan, analitik, dan pencegahan penipuan. UMP dapat memproses status persetujuan dan pilihan privasi.

Data lokal dapat dihapus melalui fitur aplikasi, penghapusan data aplikasi di sistem operasi, atau pencopotan aplikasi. Cadangan sistem, tangkapan layar, atau file yang dibagikan pengguna dapat tetap ada sesuai kebijakan penyedia. Hindari memasukkan data sensitif di kolom teks bebas.

### C. Izin, SDK, cadangan, dan keamanan

Aplikasi dapat menggunakan `INTERNET`, `ACCESS_NETWORK_STATE`, dan `com.google.android.gms.permission.AD_ID` untuk iklan dan pemberitahuan hukum. Akses foto atau pemilih gambar hanya digunakan saat pengguna memilih membaca teks dari gambar.

Google Mobile Ads SDK dapat memproses alamat IP, interaksi iklan, diagnostik, dan pengenal perangkat/akun untuk iklan, analitik, dan pencegahan penipuan. UMP dapat memproses status persetujuan dan pilihan privasi.

Data lokal dapat dihapus melalui fitur aplikasi, penghapusan data aplikasi di sistem operasi, atau pencopotan aplikasi. Cadangan sistem, tangkapan layar, atau file yang dibagikan pengguna dapat tetap ada sesuai kebijakan penyedia. Hindari memasukkan data sensitif di kolom teks bebas.

---

## 11. Informasi Mengenai Informasi Sensitif

Aplikasi ini tidak mengharuskan pengguna memasukkan informasi sensitif.  
Pengguna disarankan untuk tidak memasukkan konten sensitif seperti informasi kesehatan, pandangan politik, agama, informasi biometrik, atau informasi terkait kehidupan seksual ke dalam catatan atau kolom input bebas.

Jika pengguna secara sukarela memasukkan konten sensitif, informasi tersebut dapat disimpan sebagai data lokal pada perangkat yang dikelola langsung oleh pengguna.

---


## 12. Perlindungan Informasi Pribadi Anak

Aplikasi ini tidak dirancang terutama untuk anak-anak.  
Wali dapat mengelola penggunaan melalui fitur kontrol orang tua yang disediakan oleh perangkat atau toko aplikasi.

---


## 13. Pengambilan Keputusan Otomatis

Aplikasi ini tidak melakukan pengambilan keputusan otomatis berdasarkan informasi pribadi yang menimbulkan akibat hukum atau dampak signifikan serupa.

---


## 14. Pemberitahuan Keamanan Data (Google Play, dll.)

Pengembang berupaya untuk menjaga dan memperbarui item pengungkapan keamanan data di pasar aplikasi (seperti Google Play) sesuai dengan praktik pemrosesan aktual aplikasi dan praktik pemrosesan aktual dari SDK pihak ketiga.

Namun, informasi yang ditampilkan di toko aplikasi dapat berbeda tergantung pada versi aplikasi, negara distribusi, konfigurasi SDK pihak ketiga, dan perubahan kebijakan.

---


## 15. Pemberitahuan Open Source

Aplikasi ini menggunakan beberapa pustaka open-source.  
Informasi mengenai lisensi terkait dapat ditemukan di layar terkait dalam aplikasi atau dalam pemberitahuan yang disediakan melalui saluran distribusi.

---


## 16. Kontak

Untuk pertanyaan terkait Kebijakan Privasi ini:

- **Petugas Perlindungan Informasi Pribadi / Narahubung:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---


## 17. Perubahan terhadap Kebijakan Privasi ini

Kebijakan ini dapat direvisi karena perubahan hukum / kebijakan, fitur aplikasi, atau SDK pihak ketiga.  
Jika terdapat perubahan material, pemberitahuan dapat diberikan melalui pemberitahuan dalam aplikasi, halaman distribusi, atau pembaruan pada halaman kebijakan.

Terakhir Diperbarui: **2026-06-15**

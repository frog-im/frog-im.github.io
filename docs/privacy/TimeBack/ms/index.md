---
title: Dasar Privasi | TimeBack
description: Dasar Privasi TimeBack
lang: ms
last_updated: 2026-06-06
---

# Dasar Privasi (TimeBack)

- **Nama apl:** TimeBack
- **Pembangun:** frog-im
- **Hubungi:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tarikh berkuatkuasa:** 2026-06-03
- **Terakhir dikemas kini:** 2026-06-06

Dasar Privasi ini adalah berdasarkan pelaksanaan semasa apl TimeBack. TimeBack menyediakan semakan masa skrin, matlamat harian, rekod masa yang dituntut semula, refleksi, cabaran, pemberitahuan, perkongsian dan ciri pengiklanan.

## 1. Ciri-ciri

TimeBack menyediakan ciri berikut:

- Semakan masa penggunaan apl melalui kebenaran akses penggunaan Android
- Matlamat penggunaan harian, peringatan dan pemberitahuan penggunaan bar status
- Pemberitahuan amaran had keras dan paparan tindanan
- Pilihan apl pengecualian tindanan
- Rekod aktiviti masa tebus guna
- Rekod refleksi harian
- Mencabar kemajuan dan pengurusan senarai semak
- Perkongsian imej statistik penggunaan
- Iklan Google AdMob dan pilihan privasi berasaskan UMP

## 2. Maklumat yang Kami Proses

### 2-1. Maklumat Baca Melalui Kebenaran Akses Penggunaan

Jika pengguna memberikan Android `PACKAGE_USAGE_STATS` kebenaran, apl boleh membaca maklumat berikut daripada peranti:

- Nama pakej apl
- Nama apl
- Masa penggunaan apl
- Julat tarikh dan masa digunakan untuk pengagregatan penggunaan

Maklumat ini digunakan untuk menyediakan statistik penggunaan dan membandingkan penggunaan dengan matlamat pengguna.

### 2-2. Maklumat yang Dimasukkan atau Dikonfigurasikan oleh Pengguna

- Matlamat penggunaan harian
- Keadaan dan selang masa didayakan peringatan penggunaan
- Tetapan paparan penggunaan bar status
- Kategori aktiviti masa tebus guna, tajuk, masa mula dan tempoh
- Teks refleksi harian
- Cabaran kemajuan dan penyertaan senarai semak
- Senarai apl pengecualian tindanan

### 2-3. Maklumat Disimpan pada Peranti

Apl mungkin menyimpan maklumat berikut dalam pangkalan data SQLite tempatan atau SharedPreferences:

- Rekod masa penggunaan apl
- Matlamat dan tetapan harian
- Rekod aktiviti masa tebus guna
- Rekod refleksi harian
- Cabaran kemajuan dan keadaan senarai semak
- Keadaan siap sedia
- Tetapan seperti peringatan penggunaan, amaran had keras, paparan bar status dan apl pengecualian tindanan
- Persetujuan iklan tempatan dan keadaan pilihan privasi

Berdasarkan pelaksanaan semasa, rekod tempatan ini tidak dimuat naik secara automatik ke pelayan frog-im.

### 2-4. Data Pengiklanan dan Persetujuan

Apabila Iklan Mudah Alih Google SDK (AdMob) dan UMP digunakan, Google atau ahli gabungannya boleh memproses maklumat seperti:

- Pengecam pengiklanan, seperti Android AD_ID
- IP alamat dan maklumat rangkaian
- Maklumat peranti, versi OS dan maklumat apl
- Tera iklan, klik, data ukuran dan isyarat ralat
- Persetujuan iklan dan keadaan pilihan privasi
- Anggaran lokasi

## 3. Tujuan Pemprosesan

Apl memproses maklumat untuk tujuan berikut:

- Masa penggunaan membaca, menunjukkan statistik dan membandingkan penggunaan dengan matlamat
- Menyimpan rekod masa tebus dan pantulan yang dimasukkan oleh pengguna
- Menguruskan kemajuan cabaran
- Menyediakan peringatan dan pemberitahuan bar status
- Menyediakan pemberitahuan amaran had keras, paparan tindanan dan pengendalian pengecualian tindanan
- Berkongsi imej statistik penggunaan apabila diminta oleh pengguna
- Menyiarkan iklan, mengukur prestasi iklan dan menggunakan pilihan persetujuan iklan
- Mengekalkan kestabilan apl dan bertindak balas terhadap ralat

## 4. Storan Tempatan dan Pemprosesan Luaran

### 4-1. Storan Tempatan

TimeBack menyimpan data pengguna terutamanya dalam storan dalaman apl pada peranti. Berdasarkan pelaksanaan semasa, rekod penggunaan, matlamat, refleksi dan maklumat cabaran tidak dimuat naik secara automatik ke pelayan frog-im.

Storan tempatan mungkin termasuk yang berikut.

| Penyimpanan | Barang yang disimpan | Tujuan | Kaedah pemadaman |
|---|---|---|---|
| pangkalan data SQLite | Rekod penggunaan apl, nama pakej, nama apl, masa penggunaan, agregat berasaskan tarikh | Tunjukkan statistik penggunaan dan bandingkan penggunaan dengan matlamat | Ciri pemadaman dalam apl, mengosongkan data apl atau menyahpasang apl |
| pangkalan data SQLite | Aktiviti masa tebus guna, refleksi, kemajuan cabaran, penyertaan senarai semak | Tunjukkan rekod dan urus kemajuan | Ciri pemadaman dalam apl, mengosongkan data apl atau menyahpasang apl |
| SharedPreferences | Keadaan siap sedia, tetapan peringatan, tetapan amaran had keras, tetapan paparan bar status, senarai apl pengecualian tindanan, keadaan persetujuan iklan setempat | Simpan tetapan apl | Membersihkan data apl atau menyahpasang apl |
| Fail/cache sementara | Imej statistik penggunaan dikongsi dan fail sementara yang serupa | Lakukan perkongsian yang diminta oleh pengguna | Dipadamkan selepas berkongsi jika boleh, atau mengikut dasar pembersihan OS/apl |

Apabila pengguna mengosongkan data apl atau menyahpasang apl, data yang disimpan dalam storan dalaman apl biasanya dipadamkan. Walau bagaimanapun, sandaran Android, sandaran pengilang, sandaran awan atau fail yang dikongsi secara langsung oleh pengguna boleh disimpan secara berasingan mengikut dasar perkhidmatan tersebut.

Rekod penggunaan dan teks refleksi mungkin mendedahkan rutin atau minat peribadi. Pada peranti kongsi, pengguna harus menggunakan perlindungan yang sesuai seperti kunci peranti atau akaun OS yang berasingan.

### 4-2. Muat Naik Pelayan

Berdasarkan projek semasa, TimeBack tidak memuat naik rekod penggunaan, refleksi atau cabaran secara automatik ke pelayan frog-im. Jika pengguna menggunakan ciri perkongsian, imej statistik yang dijana mungkin dipindahkan ke apl atau perkhidmatan luaran yang dipilih oleh pengguna.

### 4-3. Pemprosesan Pengiklanan

Google AdMob dan UMP digunakan untuk pengiklanan dalam apl dan pengurusan persetujuan. Maklumat berkaitan pengiklanan mungkin diproses pada infrastruktur Google.

## 5. Perkhidmatan dan Pemproses Pihak Ketiga

### 5-1. Google AdMob / UMP

Tujuan:

- Penghantaran iklan sepanduk
- Persetujuan iklan dan pengendalian pilihan privasi
- Pengukuran prestasi iklan dan pencegahan penipuan

Maklumat yang mungkin diproses:

- Pengecam pengiklanan
- Maklumat peranti dan rangkaian
- Maklumat interaksi iklan
- Keadaan persetujuan dan privasi-pilihan

### 5-2. Berkongsi Apl atau Perkhidmatan Sasaran

Jika pengguna secara langsung menggunakan ciri perkongsian imej statistik penggunaan, apl atau perkhidmatan luaran yang dipilih mungkin memproses imej yang dikongsi. Pemprosesan itu dikawal oleh dasar privasi perkhidmatan yang dipilih.

## 6. Notis Pemindahan Rentas Sempadan

Maklumat boleh diproses di luar negara pengguna dalam kes berikut.

| item | Butiran |
|---|---|
| Penerima | Google LLC dan ahli gabungannya |
| Destinasi | Amerika Syarikat dan negara/rantau lain yang menempatkan infrastruktur Google |
| Masa | Apabila apl dijalankan, meminta iklan, memaparkan atau mengukur iklan, memproses klik atau mengendalikan persetujuan |
| Kaedah | Komunikasi rangkaian yang disulitkan (HTTPS/TLS) |
| Tujuan | Penyampaian iklan, pengendalian keadaan pemperibadian, pengukuran, analitik, peningkatan kestabilan perkhidmatan, pematuhan undang-undang |
| Data | Pengecam pengiklanan, maklumat peranti/apl/rangkaian, maklumat interaksi iklan, keadaan persetujuan, anggaran lokasi, dsb. |
| Pengekalan | Selaras dengan dasar Google dan undang-undang yang terpakai |

Untuk butiran, sila lihat [Cross-Border Transfer Notice](./policy/).

## 7. Senarai Apl yang Dipasang dan Pengecualian Tindanan

Pada Android, jika pengguna mengkonfigurasi apl pengecualian tindanan, apl itu boleh membaca nama pakej dan nama apl apl boleh dilancarkan pada peranti untuk memaparkan senarai pilihan. Nama pakej yang dipilih oleh pengguna sebagai pengecualian disimpan dalam SharedPreferences pada peranti dan digunakan hanya untuk mengelak daripada menunjukkan tindanan amaran had keras di atas apl tersebut.

## 8. Pengekalan

Aplikasi ini mengekalkan maklumat di bawah piawaian berikut:

- Maklumat penggunaan, matlamat, refleksi dan cabaran setempat: sehingga pengguna memadamkannya, mengosongkan data apl atau menyahpasang apl
- Tetapan SharedPreferences: sehingga pengguna mengosongkan data apl atau menyahpasang apl
- Fail sementara untuk imej kongsi: seperti yang diperlukan untuk perkongsian atau mengikut dasar pembersihan OS
- Pengiklanan dan data berkaitan persetujuan: mengikut dasar Google dan pihak ketiga lain yang berkaitan

## 9. Kebenaran

Apl mungkin menggunakan kebenaran berikut:

- `PACKAGE_USAGE_STATS`: baca masa penggunaan apl
- `POST_NOTIFICATIONS`: tunjukkan peringatan penggunaan dan pemberitahuan bar status
- `SYSTEM_ALERT_WINDOW`: tunjukkan tindanan amaran had keras
- `INTERNET`: berkomunikasi dengan SDKs iklan dan tunjukkan halaman notis undang-undang
- `ACCESS_NETWORK_STATE`: semak keadaan rangkaian
- `com.google.android.gms.permission.AD_ID`: gunakan pengecam pengiklanan

Kebenaran digunakan hanya seperti yang diperlukan untuk ciri apl. Pengguna boleh membatalkan kebenaran dalam tetapan peranti, tetapi ciri yang berkaitan mungkin terhad.

## 10. Hak dan Pilihan Pengguna

Pengguna boleh:

- Lihat, edit atau padamkan rekod dalam apl
- Padamkan maklumat setempat dengan mengosongkan data apl atau menyahpasang apl
- Tukar tetapan akses penggunaan, pemberitahuan dan pengecam pengiklanan dalam tetapan peranti
- Batalkan kebenaran tindanan dan tukar tetapan aplikasi pengecualian tindanan
- Tukar pilihan privasi iklan
- Hubungi kami dengan soalan privasi atau permintaan pemadaman

E-mel hubungan: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Langkah Keselamatan

Aplikasi ini terpakai atau mungkin menggunakan perlindungan berikut:

- Komunikasi luaran berasaskan HTTPS/TLS
- Pemprosesan data tempatan pertama
- Permintaan kebenaran minimum diperlukan untuk ciri apl
- Permohonan keadaan persetujuan pengiklanan

Keadaan keselamatan peranti seperti pengakaran, pemecahan jail, perisian hasad atau penggunaan peranti kongsi boleh menimbulkan risiko tambahan.

## 12. Privasi Kanak-kanak

TimeBack tidak direka bentuk terutamanya untuk kanak-kanak. Tetapan berkaitan umur atau dasar platform Iklan Mudah Alih Google SDK dan UMP mungkin dikenakan semasa pemprosesan pengiklanan dan persetujuan.

## 13. Perubahan

Dasar ini mungkin dikemas kini disebabkan oleh perubahan dalam undang-undang, konfigurasi perkhidmatan pihak ketiga atau ciri apl. Perubahan material akan dimaklumkan melalui notis dalam apl atau dengan mengemas kini halaman ini.

## 14. Hubungi

- Pemaju: frog-im
- E-mel: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

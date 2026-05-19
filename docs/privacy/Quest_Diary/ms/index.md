---
title: Dasar Privasi | QDiary
description: Dasar Privasi QDiary
---

# Dasar Privasi (QDiary)

- Nama Aplikasi: QDiary
- Pembangun: frog-im
- Hubungi: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Tarikh Berkuat Kuasa: 2026-04-19
- Kemas Kini Terakhir: 2026-04-19

Dasar Privasi ini disediakan berdasarkan pelaksanaan semasa aplikasi QDiary. QDiary menyediakan ciri penulisan diari, penjanaan dan refleksi quest, log masuk, simpanan awan secara manual, pengiklanan, dan pemberitahuan, dan dalam proses tersebut mungkin memproses data peribadi atau maklumat yang boleh dianggap sebagai data peribadi setakat yang diperlukan.

## 1. Ciri yang Disediakan

QDiary menyediakan ciri berikut:

- Menulis, mengedit, dan melihat diari
- Pengelasan kategori dan paparan kalendar
- Penjanaan quest, refleksi quest, dan pengendalian penyelesaian quest
- Kunci aplikasi diari tempatan dan penyulitan tempatan
- Log masuk e-mel, pengesahan e-mel, log masuk tanpa nama (tetamu), dan tetapan semula kata laluan
- Simpanan dan muatan awan yang dimulakan oleh pengguna
- Paparan iklan dan pengendalian pilihan privasi iklan
- Pemberitahuan peringatan quest

## 2. Kategori Maklumat yang Diproses

### 2-1. Maklumat yang Dimasukkan Secara Terus oleh Pengguna

- Alamat e-mel
- Kata laluan
- Tajuk diari, kandungan, tarikh, kategori, dan tahap kesukaran
- Respons quest, kandungan refleksi, dan maklumat quest yang dipilih
- Pilihan berkaitan profil quest dan teks ringkasan
- Frasa laluan untuk kunci aplikasi diari

### 2-2. Maklumat yang Disimpan oleh Aplikasi pada Peranti

- Pangkalan data diari tempatan (SQLite)
- Maklumat status quest untuk diari tempatan
- Nilai status berkaitan kehadiran, tetapan, bahasa, pemberitahuan, dan iklan
- Nilai pengesahan kunci aplikasi, salt, dan metadata penyulitan
- Maklumat penjadualan pemberitahuan quest

### 2-3. Maklumat Akaun dan Pengenalpastian

Maklumat berikut mungkin diproses melalui Firebase Authentication:

- Firebase UID
- Alamat e-mel
- Sama ada pengesahan e-mel telah diselesaikan
- Sama ada log masuk tanpa nama sedang digunakan

### 2-4. Maklumat Pengiklanan dan Persetujuan

Apabila menggunakan Google AdMob dan UMP SDK, maklumat berikut mungkin diproses:

- Pengenal iklan (seperti Android AD_ID)
- Alamat IP dan maklumat rangkaian
- Maklumat peranti, versi OS, dan maklumat aplikasi
- Maklumat tera iklan, klik, dan pemprosesan ganjaran
- Status persetujuan iklan dan status pilihan privasi

### 2-5. Maklumat Berkaitan Pemberitahuan

- Sama ada kebenaran pemberitahuan telah diberikan
- Nilai pengecam bagi diari yang mengandungi quest yang sedang berjalan
- Teks pemberitahuan quest
- Masa pemberitahuan yang dijadualkan

## 3. Tujuan Pemprosesan

Aplikasi memproses maklumat bagi tujuan berikut:

- Pendaftaran, log masuk, pengesahan e-mel, dan tetapan semula kata laluan
- Menulis, menyimpan, dan melihat diari
- Penjanaan quest, refleksi, dan penentuan penyelesaian
- Penyulitan dan penyahsulitan tempatan yang berkaitan dengan kunci aplikasi
- Simpanan dan muatan awan yang diminta oleh pengguna
- Menyediakan pemberitahuan quest
- Menyediakan iklan, memproses ganjaran iklan, dan mencerminkan status persetujuan iklan
- Keselamatan, pengendalian ralat, dan operasi perkhidmatan

## 4. Storan Tempatan, Storan Awan, dan Pemprosesan Luaran

### 4-1. Storan Tempatan

Maklumat diari dan quest terutamanya disimpan dalam pangkalan data tempatan peranti.

- Jika kunci aplikasi tidak diaktifkan: disimpan secara tempatan dalam bentuk umum
- Jika kunci aplikasi diaktifkan: sesetengah maklumat, seperti tajuk diari, kandungan, dan status quest, mungkin disulitkan dan disimpan secara tempatan

### 4-2. Storan Awan

Aplikasi menyimpan data dalam Firebase Firestore hanya apabila pengguna secara langsung melaksanakan ciri `Save`.

Di bawah konfigurasi projek semasa:

- Penyegerakan penuh automatik tidak digunakan
- Data disimpan dalam Firestore `savedDiaries` hanya apabila pengguna menyimpannya secara manual
- Apabila disimpan, tajuk diari, kandungan, dan status quest mungkin disimpan dalam bentuk disulitkan bergantung pada status semasa kunci aplikasi
- Data dimuat semula ke storan tempatan hanya apabila pengguna melaksanakan `Load`

### 4-3. Pemprosesan Luaran untuk Penjanaan dan Refleksi Quest

Apabila pengguna meminta penjanaan quest atau refleksi, maklumat berikut mungkin digunakan untuk pemprosesan luaran melalui Firebase Functions:

- Tajuk diari
- Kandungan diari atau kandungan refleksi
- Kategori
- Tahap kesukaran
- Quest yang dipilih
- Maklumat ringkasan profil quest

Maklumat ini digunakan untuk penjanaan dan penilaian quest melalui OpenAI API.

Penting:

- Kandungan diari yang berkaitan hanya digunakan untuk pemprosesan luaran apabila ciri quest digunakan.
- Di bawah konfigurasi projek semasa, kod yang menyimpan log quest dalam koleksi berasingan `questLogs` tidak digunakan.

## 5. Perkhidmatan Pihak Ketiga dan Pemprosesan Luar

### 5-1. Google Firebase

Tujuan:

- Pengesahan (Firebase Authentication)
- Storan Firestore
- Pelaksanaan Cloud Functions

Maklumat yang mungkin diproses:

- UID, alamat e-mel, dan status pengesahan
- Data diari yang disimpan secara manual oleh pengguna
- Data permintaan quest

### 5-2. OpenAI

Tujuan:

- Penjanaan quest
- Refleksi quest dan penilaian penyelesaian

Maklumat yang mungkin diproses:

- Tajuk/kandungan diari
- Teks quest
- Tahap kesukaran dan kategori
- Kandungan refleksi yang dimasukkan oleh pengguna
- Maklumat ringkasan profil quest

### 5-3. Google AdMob / UMP

Tujuan:

- Menyediakan iklan sepanduk, antara halaman, dan berasaskan ganjaran
- Mengendalikan persetujuan iklan dan pilihan privasi

Maklumat yang mungkin diproses:

- Pengenal iklan
- Maklumat peranti dan rangkaian
- Maklumat interaksi iklan
- Status persetujuan

## 6. Notis Pemindahan Antarabangsa

Aplikasi mungkin memproses data peribadi atau maklumat berkaitan di luar negara pengguna dalam keadaan berikut:

| Item | Butiran |
|---|---|
| Penerima | Google LLC, OpenAI, dan pengendali infrastruktur berkaitan |
| Negara Destinasi | Amerika Syarikat, dan lain-lain |
| Masa Pemindahan | Semasa log masuk, penjanaan/refleksi quest, permintaan iklan, dan pemprosesan persetujuan |
| Kaedah Pemindahan | Komunikasi rangkaian yang disulitkan |
| Tujuan Pemindahan | Pengesahan, storan data, pemprosesan tanpa pelayan, penjanaan/penilaian quest berasaskan AI, dan pengiklanan |

## 7. Tempoh Penyimpanan dan Penggunaan

Aplikasi menyimpan maklumat mengikut piawaian berikut:

- Maklumat diari/tetapan tempatan: sehingga pengguna memadamkannya atau menyahpasang aplikasi
- Maklumat akaun Firebase: selagi pengguna mengekalkan akaun
- Data yang disimpan dalam Firestore: selagi pengguna mengekalkan item yang disimpan
- Data pemprosesan permintaan quest: setakat yang diperlukan untuk pemprosesan tanpa pelayan
- Data berkaitan iklan/persetujuan: mengikut dasar setiap penyedia luar

Selain itu, projek semasa merangkumi logik pembersihan automatik berikut:

- Pembersihan akaun pengguna tanpa nama dan data Firestore subkoleksi pengguna selepas tempoh tertentu
- Pembersihan akaun pengguna biasa yang tidak aktif untuk tempoh lama dan data Firestore subkoleksi pengguna

Walau bagaimanapun, sama ada perkara ini benar-benar diterapkan dalam persekitaran pengeluaran mungkin berbeza bergantung pada status penggunaan dan tetapan pelayan.

## 8. Notis Kunci Aplikasi dan Penyulitan Tempatan

Aplikasi menyediakan ciri berasingan `Diary App Lock`.

- Frasa laluan kunci aplikasi adalah berasingan daripada kata laluan akaun.
- Frasa laluan kunci aplikasi digunakan untuk penyulitan dan penyahsulitan diari tempatan.
- Walaupun frasa laluan yang salah dimasukkan, aplikasi itu sendiri mungkin tidak sentiasa disekat sepenuhnya; sebaliknya, sesetengah kandungan diari mungkin kekal tidak boleh dibaca.
- Sesetengah diari mungkin disulitkan secara berasingan berdasarkan frasa laluan yang digunakan semasa penulisan atau buka kunci sementara.

Pengguna hendaklah menjaga keselamatan frasa laluan mereka, dan jika ia hilang, pemulihan sebahagian data tempatan mungkin sukar.

## 9. Notis Pemberitahuan Quest

Jika pengguna mengaktifkan pemberitahuan quest, pemberitahuan tempatan mungkin dijadualkan bagi setiap diari dengan quest yang sedang berjalan.

- Penjadualan terutamanya dikendalikan melalui sistem penjadualan dalaman peranti.
- Di bawah konfigurasi projek semasa, tiada struktur yang disahkan di mana teks sumber diari dihantar secara berkala ke pelayan pusat semata-mata untuk tujuan pemberitahuan.

## 10. Notis Penggunaan Kebenaran

Aplikasi mungkin menggunakan kebenaran berikut untuk menyediakan cirinya:

- `INTERNET`: komunikasi dengan Firebase, OpenAI, dan SDK iklan
- `com.google.android.gms.permission.AD_ID`: penggunaan pengenal iklan
- `POST_NOTIFICATIONS`: memaparkan pemberitahuan quest
- `RECEIVE_BOOT_COMPLETED`: memulihkan pemberitahuan berjadual selepas peranti dimulakan semula

Kebenaran hanya digunakan setakat yang perlu untuk melaksanakan fungsi yang berkaitan.

## 11. Hak Subjek Data dan Cara Menggunakannya

Pengguna boleh menggunakan hak berikut:

- Mengakses, mengubah suai, dan memadam data dalam aplikasi
- Memadam atau menulis ganti data yang disimpan di awan
- Meminta log keluar dan pemadaman akaun
- Menukar pilihan privasi iklan
- Melumpuhkan kebenaran pemberitahuan

Cara menggunakan hak-hak ini:

- Memadam atau mengedit diari secara terus dalam aplikasi
- Memadam aplikasi atau menetapkan semula data tempatan
- Log keluar daripada akaun dan meminta pemadaman secara berasingan
- Menukar pemberitahuan, pengenal iklan, dan kebenaran dalam tetapan peranti
- E-mel hubungan: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Langkah Keselamatan

Aplikasi melaksanakan atau mungkin melaksanakan langkah perlindungan berikut:

- Komunikasi berasaskan HTTPS
- Kunci aplikasi diari tempatan dan penyulitan
- Penyimpanan berasingan nilai pengesahan frasa laluan
- Penggunaan Firebase Authentication
- Permintaan kebenaran minimum

Walau bagaimanapun, risiko mungkin timbul bergantung pada status keselamatan peranti pengguna, seperti rooting, jailbreaking, perisian hasad, atau penggunaan peranti bersama.

## 13. Data Peribadi Kanak-Kanak

Aplikasi ini tidak direka sebagai perkhidmatan yang ditujukan terutamanya kepada kanak-kanak. Walau bagaimanapun, pilihan berkaitan umur dalam UMP mungkin digunakan semasa pemprosesan iklan/persetujuan.

## 14. Perubahan kepada Dasar Ini

Dasar ini mungkin disemak semula disebabkan perubahan dalam undang-undang, perkhidmatan pihak ketiga, atau ciri aplikasi.

- Kemas kini terakhir untuk versi semasa: **2026-04-19**

## 15. Hubungi

- Pembangun: frog-im
- E-mel: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Panduan pemadaman akaun: [Arahan pemadaman](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)


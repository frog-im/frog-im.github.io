---
title: Kebijakan Privasi | QDiary
description: Kebijakan Privasi QDiary
---

# Kebijakan Privasi (QDiary)

- Nama Aplikasi: QDiary
- Pengembang: frog-im
- Kontak: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Tanggal Berlaku: 2026-04-19
- Terakhir Diperbarui: 2026-04-19

Kebijakan Privasi ini disusun berdasarkan implementasi QDiary saat ini. QDiary menyediakan fitur penulisan diary, pembuatan dan refleksi quest, login, penyimpanan cloud manual, iklan, dan notifikasi, dan dalam proses tersebut dapat memproses data pribadi atau informasi yang dapat dianggap sebagai data pribadi sejauh diperlukan.

## 1. Fitur yang Disediakan

QDiary menyediakan fitur berikut:

- Menulis, mengedit, dan melihat diary
- Klasifikasi kategori dan tampilan kalender
- Pembuatan quest, refleksi quest, dan penanganan penyelesaian quest
- Kunci aplikasi diary lokal dan enkripsi lokal
- Login email, verifikasi email, login anonim (tamu), dan reset kata sandi
- Simpan dan muat cloud yang dipicu oleh pengguna
- Penayangan iklan dan penanganan opsi privasi iklan
- Notifikasi pengingat quest

## 2. Kategori Informasi yang Diproses

### 2-1. Informasi yang Dimasukkan Langsung oleh Pengguna

- Alamat email
- Kata sandi
- Judul diary, isi, tanggal, kategori, dan tingkat kesulitan
- Respons quest, isi refleksi, dan informasi quest yang dipilih
- Nilai pilihan terkait profil quest dan teks ringkasan
- Frasa sandi untuk kunci aplikasi diary

### 2-2. Informasi yang Disimpan oleh Aplikasi di Perangkat

- Basis data diary lokal (SQLite)
- Informasi status quest untuk diary lokal
- Nilai status terkait kehadiran, pengaturan, bahasa, notifikasi, dan iklan
- Nilai verifikasi kunci aplikasi, salt, dan metadata enkripsi
- Informasi penjadwalan notifikasi quest

### 2-3. Informasi Akun dan Identifikasi

Informasi berikut dapat diproses melalui Firebase Authentication:

- Firebase UID
- Alamat email
- Apakah verifikasi email telah selesai
- Apakah login anonim sedang digunakan

### 2-4. Informasi Iklan dan Persetujuan

Saat menggunakan Google AdMob dan SDK UMP, informasi berikut dapat diproses:

- Pengidentifikasi iklan (seperti Android AD_ID)
- Alamat IP dan informasi jaringan
- Informasi perangkat, versi OS, dan informasi aplikasi
- Informasi tayangan iklan, klik, dan pemrosesan hadiah
- Status persetujuan iklan dan status opsi privasi

### 2-5. Informasi Terkait Notifikasi

- Apakah izin notifikasi telah diberikan
- Nilai pengenal untuk diary yang memiliki quest yang sedang berlangsung
- Teks notifikasi quest
- Waktu notifikasi yang dijadwalkan

## 3. Tujuan Pemrosesan

Aplikasi memproses informasi untuk tujuan berikut:

- Pendaftaran, login, verifikasi email, dan reset kata sandi
- Menulis, menyimpan, dan melihat diary
- Pembuatan quest, refleksi, dan penentuan penyelesaian
- Enkripsi dan dekripsi lokal yang terkait dengan kunci aplikasi
- Simpan dan muat cloud yang diminta oleh pengguna
- Menyediakan notifikasi quest
- Menyediakan iklan, memproses hadiah iklan, dan mencerminkan status persetujuan iklan
- Keamanan, penanganan kesalahan, dan operasional layanan

## 4. Penyimpanan Lokal, Penyimpanan Cloud, dan Pemrosesan Eksternal

### 4-1. Penyimpanan Lokal

Informasi diary dan quest terutama disimpan dalam basis data lokal perangkat.

- Jika kunci aplikasi tidak diaktifkan: disimpan secara lokal dalam bentuk umum
- Jika kunci aplikasi diaktifkan: beberapa informasi, seperti judul diary, isi, dan status quest, dapat dienkripsi dan disimpan secara lokal

### 4-2. Penyimpanan Cloud

Aplikasi hanya menyimpan data di Firebase Firestore ketika pengguna secara langsung menjalankan fitur `Save`.

Berdasarkan konfigurasi proyek saat ini:

- Sinkronisasi penuh otomatis tidak digunakan
- Data disimpan di Firestore `savedDiaries` hanya ketika pengguna menyimpannya secara manual
- Saat disimpan, judul diary, isi, dan status quest dapat disimpan dalam bentuk terenkripsi tergantung pada status kunci aplikasi saat itu
- Data dimuat kembali ke penyimpanan lokal hanya ketika pengguna menjalankan `Load`

### 4-3. Pemrosesan Eksternal untuk Pembuatan dan Refleksi Quest

Ketika pengguna meminta pembuatan quest atau refleksi, informasi berikut dapat digunakan untuk pemrosesan eksternal melalui Firebase Functions:

- Judul diary
- Isi diary atau isi refleksi
- Kategori
- Tingkat kesulitan
- Quest yang dipilih
- Informasi ringkasan profil quest

Informasi ini digunakan untuk pembuatan dan evaluasi quest melalui OpenAI API.

Penting:

- Isi diary yang relevan hanya digunakan untuk pemrosesan eksternal ketika fitur quest digunakan.
- Berdasarkan konfigurasi proyek saat ini, tidak digunakan kode yang menyimpan log quest ke koleksi terpisah `questLogs`.

## 5. Layanan Pihak Ketiga dan Pemrosesan oleh Pihak Ketiga

### 5-1. Google Firebase

Tujuan:

- Autentikasi (Firebase Authentication)
- Penyimpanan Firestore
- Eksekusi Cloud Functions

Informasi yang dapat diproses:

- UID, alamat email, dan status autentikasi
- Data diary yang disimpan secara manual oleh pengguna
- Data permintaan quest

### 5-2. OpenAI

Tujuan:

- Pembuatan quest
- Refleksi quest dan evaluasi penyelesaian

Informasi yang dapat diproses:

- Judul/isi diary
- Teks quest
- Tingkat kesulitan dan kategori
- Isi refleksi yang dimasukkan oleh pengguna
- Informasi ringkasan profil quest

### 5-3. Google AdMob / UMP

Tujuan:

- Menyediakan iklan banner, interstisial, dan berhadiah
- Menangani persetujuan iklan dan opsi privasi

Informasi yang dapat diproses:

- Pengidentifikasi iklan
- Informasi perangkat dan jaringan
- Informasi interaksi iklan
- Status persetujuan

## 6. Pemberitahuan Transfer Internasional

Aplikasi dapat memproses data pribadi atau informasi terkait di luar negara pengguna dalam kasus berikut:

| Item | Detail |
|---|---|
| Penerima | Google LLC, OpenAI, dan operator infrastruktur terkait |
| Negara Tujuan | Amerika Serikat, dan lain-lain |
| Waktu Transfer | Saat login, pembuatan/refleksi quest, permintaan iklan, dan pemrosesan persetujuan |
| Metode Transfer | Komunikasi jaringan terenkripsi |
| Tujuan Transfer | Autentikasi, penyimpanan data, pemrosesan serverless, pembuatan/evaluasi quest berbasis AI, dan penyediaan iklan |

## 7. Masa Retensi dan Penggunaan

Aplikasi menyimpan informasi sesuai dengan standar berikut:

- Informasi diary/pengaturan lokal: sampai pengguna menghapusnya atau menghapus instalasi aplikasi
- Informasi akun Firebase: selama pengguna mempertahankan akun
- Data yang disimpan di Firestore: selama pengguna mempertahankan item yang disimpan
- Data pemrosesan permintaan quest: sejauh diperlukan untuk pemrosesan serverless
- Data terkait iklan/persetujuan: sesuai dengan kebijakan masing-masing penyedia eksternal

Selain itu, proyek saat ini mencakup logika pembersihan otomatis berikut:

- Pembersihan akun pengguna anonim dan data Firestore subkoleksi pengguna setelah jangka waktu tertentu
- Pembersihan akun pengguna reguler yang lama tidak aktif dan data Firestore subkoleksi pengguna

Namun, apakah hal ini benar-benar diterapkan di lingkungan produksi dapat berbeda tergantung pada status deployment dan pengaturan server.

## 8. Pemberitahuan tentang Kunci Aplikasi dan Enkripsi Lokal

Aplikasi menyediakan fitur terpisah `Diary App Lock`.

- Frasa sandi kunci aplikasi terpisah dari kata sandi akun.
- Frasa sandi kunci aplikasi digunakan untuk enkripsi dan dekripsi diary lokal.
- Meskipun frasa sandi yang salah dimasukkan, aplikasi itu sendiri mungkin tidak selalu sepenuhnya terkunci; sebagai gantinya, beberapa isi diary mungkin tetap tidak dapat dibaca.
- Beberapa diary dapat dienkripsi secara terpisah berdasarkan frasa sandi yang digunakan saat penulisan atau saat pembukaan sementara.

Pengguna harus menjaga keamanan frasa sandi mereka, dan jika hilang, pemulihan beberapa data lokal mungkin akan sulit.

## 9. Pemberitahuan tentang Notifikasi Quest

Jika pengguna mengaktifkan notifikasi quest, notifikasi lokal dapat dijadwalkan untuk setiap diary yang memiliki quest yang sedang berlangsung.

- Penjadwalan terutama ditangani oleh sistem penjadwalan internal perangkat.
- Berdasarkan konfigurasi proyek saat ini, tidak ditemukan struktur yang secara berkala mengirimkan teks asli diary ke server pusat semata-mata untuk tujuan notifikasi.

## 10. Pemberitahuan tentang Penggunaan Izin

Aplikasi dapat menggunakan izin berikut untuk menyediakan fiturnya:

- `INTERNET`: komunikasi dengan Firebase, OpenAI, dan SDK iklan
- `com.google.android.gms.permission.AD_ID`: penggunaan pengidentifikasi iklan
- `POST_NOTIFICATIONS`: menampilkan notifikasi quest
- `RECEIVE_BOOT_COMPLETED`: memulihkan notifikasi terjadwal setelah perangkat dihidupkan ulang

Izin digunakan hanya sejauh diperlukan untuk menjalankan fungsi yang terkait.

## 11. Hak Subjek Data dan Cara Menggunakannya

Pengguna dapat menggunakan hak berikut:

- Mengakses, mengubah, dan menghapus data di dalam aplikasi
- Menghapus atau menimpa data yang disimpan di cloud
- Meminta logout dan penghapusan akun
- Mengubah opsi privasi iklan
- Menonaktifkan izin notifikasi

Cara menggunakan hak-hak tersebut:

- Menghapus atau mengedit diary secara langsung di dalam aplikasi
- Menghapus aplikasi atau mereset data lokal
- Logout dari akun dan meminta penghapusan secara terpisah
- Mengubah notifikasi, pengidentifikasi iklan, dan izin di pengaturan perangkat
- Email kontak: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Langkah-Langkah Keamanan

Aplikasi menerapkan atau dapat menerapkan langkah perlindungan berikut:

- Komunikasi berbasis HTTPS
- Kunci aplikasi diary lokal dan enkripsi
- Penyimpanan terpisah nilai verifikasi frasa sandi
- Penggunaan Firebase Authentication
- Permintaan izin minimum

Namun, risiko dapat timbul tergantung pada status keamanan perangkat pengguna, seperti rooting, jailbreaking, malware, atau penggunaan perangkat bersama.

## 13. Data Pribadi Anak

Aplikasi ini tidak dirancang sebagai layanan yang terutama ditujukan untuk anak-anak. Namun, opsi terkait usia dalam UMP dapat diterapkan selama pemrosesan iklan/persetujuan.

## 14. Perubahan pada Kebijakan Ini

Kebijakan ini dapat direvisi karena perubahan hukum, layanan pihak ketiga, atau fitur aplikasi.

- Terakhir diperbarui untuk versi saat ini: **2026-04-19**

## 15. Kontak

- Pengembang: frog-im
- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Panduan penghapusan akun: [Petunjuk penghapusan](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)


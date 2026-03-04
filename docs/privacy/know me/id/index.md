---
title: Kebijakan Privasi | know_me
description: know_me (PeopleNote, Memory for People) Kebijakan Privasi (Bahasa Indonesia)
---

# Kebijakan Privasi (know_me / PeopleNote, Memory for People)

- **Nama Aplikasi:** know_me (PeopleNote, Memory for People)
- **Pengembang:** frog-im
- **Petugas Perlindungan Informasi Pribadi / Narahubung:** frog-im
- **Kontak:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tanggal Berlaku:** 2026-03-04
- **Terakhir Diperbarui:** 2026-03-04

> Kebijakan ini disusun berdasarkan informasi yang diproses oleh aplikasi dan fitur-fitur terkaitnya.  
> Jika terdapat hukum atau peraturan yang bersifat wajib di negara atau wilayah tertentu, maka hukum atau peraturan tersebut dapat berlaku lebih dahulu.

---

## 1. Tujuan dan Ruang Lingkup

`know_me` adalah aplikasi yang dirancang untuk membantu pengguna mencatat dan mengelola informasi tentang orang, dan bila diperlukan, mencadangkan, memulihkan, serta membagikan informasi tersebut dalam bentuk file PDF.

Fitur utamanya meliputi:

- Menyimpan informasi spesifik tentang orang (seperti nama, teks identifikasi, catatan, sifat kepribadian, negara, jenis kelamin, informasi kontak, dan sebagainya)
- Klasifikasi folder, pencarian, dan fungsi penggabungan
- Melampirkan foto dan mengelola deskripsi
- Mengekspor dan mengimpor cadangan (`.knm`)
- Mengekspor PDF
- Kunci aplikasi (kata sandi / pola)
- Pengelolaan iklan dan persetujuan (AdMob / UMP)

Aplikasi ini tidak memerlukan pendaftaran akun terpisah, dan data utama pengguna pada umumnya disimpan secara lokal di perangkat pengguna.  
Namun, beberapa SDK pihak ketiga yang disertakan untuk pengelolaan iklan dan persetujuan dapat memproses sebagian informasi.

---

## 2. Kategori Informasi Pribadi yang Diproses

### 2-1) Informasi yang Dimasukkan Langsung oleh Pengguna

Informasi berikut hanya disimpan ketika pengguna memasukkannya secara langsung:

- Nama
- Teks identifikasi (seperti penampilan / ciri-ciri yang digunakan sebagai teks catatan)
- Catatan
- Sifat kepribadian, negara, jenis kelamin
- Nomor telepon
- Teks yang berkaitan dengan waktu kemunculan / waktu pertemuan
- Informasi platform / situs
- Nama / warna folder
- Deskripsi gambar (caption)

### 2-2) File yang Dipilih di Perangkat

- File gambar yang dipilih pengguna saat melampirkan foto
- File cadangan `.knm` yang dipilih pengguna saat mengimpor cadangan
- Jalur penyimpanan dan file tersimpan yang dipilih pengguna saat mengekspor PDF / cadangan

### 2-3) Data yang Disimpan Secara Lokal di Dalam Aplikasi

Data berikut dapat disimpan di perangkat pengguna untuk menyediakan fitur aplikasi:

- Basis data SQLite (`people_note.db`): metadata terkait orang / folder / platform / situs / gambar
- File gambar: dienkripsi dan disimpan di folder dokumen aplikasi (`.enc`)
- Pengaturan aplikasi (`SharedPreferences`): tema, pengurutan, opsi privasi / iklan, opsi penyamaran PDF, kebijakan kunci aplikasi, dan sebagainya
- Informasi kunci aplikasi: nilai hash dan salt untuk kata sandi / pola (`SharedPreferences`)
- Kunci enkripsi lokal: disimpan di `flutter_secure_storage`
- File sementara: pratinjau dekripsi gambar, file cache impor / ekspor, dan sebagainya (folder sementara)

### 2-4) Informasi yang Dapat Diproses Secara Otomatis Selama Pengelolaan Iklan dan Persetujuan

Ketika fitur iklan atau pengelolaan persetujuan diaktifkan, SDK milik Google LLC dan mitra terkait (seperti AdMob dan UMP) dapat secara otomatis memproses informasi berikut:

- Pengenal iklan (AAID / IDFA, dan sebagainya)
- Alamat IP dan informasi jaringan
- Informasi perangkat (versi OS, model perangkat, versi aplikasi, dan sebagainya)
- Informasi interaksi dengan iklan (tayangan, klik, dan sebagainya)
- Status persetujuan dan informasi pilihan privasi
- Informasi terkait diagnostik, performa, dan keamanan

Catatan utama pengguna di aplikasi ini pada umumnya tidak diunggah ke server pengembang, tetapi sebagian informasi di atas dapat dikirimkan ke layanan pihak ketiga saat fitur iklan / persetujuan digunakan.

---

## 3. Tujuan Pemrosesan Informasi Pribadi

Aplikasi ini memproses informasi pribadi atau informasi terkait untuk tujuan berikut:

- Mencatat dan menelusuri informasi terkait orang yang berfokus pada kontak / catatan
- Menyediakan fitur pengorganisasian seperti klasifikasi folder, pencarian, dan penggabungan
- Melampirkan dan menampilkan foto
- Menjalankan fitur yang diminta pengguna, seperti pencadangan / pemulihan dan ekspor PDF
- Menyediakan fitur keamanan kunci aplikasi
- Menyediakan iklan, mengelola persetujuan, mencegah aktivitas penipuan, dan mematuhi kewajiban hukum

---

## 4. Jangka Waktu Penyimpanan dan Retensi Informasi Pribadi

- Data internal aplikasi (SQLite, pengaturan lokal, gambar terenkripsi): disimpan di perangkat pengguna hingga aplikasi dihapus, data aplikasi dihapus, atau pengguna menghapus data secara langsung
- File sementara: dihapus setelah tugas terkait selesai atau dibersihkan sesuai kebijakan cache sistem operasi
- File yang diekspor pengguna (PDF, file cadangan): dapat tetap berada di lokasi penyimpanan yang dipilih pengguna dan harus dihapus langsung oleh pengguna
- Data terkait iklan / persetujuan (diproses oleh pihak ketiga): tunduk pada kebijakan masing-masing penyedia layanan dan hukum yang berlaku

Pada prinsipnya, aplikasi ini tidak menyimpan catatan utama pengguna di server pengembang.  
Namun, file yang disimpan langsung oleh pengguna ke penyimpanan eksternal dikelola dalam lingkungan milik pengguna sendiri.

---

## 5. Prosedur dan Metode Penghapusan Informasi Pribadi

Ketika tujuan pemrosesan telah tercapai, atau ketika pengguna meminta penghapusan, aplikasi akan menghapus informasi terkait atau memprosesnya sehingga tidak lagi dirujuk, sebagai berikut.

### 5-1) Prosedur Penghapusan

- Ketika pengguna secara langsung menghapus catatan orang, folder, gambar, data cadangan, dan sebagainya, data tersebut dianggap sebagai subjek penghapusan segera.
- Ketika pengguna menghapus aplikasi atau membersihkan data aplikasi dari pengaturan perangkat, data yang disimpan di area penyimpanan internal aplikasi akan dihapus sesuai prosedur penghapusan sistem operasi.
- File sementara akan menjadi subjek pembersihan setelah tugas terkait berakhir, dan sebagian data cache dapat tetap tersimpan untuk jangka waktu tertentu tergantung pada kebijakan sistem operasi.

### 5-2) Metode Penghapusan

- Data SQLite: penghapusan catatan yang relevan
- Pengaturan aplikasi (`SharedPreferences`): penghapusan kunci yang relevan atau seluruh pengaturan
- Nilai pada `flutter_secure_storage`: penghapusan item penyimpanan aman yang relevan
- File internal aplikasi (gambar terenkripsi, file sementara, dan sebagainya): penghapusan file yang relevan
- PDF / file cadangan yang disimpan langsung oleh pengguna di penyimpanan eksternal: tidak dihapus secara otomatis oleh aplikasi dan harus dihapus langsung oleh pengguna

Kecuali diwajibkan lain oleh hukum yang berlaku, pengembang tidak menyimpan secara terpisah catatan utama pengguna di server pengembang.

---

## 6. Penyediaan kepada Pihak Ketiga, Penugasan Pemrosesan, dan Transfer Lintas Batas

Aplikasi ini dapat menggunakan layanan Google untuk pengelolaan iklan dan persetujuan.

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

Pengembang tidak mengumpulkan atau menjual data inti catatan orang dari aplikasi ini melalui server miliknya sendiri.

---

## 7. Informasi tentang Izin yang Digunakan

Aplikasi ini dapat menggunakan izin berikut:

- `INTERNET`: komunikasi untuk SDK iklan dan fitur jaringan terkait
- `com.google.android.gms.permission.AD_ID`: penggunaan pengenal iklan (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 dan di bawahnya): melampirkan / memilih foto

Izin hanya digunakan dalam lingkup yang diperlukan untuk menyediakan fitur terkait.

---

## 8. Pemasangan, Pengoperasian, dan Penolakan terhadap Mekanisme Pengumpulan Otomatis

Aplikasi ini tidak secara langsung menggunakan cookie situs web umum.  
Namun, sehubungan dengan fitur iklan dan pengelolaan persetujuan, SDK pihak ketiga dapat secara otomatis memproses pengenal iklan, informasi jaringan, informasi perangkat, dan data serupa.

Pengguna dapat menyesuaikan pengaturan terkait dengan cara berikut:

- Mengubah pilihan dalam opsi privasi aplikasi atau layar pengelolaan persetujuan (jika tersedia)
- Mengatur ulang atau menghapus pengenal iklan di pengaturan sistem operasi perangkat
- Membatasi iklan yang dipersonalisasi atau menyesuaikan opsi privasi terkait di pengaturan sistem operasi perangkat

Jika pengguna membatasi iklan yang dipersonalisasi, iklan non-personalisasi dapat ditampilkan, atau beberapa fitur terkait iklan dapat dibatasi.

---

## 9. Hak Pengguna dan Cara Menggunakannya

Tunduk pada hukum yang berlaku, pengguna dapat memiliki hak-hak berikut:

- Meminta akses, koreksi, atau penghapusan informasi pribadi
- Meminta penangguhan atau pembatasan pemrosesan
- Menarik persetujuan untuk pemrosesan yang berbasis persetujuan
- Mengubah pilihan iklan / persetujuan

Hak-hak ini dapat digunakan melalui cara berikut:

- Mengubah atau menghapus data secara langsung di dalam aplikasi
- Menginisialisasi data lokal dengan menghapus data aplikasi atau mencopot pemasangan aplikasi
- Mengubah persetujuan iklan melalui opsi privasi / layar persetujuan aplikasi (di wilayah tempat fitur tersebut tersedia)
- Mengatur ulang / menghapus pengenal iklan atau membatasi iklan yang dipersonalisasi melalui pengaturan OS perangkat
- Kontak: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Langkah-Langkah Keamanan

Pengembang menerapkan atau berupaya menerapkan langkah-langkah berikut:

- Catatan pengguna umumnya disimpan secara lokal di perangkat
- File gambar terlampir disimpan secara lokal dalam bentuk terenkripsi (berbasis AES-GCM)
- Informasi kunci aplikasi disimpan dalam bentuk hash, bukan teks biasa
- File cadangan disimpan setelah dienkripsi berdasarkan kata sandi pengguna
- Komunikasi dengan SDK pihak ketiga dienkripsi (HTTPS / TLS)
- Izin digunakan dengan cakupan akses seminimal mungkin

Namun, risiko yang timbul dari kondisi keamanan perangkat pengguna (seperti rooting / jailbreaking, aplikasi berbahaya, atau terbukanya penyimpanan bersama) tidak dapat sepenuhnya dihilangkan.

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

Terakhir Diperbarui: **2026-03-04**
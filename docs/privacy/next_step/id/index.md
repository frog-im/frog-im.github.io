---
title: Kebijakan Privasi | Next Step
description: Kebijakan Privasi Next Step
lang: id
last_updated: 2026-07-08
---

# Kebijakan Privasi (Next Step)

- **Nama aplikasi:** Next Step (다음한걸음)
- **Pengembang:** frog-im
- **Kontak privasi:** frog-im
- **Kontak:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tanggal berlaku:** 2026-07-08
- **Terakhir diperbarui:** 2026-07-08

> Kebijakan ini disusun berdasarkan implementasi Next Step saat ini. Jika ada ketentuan wajib di suatu negara atau wilayah, ketentuan tersebut dapat berlaku lebih dahulu.

---

## 1. Tujuan dan ruang lingkup

Next Step adalah aplikasi refleksi diri berbasis lokal yang membantu pengguna mengatur dan meninjau masalah berulang, penyebab, tindakan berikutnya, dan catatan pelaksanaan di perangkatnya sendiri.

Aplikasi tidak mewajibkan pendaftaran atau login. Pengembang tidak mengoperasikan server milik pengembang yang menerima isi catatan, informasi folder, file cadangan, PIN, informasi biometrik, atau data statistik. Namun, untuk menyediakan iklan dan pilihan privasi iklan, aplikasi dapat menggunakan Google AdMob dan Google User Messaging Platform (UMP).

## 2. Informasi yang diproses

### 2-1. Data catatan yang dimasukkan atau dibuat langsung oleh pengguna

Untuk menyediakan fitur, aplikasi dapat memproses informasi berikut di perangkat.

- Masalah, alasan, tindakan berikutnya, dan catatan pelaksanaan yang ditulis pengguna
- Emosi, tingkat penting, tag, kategori, dan status selesai
- Waktu pembuatan, waktu perubahan, dan status penyelesaian catatan
- Nama folder, warna, dan informasi folder induk yang dibuat atau diubah pengguna
- Hasil perhitungan lokal untuk layar tinjauan, statistik, eksekusi makro, dan retrospektif

Informasi ini diproses di perangkat pengguna untuk menyediakan fitur aplikasi. Pengembang tidak mengunggahnya ke server milik pengembang.

### 2-2. Informasi autentikasi dan keamanan

Untuk menyediakan kunci aplikasi, aplikasi dapat memproses informasi berikut di penyimpanan aman perangkat.

- Apakah kunci aplikasi diaktifkan
- Hash PIN dan salt
- Apakah autentikasi biometrik diaktifkan
- Informasi pengaturan seperti waktu pembaruan terkait kunci

PIN asli tidak disimpan atau dikirim kepada pengembang. Autentikasi biometrik dilakukan oleh sistem operasi; aplikasi tidak mengumpulkan gambar sidik jari, gambar wajah, atau templat biometrik, dan hanya memeriksa apakah autentikasi berhasil.

### 2-3. Cadangan lokal, pemulihan, dan berbagi

Saat pengguna mengekspor, memulihkan, atau membagikan data secara langsung, aplikasi dapat memproses informasi berikut.

- File cadangan JSON yang berisi catatan dan folder
- Nama file cadangan, waktu pembuatan, dan informasi hasil pemulihan
- File gambar yang dibuat saat membagikan gambar tinjauan
- Jalur file yang dipilih pengguna atau hasil pemilih dokumen dari sistem operasi

File cadangan dan gambar tinjauan hanya dibuat ketika pengguna mengekspor atau membagikannya secara langsung. Pengembang tidak menerima file tersebut di server milik pengembang.

### 2-4. Informasi yang dapat diproses otomatis selama iklan dan persetujuan

Pada platform yang didukung, aplikasi dapat menggunakan Google AdMob dan UMP. Google dan penyedia teknologi iklan dapat memproses informasi berikut.

- ID iklan, ID instans aplikasi, atau ID terkait perangkat
- Alamat IP dan perkiraan lokasi yang disimpulkan dari alamat IP atau data serupa
- Model perangkat, sistem operasi, versi aplikasi, bahasa, dan informasi jaringan
- Permintaan iklan, tayangan, klik, interaksi, dan informasi diagnostik
- Status persetujuan iklan dan pilihan privasi regional

Informasi ini dapat diproses untuk penayangan iklan, iklan non-personalisasi, pembatasan frekuensi, pengukuran, pencegahan penyalahgunaan, pengelolaan persetujuan, keamanan, dan kepatuhan hukum. Aplikasi diimplementasikan untuk meminta iklan hanya saat permintaan iklan dimungkinkan setelah proses UMP.

Cara pemrosesan Google dijelaskan dalam [Kebijakan Privasi Google](https://policies.google.com/privacy) dan [panduan teknologi iklan Google](https://policies.google.com/technologies/ads).

## 3. Tujuan pemrosesan

Next Step memproses informasi untuk tujuan berikut.

- Menyimpan dan menampilkan catatan, penyebab, tindakan berikutnya, emosi, tag, dan folder
- Mengelola status penyelesaian catatan dan alur retrospektif
- Menyediakan hasil analisis lokal seperti tinjauan, statistik, masalah berulang, dan tindakan tersisa
- Mengontrol akses melalui kunci aplikasi, PIN, dan autentikasi biometrik
- Membuat dan memulihkan file cadangan serta membagikan gambar tinjauan
- Menyimpan pengaturan aplikasi seperti bahasa, tema, dan pilihan privasi iklan
- Menyediakan iklan, mengelola frekuensi iklan, dan menyediakan pilihan privasi
- Mencegah penyalahgunaan, menjaga keamanan layanan, dan mematuhi kewajiban hukum

## 4. Lokasi penyimpanan dan periode retensi

| Kategori | Lokasi dan periode penyimpanan | Cara menghapus |
|---|---|---|
| Data inti seperti catatan, folder, dan status selesai | Penyimpanan lokal khusus aplikasi sampai pengguna menghapusnya | Hapus di aplikasi, hapus data aplikasi, atau hapus instalasi aplikasi |
| Pengaturan kunci aplikasi, hash PIN, dan pengaturan biometrik | Penyimpanan aman sistem operasi sampai pengaturan diubah atau data aplikasi dihapus | Nonaktifkan fitur terkait, hapus data aplikasi, atau hapus instalasi aplikasi |
| File cadangan | Folder perangkat, penyedia dokumen, atau lokasi eksternal yang dipilih pengguna sampai dihapus | Hapus melalui aplikasi pengelola file atau layanan penyimpanan terkait |
| Gambar tinjauan | Dibuat sementara tepat sebelum berbagi dan diproses oleh sistem operasi atau aplikasi yang dipilih | Keluar dari aplikasi, bersihkan cache, atau hapus dari aplikasi/lokasi berbagi |
| Informasi iklan Google | Disimpan sesuai kebijakan dan kewajiban hukum Google serta pemroses terkait | Ubah pengaturan iklan aplikasi/perangkat atau gunakan pengaturan privasi Google |

Sistem operasi, produsen perangkat, penyedia file, atau layanan penyimpanan cloud dapat menyimpan salinan terpisah atas data aplikasi atau file cadangan yang dibuat pengguna. Salinan tersebut tunduk pada kebijakan penyedia terkait.

## 5. Penyediaan kepada pihak ketiga, penugasan pemrosesan, dan penjualan

Pengembang tidak menjual isi catatan, PIN, atau data lokal dalam aplikasi, dan tidak memberikannya kepada pihak ketiga melalui server milik pengembang.

Jika fitur iklan atau persetujuan berjalan, Google LLC, afiliasi Google, penyedia teknologi iklan, dan pemroses terkait dapat memproses informasi pada Bagian 2-4. Untuk detail, lihat [Pemberitahuan Transfer Data Internasional](policy/).

Jika pengguna langsung memilih aplikasi eksternal atau layanan cloud untuk menyimpan file cadangan, memilih file, atau membagikan gambar tinjauan, penyedia tersebut dapat memproses file sesuai instruksi pengguna. Dalam hal ini, kebijakan privasi dan pengaturan keamanan penyedia tersebut berlaku, dan pengembang tidak mengendalikan cara pemrosesan oleh layanan eksternal yang dipilih pengguna.

## 6. Transfer data internasional

Catatan dan data inti aplikasi tidak ditransfer ke server milik pengembang. Namun, saat fitur iklan dan persetujuan digunakan, Google dan pemroses terkait dapat memproses informasi terkait iklan dan persetujuan di Amerika Serikat dan negara lain tempat infrastruktur mereka beroperasi.

Jika pengguna memilih layanan cloud luar negeri atau layanan berbasis server luar negeri sebagai lokasi cadangan atau tujuan berbagi, file dapat ditransfer atau disinkronkan ke server luar negeri sesuai pilihan pengguna. Untuk detail, lihat [Pemberitahuan Transfer Data Internasional](policy/).

## 7. Penggunaan izin

Aplikasi dapat menggunakan izin atau fungsi sistem berikut saat pengguna menggunakan fitur terkait.

- **Pemilihan dan penyimpanan file:** digunakan untuk memilih atau menyimpan file cadangan
- **Autentikasi biometrik:** digunakan untuk membuka kunci aplikasi atau mengonfirmasi ulang perubahan pengaturan sensitif
- **Internet dan status jaringan:** digunakan untuk meminta iklan AdMob dan informasi persetujuan UMP
- **ID iklan:** digunakan untuk menyediakan fitur iklan Google

Jika izin tidak diberikan, hanya fitur terkait yang dapat dibatasi. Saat pemilih file sistem digunakan, akses aplikasi pada prinsipnya terbatas pada item yang dipilih pengguna.

## 8. Langkah keamanan dan batasan

Implementasi saat ini menggunakan langkah berikut.

- Menyimpan data catatan dan folder di penyimpanan lokal perangkat
- Menyimpan hash PIN dan salt di penyimpanan aman
- Menggunakan autentikasi biometrik sistem operasi pada perangkat yang didukung
- Menyimpan status kunci aplikasi dan pengaturan keamanan di penyimpanan aman
- Memungkinkan pengguna membuat, menyimpan, dan memulihkan file cadangan secara langsung

Tidak ada metode keamanan yang dapat sepenuhnya menghilangkan semua risiko. Informasi dapat terekspos karena perangkat hilang, malware, kerentanan sistem operasi, PIN lemah, file yang dibagikan langsung oleh pengguna, atau masalah keamanan layanan penyimpanan eksternal.

Jika file cadangan atau gambar tinjauan disimpan atau dibagikan melalui aplikasi eksternal atau layanan cloud, salinan terpisah dapat tetap berada di lokasi tersebut. Pengguna harus memeriksa sendiri apakah terdapat informasi sensitif.

## 9. Hak dan pilihan pengguna

Karena sebagian besar informasi hanya ada di perangkat pengguna, pengembang tidak dapat melihat, mengubah, atau menghapusnya dari jarak jauh. Pengguna dapat mengelola informasi dengan cara berikut.

- Menghapus catatan, folder, atau catatan penyelesaian di aplikasi
- Mengubah kunci aplikasi, PIN, autentikasi biometrik, bahasa, dan tema
- Menghapus data aplikasi atau menghapus instalasi aplikasi
- Menghapus file cadangan dan file yang dibagikan dari lokasi penyimpanannya
- Jika berlaku, mengubah persetujuan pada layar pilihan privasi iklan Google di aplikasi
- Menghapus atau menyetel ulang ID iklan, atau membatasi personalisasi iklan, di pengaturan perangkat

Permintaan terkait informasi yang diberikan langsung oleh pengguna dan dimiliki pengembang, seperti email pertanyaan, dapat dikirim ke kontak di bawah ini. Jika diakui oleh hukum yang berlaku, hak akses, perbaikan, penghapusan, pembatasan pemrosesan, penarikan persetujuan, dan pengaduan kepada otoritas pengawas dapat tersedia.

## 10. Privasi anak

Next Step tidak dirancang terutama untuk anak-anak dan tidak meminta anak-anak memasukkan informasi pribadi. Wali dapat menggunakan fitur kontrol orang tua pada perangkat atau toko aplikasi.

## 11. Kontak

Pertanyaan terkait pemrosesan informasi pribadi:

- **Penanggung jawab:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Permintaan terkait informasi iklan yang diproses oleh Google dapat dilakukan melalui kontrol privasi dan prosedur kontak yang dijelaskan dalam [Kebijakan Privasi Google](https://policies.google.com/privacy).

## 12. Perubahan kebijakan

Kebijakan ini dapat direvisi jika hukum, fitur aplikasi, izin, atau cara pemrosesan SDK pihak ketiga berubah. Perubahan penting dapat diberitahukan melalui halaman ini, layar dalam aplikasi, atau halaman distribusi.

Terakhir diperbarui: **2026-07-08**

---
title: Kebijakan Privasi | FileGuard
description: Kebijakan Privasi FileGuard
lang: id
last_updated: 2026-06-23
---

# Kebijakan Privasi (FileGuard)

- **Aplikasi:** FileGuard
- **Pengembang:** frog-im
- **Kontak privasi:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tanggal berlaku:** 23 Juni 2026
- **Terakhir diperbarui:** 23 Juni 2026

> Kebijakan ini menjelaskan implementasi saat ini dari aplikasi FileGuard. Hukum wajib di negara atau wilayah Anda dapat berlaku lebih dahulu.

---

## 1. Ruang lingkup dan tujuan

FileGuard adalah utilitas keamanan yang memungkinkan Anda menyimpan file yang dipilih, media yang diambil, catatan, dan teks papan klip dalam brankas terenkripsi di perangkat Anda serta membuat file cadangan terenkripsi.

Aplikasi tidak memerlukan pendaftaran atau masuk. Pengembang tidak mengoperasikan server yang menerima file brankas, isi file, kata sandi, nama brankas, atau riwayat aktivitas Anda. Namun, pada Android, aplikasi dapat menggunakan Google AdMob dan Google User Messaging Platform (UMP) untuk iklan dan pilihan privasi.

## 2. Informasi yang diproses

### 2.1 Data brankas yang Anda pilih atau buat

Aplikasi dapat memproses informasi berikut di perangkat Anda:

- Foto, video, dokumen, dan file lain yang Anda pilih melalui pemilih file sistem
- Foto atau video yang diambil dengan aplikasi, termasuk audio yang direkam bersama video
- Teks papan klip yang Anda simpan secara manual atau yang terdeteksi saat Anda mengaktifkan perlindungan papan klip otomatis
- Nama file, jenis MIME, ukuran, waktu pembuatan, keterangan, dan informasi terkait pratinjau
- Nama dan pengenal brankas, klasifikasi keamanan, status file asli, dan referensi file asli
- Paket ekspor, transfer, atau cadangan terenkripsi yang Anda buat

Informasi ini diproses di perangkat Anda untuk menyediakan fitur aplikasi. Pengembang tidak mengunggahnya ke server yang dioperasikan oleh pengembang.

### 2.2 Informasi autentikasi dan keamanan

Aplikasi dapat memproses informasi berikut dalam penyimpanan aman di perangkat Anda:

- Salt, pengaturan derivasi kunci, dan bundel kunci terenkripsi yang digunakan untuk menurunkan atau melindungi kunci enkripsi
- Kredensial akses brankas dan kunci lokal yang dilindungi oleh kunci terikat perangkat untuk akses biometrik
- Preferensi keamanan seperti perlindungan tangkapan layar, pembersihan papan klip, autentikasi ulang biometrik, dan perlindungan otomatis

Kata sandi teks biasa Anda tidak dikirim kepada pengembang. Autentikasi biometrik dilakukan oleh sistem operasi. Aplikasi tidak mengumpulkan gambar sidik jari atau wajah maupun templat biometrik; aplikasi hanya menerima hasil autentikasi.

### 2.3 Informasi aktivitas lokal dan cadangan

Aplikasi dapat menyimpan secara lokal:

- Jenis, deskripsi, waktu, dan pengenal item terkait untuk peristiwa perlindungan, penguncian, penghapusan, penghapusan asli, pencadangan, dan pemulihan
- Hingga 500 entri log aktivitas
- Tujuan cadangan, waktu cadangan terakhir, jumlah item, dan status berhasil atau gagal
- Apakah pencadangan otomatis diaktifkan dan kata sandi yang diperlukan untuk memperbarui cadangan tersebut
- Pilihan privasi iklan, pilihan pemrosesan data terbatas, dan jumlah item terlindungi yang digunakan untuk frekuensi iklan

Pengaturan sensitif, termasuk status cadangan dan kata sandi pencadangan otomatis, disimpan dalam penyimpanan lokal yang terenkripsi dengan kunci perangkat. Anda bertanggung jawab menjaga keamanan kata sandi cadangan Anda.

### 2.4 Informasi yang diproses selama iklan dan persetujuan

Pada platform iklan yang didukung, saat ini Android, aplikasi dapat menggunakan Google AdMob dan UMP. Google dan penyedia teknologi periklanan dapat memproses:

- Pengenal terkait iklan, instance aplikasi, atau perangkat
- Alamat IP dan perkiraan lokasi yang disimpulkan dari informasi seperti alamat IP
- Model perangkat, sistem operasi, versi aplikasi, bahasa, dan informasi jaringan
- Permintaan iklan, tayangan, klik, interaksi, dan diagnostik
- Status persetujuan dan pilihan privasi regional

Informasi ini dapat digunakan untuk penayangan iklan, iklan non-personalisasi, pembatasan frekuensi, pengukuran, pencegahan penipuan, pengelolaan persetujuan, keamanan, dan kepatuhan hukum. Aplikasi diimplementasikan untuk menginisialisasi Google Mobile Ads SDK hanya setelah UMP menunjukkan bahwa iklan dapat diminta.

Lihat [Kebijakan Privasi Google](https://policies.google.com/privacy) dan [informasi teknologi periklanan Google](https://policies.google.com/technologies/ads).

## 3. Tujuan pemrosesan

FileGuard memproses informasi untuk:

- Menyimpan dan menampilkan konten yang dipilih atau diambil dalam brankas terenkripsi
- Mengontrol akses brankas dengan penguncian, kata sandi, dan autentikasi biometrik
- Mengimpor, mengekspor, memindahkan, menghapus, dan melacak status file asli konten
- Membuat dan memulihkan cadangan terenkripsi di lokasi yang Anda pilih
- Menjaga preferensi keamanan dan membersihkan file sementara yang didekripsi serta isi papan klip
- Menampilkan aktivitas keamanan lokal dan status kesalahan
- Menayangkan iklan Android, mengontrol frekuensi iklan, dan menyediakan pilihan privasi
- Mencegah penyalahgunaan, mengamankan layanan, dan mematuhi kewajiban hukum

## 4. Penyimpanan dan retensi

| Kategori | Penyimpanan dan retensi | Cara menghapus |
|---|---|---|
| File dan metadata brankas terenkripsi | Disimpan dalam penyimpanan lokal privat aplikasi sampai Anda menghapusnya | Hapus item atau brankas di aplikasi, hapus data aplikasi, atau copot pemasangan |
| Kredensial dan pengaturan keamanan | Disimpan dalam penyimpanan aman sistem operasi dan penyimpanan terenkripsi kunci perangkat sampai diubah atau data aplikasi dihapus | Nonaktifkan fitur terkait, hapus data aplikasi, atau copot pemasangan |
| Riwayat aktivitas | Hingga 500 entri dalam penyimpanan lokal terenkripsi | Hapus data aplikasi atau copot pemasangan |
| File sementara yang didekripsi | Ditulis sementara ke cache aplikasi dan dibersihkan saat mulai, masuk latar belakang, atau fitur selesai dengan upaya terbaik | Tutup aplikasi atau hapus cache/datanya |
| Isi papan klip | Diproses melalui papan klip sistem operasi saat salin atau perlindungan otomatis digunakan | Pembersihan otomatis dengan upaya terbaik, salin konten lain, atau mulai ulang perangkat |
| File cadangan terenkripsi | Disimpan dalam folder perangkat, penyedia dokumen, atau lokasi tersinkron cloud yang Anda pilih sampai Anda menghapusnya | Hapus melalui pengelola file atau layanan penyimpanan terkait |
| Data iklan Google | Disimpan sesuai kebijakan Google dan pemroses serta kewajiban hukum | Ubah pengaturan iklan aplikasi/perangkat atau gunakan kontrol privasi Google |

Sistem operasi, produsen perangkat, penyedia dokumen, atau penyedia cadangan cloud dapat menyimpan salinan terpisah dari data aplikasi atau file cadangan yang Anda buat. Salinan tersebut diatur oleh kebijakan penyedia terkait.

## 5. Pihak ketiga, penyedia layanan, dan penjualan

Pengembang tidak menjual konten brankas, kata sandi, atau riwayat aktivitas dalam aplikasi dan tidak menyediakannya kepada pihak ketiga melalui server yang dioperasikan pengembang.

Saat fitur iklan atau persetujuan Android beroperasi, Google LLC, afiliasi Google, penyedia teknologi periklanan, dan pemroses terkait dapat memproses informasi yang dijelaskan dalam Bagian 2.4. Lihat [Pemberitahuan Transfer Data Internasional](policy/) terpisah.

Jika Anda langsung memilih aplikasi eksternal atau layanan cloud melalui pemilih file, fungsi berbagi, atau tujuan cadangan, penyedia tersebut dapat memproses file atas arahan Anda. Kebijakan privasi dan pengaturan keamanannya berlaku, dan pengembang tidak mengontrol praktik penyedia tersebut.

## 6. Transfer data internasional

Konten brankas tidak ditransfer ke server yang dioperasikan oleh pengembang. Informasi iklan dan persetujuan dapat diproses oleh Google dan pemroses terkait di Amerika Serikat dan negara lain tempat mereka mengoperasikan infrastruktur.

Jika Anda memilih layanan cloud luar negeri sebagai lokasi cadangan terenkripsi, file dapat disinkronkan ke server di luar negara Anda atas arahan Anda. Lihat [Pemberitahuan Transfer Data Internasional](policy/) untuk detail.

## 7. Izin

Aplikasi dapat menggunakan izin atau kemampuan sistem berikut saat Anda menggunakan fitur terkait:

- **File dan foto:** Mengimpor hanya konten yang Anda pilih
- **Kamera:** Mengambil foto atau video untuk brankas
- **Mikrofon:** Menyertakan audio saat merekam video
- **Biometrik:** Mengonfirmasi akses brankas atau perubahan pengaturan sensitif
- **Internet dan status jaringan di Android:** Meminta iklan AdMob dan informasi persetujuan UMP
- **ID iklan di Android:** Mendukung fitur iklan Google
- **Papan klip:** Menyalin konten atau melindungi teks papan klip saat Anda secara eksplisit mengaktifkan perlindungan otomatis

Menolak izin dapat menonaktifkan hanya fitur terkait. Saat pemilih file sistem digunakan, akses umumnya terbatas pada item yang Anda pilih.

## 8. Langkah keamanan dan batasan

Implementasi saat ini menggunakan langkah-langkah yang meliputi:

- Enkripsi AES-256-GCM untuk konten dan indeks brankas
- Derivasi kunci PBKDF2-HMAC-SHA256 untuk kunci berbasis kata sandi
- Perlindungan Android Keystore atau StrongBox untuk kunci lokal pada perangkat Android yang didukung
- Enkripsi kunci perangkat untuk pengaturan sensitif dan riwayat aktivitas
- Penguncian brankas serta pembersihan file sementara dan papan klip dengan upaya terbaik saat aplikasi masuk latar belakang
- Perlindungan tangkapan layar opsional dan autentikasi ulang biometrik
- Paket cadangan portabel terenkripsi kata sandi

Tidak ada metode keamanan yang menghilangkan semua risiko. Pencurian perangkat, malware, kerentanan sistem operasi, kata sandi lemah, file yang Anda bagikan, atau masalah keamanan pada penyedia penyimpanan eksternal dapat mengekspos informasi.

Membuka atau mengekspor konten yang didekripsi ke aplikasi lain dapat membuat salinan terpisah. Penghapusan file asli dan pembersihan file sementara atau papan klip dapat dibatasi oleh sistem operasi, jadi Anda harus memverifikasi penghapusan konten sensitif.

## 9. Hak dan pilihan Anda

Sebagian besar informasi tetap hanya di perangkat Anda, sehingga pengembang tidak dapat mengakses, memperbaiki, atau menghapusnya dari jarak jauh. Anda dapat:

- Menghapus item brankas atau brankas di aplikasi
- Mengubah pengaturan keamanan, biometrik, perlindungan otomatis, papan klip, dan pencadangan otomatis
- Menghapus data atau cache aplikasi, atau mencopot pemasangan aplikasi
- Menghapus file cadangan dan ekspor dari lokasi penyimpanannya
- Jika tersedia, mengubah persetujuan melalui opsi privasi iklan Google di aplikasi
- Menghapus atau mereset pengenal iklan atau membatasi personalisasi iklan di pengaturan perangkat

Anda dapat menghubungi kami mengenai informasi yang Anda berikan langsung kepada pengembang, seperti email pertanyaan. Jika berlaku, hukum setempat dapat memberi Anda hak akses, koreksi, penghapusan, pembatasan, penarikan persetujuan, dan pengaduan kepada otoritas pengawas.

## 10. Anak-anak

FileGuard tidak dirancang terutama untuk anak-anak dan tidak mewajibkan anak-anak memberikan informasi pribadi. Wali dapat menggunakan kontrol orang tua yang disediakan oleh perangkat atau toko aplikasi. Konfigurasi persetujuan di bawah umur untuk iklan Android harus ditinjau secara terpisah terhadap audiens yang dituju dan hukum yang berlaku sebelum distribusi.

## 11. Kontak

Untuk pertanyaan tentang Kebijakan ini:

- **Kontak:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Untuk data iklan yang diproses oleh Google, gunakan kontrol privasi dan prosedur kontak yang dijelaskan dalam [Kebijakan Privasi Google](https://policies.google.com/privacy).

## 12. Perubahan pada Kebijakan ini

Kami dapat memperbarui Kebijakan ini ketika hukum, fitur aplikasi, izin, atau praktik SDK pihak ketiga berubah. Perubahan material dapat dikomunikasikan di halaman ini, di aplikasi, atau melalui halaman distribusi.

Terakhir diperbarui: **23 Juni 2026**

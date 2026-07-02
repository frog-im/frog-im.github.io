---
title: Dasar Privasi | FileGuard
description: Dasar Privasi FileGuard
lang: ms
last_updated: 2026-06-23
---

# Dasar Privasi (FileGuard)

- **Aplikasi:** FileGuard
- **Pembangun:** frog-im
- **Hubungan privasi:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tarikh berkuat kuasa:** 23 Jun 2026
- **Terakhir dikemas kini:** 23 Jun 2026

> Dasar ini menjelaskan implementasi saat ini dari aplikasi FileGuard. Hukum wajib di negara atau wilayah Anda dapat berlaku lebih dahulu.

---

## 1. Ruang lingkup dan tujuan

FileGuard adalah utilitas keselamatan yang memungkinkan Anda menyimpan fail yang dipilih, media yang diambil, catatan, dan teks papan keratan dalam peti besi terenkripsi di peranti Anda serta membuat fail sandaran terenkripsi.

Aplikasi tidak memerlukan pendaftaran atau masuk. Pembangun tidak mengoperasikan server yang menerima fail peti besi, isi fail, kata laluan, nama peti besi, atau sejarah aktiviti Anda. Namun, pada Android, aplikasi dapat menggunakan Google AdMob dan Google User Messaging Platform (UMP) untuk iklan dan pilihan privasi.

## 2. Maklumat yang diproses

### 2.1 Data peti besi yang Anda pilih atau buat

Aplikasi dapat memproses maklumat berikut di peranti Anda:

- Foto, video, dokumen, dan fail lain yang Anda pilih melalui pemilih fail sistem
- Foto atau video yang diambil dengan aplikasi, termasuk audio yang direkam bersama video
- Teks papan keratan yang Anda simpan secara manual atau yang terdeteksi saat Anda mengaktifkan perlindungan papan keratan otomatis
- Nama fail, jenis MIME, ukuran, waktu pembuatan, keterangan, dan maklumat terkait pratinjau
- Nama dan pengenal peti besi, klasifikasi keselamatan, status fail asli, dan referensi fail asli
- Paket ekspor, transfer, atau sandaran terenkripsi yang Anda buat

Maklumat ini diproses di peranti Anda untuk menyediakan fitur aplikasi. Pembangun tidak mengunggahnya ke server yang dioperasikan oleh pembangun.

### 2.2 Maklumat pengesahan dan keselamatan

Aplikasi dapat memproses maklumat berikut dalam storan aman di peranti Anda:

- Salt, tetapan derivasi kunci, dan bundel kunci terenkripsi yang digunakan untuk menurunkan atau melindungi kunci enkripsi
- Kredensial akses peti besi dan kunci lokal yang dilindungi oleh kunci terikat peranti untuk akses biometrik
- Preferensi keselamatan seperti perlindungan tangkapan layar, pembersihan papan keratan, pengesahan ulang biometrik, dan perlindungan otomatis

Kata sandi teks biasa Anda tidak dikirim kepada pembangun. Autentikasi biometrik dilakukan oleh sistem pengendalian. Aplikasi tidak mengumpulkan gambar sidik jari atau wajah maupun templat biometrik; aplikasi hanya menerima hasil pengesahan.

### 2.3 Maklumat aktivitas lokal dan sandaran

Aplikasi dapat menyimpan secara lokal:

- Jenis, deskripsi, waktu, dan pengenal item terkait untuk peristiwa perlindungan, penguncian, pemadaman, pemadaman asli, pensandaran, dan pemulihan
- Hingga 500 entri log aktivitas
- Tujuan sandaran, waktu sandaran terakhir, jumlah item, dan status berhasil atau gagal
- Apakah pensandaran otomatis diaktifkan dan kata laluan yang diperlukan untuk memperbarui sandaran tersebut
- Pilihan privasi iklan, pilihan pemprosesan data terbatas, dan jumlah item terlindungi yang digunakan untuk frekuensi iklan

Pengaturan sensitif, termasuk status sandaran dan kata laluan pensandaran otomatis, disimpan dalam storan lokal yang terenkripsi dengan kunci peranti. Anda bertanggung jawab menjaga keselamatan kata laluan sandaran Anda.

### 2.4 Maklumat yang diproses selama iklan dan persetujuan

Pada platform iklan yang didukung, saat ini Android, aplikasi dapat menggunakan Google AdMob dan UMP. Google dan penyedia teknologi periklanan dapat memproses:

- Pengenal terkait iklan, instance aplikasi, atau peranti
- Alamat IP dan perkiraan lokasi yang disimpulkan dari maklumat seperti alamat IP
- Model peranti, sistem pengendalian, versi aplikasi, bahasa, dan maklumat jaringan
- Permintaan iklan, tayangan, klik, interaksi, dan diagnostik
- Status persetujuan dan pilihan privasi regional

Maklumat ini dapat digunakan untuk penayangan iklan, iklan non-personalisasi, pembatasan frekuensi, pengukuran, pencegahan penipuan, pengelolaan persetujuan, keselamatan, dan kepatuhan hukum. Aplikasi diimplementasikan untuk menginisialisasi Google Mobile Ads SDK hanya setelah UMP menunjukkan bahwa iklan dapat diminta.

Lihat [Dasar Privasi Google](https://policies.google.com/privacy) dan [maklumat teknologi periklanan Google](https://policies.google.com/technologies/ads).

## 3. Tujuan pemprosesan

FileGuard memproses maklumat untuk:

- Menyimpan dan menampilkan konten yang dipilih atau diambil dalam peti besi terenkripsi
- Mengontrol akses peti besi dengan penguncian, kata laluan, dan pengesahan biometrik
- Mengimpor, mengekspor, memindahkan, menghapus, dan melacak status fail asli konten
- Membuat dan memulihkan sandaran terenkripsi di lokasi yang Anda pilih
- Menjaga preferensi keselamatan dan membersihkan fail sementara yang didekripsi serta isi papan keratan
- Menampilkan aktivitas keselamatan lokal dan status kesalahan
- Menayangkan iklan Android, mengontrol frekuensi iklan, dan menyediakan pilihan privasi
- Mencegah penyalahgunaan, mengamankan layanan, dan mematuhi kewajiban hukum

## 4. Penyimpanan dan retensi

| Kategori | Penyimpanan dan retensi | Cara menghapus |
|---|---|---|
| File dan metadata peti besi terenkripsi | Disimpan dalam storan lokal privat aplikasi sampai Anda menghapusnya | Hapus item atau peti besi di aplikasi, hapus data aplikasi, atau copot pemasangan |
| Kredensial dan tetapan keselamatan | Disimpan dalam storan aman sistem pengendalian dan storan terenkripsi kunci peranti sampai diubah atau data aplikasi dihapus | Nonaktifkan fitur terkait, hapus data aplikasi, atau copot pemasangan |
| Riwayat aktivitas | Hingga 500 entri dalam storan lokal terenkripsi | Hapus data aplikasi atau copot pemasangan |
| File sementara yang didekripsi | Ditulis sementara ke cache aplikasi dan dibersihkan saat mulai, masuk latar belakang, atau fitur selesai dengan upaya terbaik | Tutup aplikasi atau hapus cache/datanya |
| Isi papan keratan | Diproses melalui papan keratan sistem pengendalian saat salin atau perlindungan otomatis digunakan | Pembersihan otomatis dengan upaya terbaik, salin konten lain, atau mulai ulang peranti |
| File sandaran terenkripsi | Disimpan dalam folder peranti, penyedia dokumen, atau lokasi tersinkron cloud yang Anda pilih sampai Anda menghapusnya | Hapus melalui pengelola fail atau layanan storan terkait |
| Data iklan Google | Disimpan sesuai kebijakan Google dan pemroses serta kewajiban hukum | Ubah tetapan iklan aplikasi/peranti atau gunakan kontrol privasi Google |

Sistem operasi, produsen peranti, penyedia dokumen, atau penyedia sandaran cloud dapat menyimpan salinan terpisah dari data aplikasi atau fail sandaran yang Anda buat. Salinan tersebut diatur oleh kebijakan penyedia terkait.

## 5. Pihak ketiga, penyedia layanan, dan penjualan

Pembangun tidak menjual konten peti besi, kata laluan, atau sejarah aktiviti dalam aplikasi dan tidak menyediakannya kepada pihak ketiga melalui server yang dioperasikan pembangun.

Saat fitur iklan atau persetujuan Android beroperasi, Google LLC, afiliasi Google, penyedia teknologi periklanan, dan pemroses terkait dapat memproses maklumat yang dijelaskan dalam Bagian 2.4. Lihat [Pemberitahuan Transfer Data Internasional](policy/) terpisah.

Jika Anda langsung memilih aplikasi eksternal atau layanan cloud melalui pemilih fail, fungsi berbagi, atau tujuan sandaran, penyedia tersebut dapat memproses fail atas arahan Anda. Dasar privasi dan tetapan keselamatannya berlaku, dan pembangun tidak mengontrol praktik penyedia tersebut.

## 6. Transfer data internasional

Konten peti besi tidak ditransfer ke server yang dioperasikan oleh pembangun. Maklumat iklan dan persetujuan dapat diproses oleh Google dan pemroses terkait di Amerika Syarikat dan negara lain tempat mereka mengoperasikan infrastruktur.

Jika Anda memilih layanan cloud luar negeri sebagai lokasi sandaran terenkripsi, fail dapat disinkronkan ke server di luar negara Anda atas arahan Anda. Lihat [Pemberitahuan Transfer Data Internasional](policy/) untuk detail.

## 7. Kebenaran

Aplikasi dapat menggunakan izin atau kemampuan sistem berikut saat Anda menggunakan fitur terkait:

- **File dan foto:** Mengimpor hanya konten yang Anda pilih
- **Kamera:** Mengambil foto atau video untuk peti besi
- **Mikrofon:** Menyertakan audio saat merekam video
- **Biometrik:** Mengonfirmasi akses peti besi atau perubahan tetapan sensitif
- **Internet dan status jaringan di Android:** Meminta iklan AdMob dan maklumat persetujuan UMP
- **ID iklan di Android:** Mendukung fitur iklan Google
- **Papan klip:** Menyalin konten atau melindungi teks papan keratan saat Anda secara eksplisit mengaktifkan perlindungan otomatis

Menolak izin dapat menonaktifkan hanya fitur terkait. Saat pemilih fail sistem digunakan, akses umumnya terbatas pada item yang Anda pilih.

## 8. Langkah keselamatan dan batasan

Implementasi saat ini menggunakan langkah-langkah yang meliputi:

- Enkripsi AES-256-GCM untuk konten dan indeks peti besi
- Derivasi kunci PBKDF2-HMAC-SHA256 untuk kunci berbasis kata laluan
- Perlindungan Android Keystore atau StrongBox untuk kunci lokal pada peranti Android yang didukung
- Enkripsi kunci peranti untuk tetapan sensitif dan sejarah aktiviti
- Penguncian peti besi serta pembersihan fail sementara dan papan keratan dengan upaya terbaik saat aplikasi masuk latar belakang
- Perlindungan tangkapan layar opsional dan pengesahan ulang biometrik
- Paket sandaran portabel terenkripsi kata laluan

Tidak ada metode keselamatan yang menghilangkan semua risiko. Pencurian peranti, malware, kerentanan sistem pengendalian, kata laluan lemah, fail yang Anda bagikan, atau masalah keselamatan pada penyedia storan eksternal dapat mengekspos maklumat.

Membuka atau mengekspor konten yang didekripsi ke aplikasi lain dapat membuat salinan terpisah. Penghapusan fail asli dan pembersihan fail sementara atau papan keratan dapat dibatasi oleh sistem pengendalian, jadi Anda harus memverifikasi pemadaman konten sensitif.

## 9. Hak dan pilihan anda

Sebagian besar maklumat tetap hanya di peranti Anda, sehingga pembangun tidak dapat mengakses, memperbaiki, atau menghapusnya dari jarak jauh. Anda dapat:

- Menghapus item peti besi atau peti besi di aplikasi
- Mengubah tetapan keselamatan, biometrik, perlindungan otomatis, papan keratan, dan pensandaran otomatis
- Menghapus data atau cache aplikasi, atau mencopot pemasangan aplikasi
- Menghapus fail sandaran dan ekspor dari lokasi storannya
- Jika tersedia, mengubah persetujuan melalui opsi privasi iklan Google di aplikasi
- Menghapus atau mereset pengenal iklan atau membatasi personalisasi iklan di tetapan peranti

Anda dapat menghubungi kami mengenai maklumat yang Anda berikan langsung kepada pembangun, seperti email pertanyaan. Jika berlaku, hukum setempat dapat memberi Anda hak akses, koreksi, pemadaman, pembatasan, penarikan persetujuan, dan pengaduan kepada otoritas pengawas.

## 10. Kanak-kanak

FileGuard tidak dirancang terutama untuk anak-anak dan tidak mewajibkan anak-anak memberikan maklumat pribadi. Wali dapat menggunakan kontrol orang tua yang disediakan oleh peranti atau toko aplikasi. Konfigurasi persetujuan di bawah umur untuk iklan Android harus ditinjau secara terpisah terhadap audiens yang dituju dan hukum yang berlaku sebelum distribusi.

## 11. Hubungan

Untuk pertanyaan tentang Dasar ini:

- **Hubungan:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Untuk data iklan yang diproses oleh Google, gunakan kontrol privasi dan prosedur kontak yang dijelaskan dalam [Dasar Privasi Google](https://policies.google.com/privacy).

## 12. Perubahan pada Dasar ini

Kami dapat memperbarui Dasar ini ketika hukum, fitur aplikasi, izin, atau praktik SDK pihak ketiga berubah. Perubahan material dapat dikomunikasikan di halaman ini, di aplikasi, atau melalui halaman distribusi.

Terakhir dikemas kini: **23 Jun 2026**

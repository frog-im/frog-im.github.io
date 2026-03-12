---
title: Kebijakan Privasi | Subtitle Tool
description: Kebijakan Privasi Subtitle Tool (Subtitle Player & Editor) - Bahasa Indonesia
lang: id
last_updated: 2026-03-11
---

# Kebijakan Privasi (Subtitle Tool / Subtitle Player & Editor)

- **Nama aplikasi:** Subtitle Player & Editor (juga disebut sebagai **Subtitle Tool** dalam Kebijakan ini)
- **Pengembang:** frog-im
- **Kontak:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tanggal berlaku:** 2026-03-11

> Kebijakan ini disusun dengan mengacu pada hukum yang berlaku, termasuk Korean Personal Information Protection Act (PIPA), GDPR / UK GDPR, Swiss FADP, dan undang-undang privasi negara bagian AS yang relevan. Jika terdapat aturan lokal yang wajib berlaku, maka aturan tersebut akan diutamakan.

---

## 1. Tujuan dan Ruang Lingkup

Aplikasi ini menyediakan:

- Pemutaran dan pengeditan subtitle
- Pemutaran video + subtitle dari file yang dipilih oleh pengguna
- Overlay subtitle / lirik mengambang yang ditampilkan di atas aplikasi lain pada Android

Penanganan subtitle yang didukung dapat mencakup format seperti:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

Aplikasi ini **tidak** membuat akun pengguna dan **tidak** mengunggah file subtitle atau media milik pengguna ke server milik pengembang. Parsing subtitle, pengeditan, pratinjau, dan sebagian besar pemrosesan terkait pemutaran dilakukan **secara lokal di perangkat**.

Namun, untuk iklan, pengelolaan persetujuan, dan kepatuhan hukum, SDK pihak ketiga seperti **Google Mobile Ads SDK (AdMob)** dan **Google UMP** dapat memproses informasi tertentu seperti pengenal iklan, sinyal perangkat, dan pilihan persetujuan.

---

## 2. Kategori Informasi yang Kami Proses

### 2-1) File yang Secara Eksplisit Dipilih oleh Pengguna

Aplikasi ini berinteraksi dengan file yang secara eksplisit dipilih oleh pengguna, termasuk:

- **File subtitle**
  - Contoh: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Penggunaan:
    - Pemutaran subtitle di dalam aplikasi
    - Pengeditan subtitle
    - Tampilan subtitle pada overlay
    - Konversi dan ekspor subtitle

- **File media**
  - Contoh: file video atau audio lokal yang dipilih oleh pengguna
  - Penggunaan:
    - Pemutaran video + subtitle
    - Penyelarasan waktu overlay dengan media yang sedang diputar

Poin penting:

- File yang dipilih oleh pengguna diproses secara lokal di perangkat.
- Aplikasi ini tidak mengunggah file tersebut ke server milik pengembang.
- Jalur file dan isi file hanya digunakan untuk pemutaran, overlay, pengeditan, penyimpanan, dan tindakan yang diminta oleh pengguna.

### 2-2) Pengaturan Lokal dan Nilai yang Disimpan

Untuk menyediakan pengaturan yang persisten dan memulihkan keadaan sebelumnya, aplikasi ini menyimpan beberapa nilai secara lokal di perangkat menggunakan `SharedPreferences` atau penyimpanan lokal serupa yang disediakan oleh OS.

Nilai-nilai ini tidak dikirim ke server milik pengembang dan biasanya dihapus jika data aplikasi dibersihkan atau aplikasi dihapus.

#### (1) Pengaturan overlay

Contohnya meliputi:

- `overlay_box_x`
- `overlay_box_y`
- `overlay_text_font`
- `overlay_text_color`
- `overlay_outline_enabled`
- `overlay_outline_color`
- `overlay_outline_width`
- `overlay_force_landscape`
- `overlay_interstitial_count`

Tujuan:

- Memulihkan posisi overlay
- Memulihkan gaya subtitle untuk overlay dan pemutaran subtitle di dalam aplikasi
- Menyimpan preferensi outline / font / orientasi
- Mengontrol logika frekuensi tampilan iklan untuk beberapa alur yang terkait dengan overlay

#### (2) Posisi pemutaran atau overlay terbaru

Contohnya meliputi:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Tujuan:

- Memulihkan atau menyarankan posisi awal subtitle/overlay terbaru
- Melanjutkan pemutaran video + subtitle dengan lebih nyaman

#### (3) Nilai preferensi iklan dan privasi

Contohnya dapat meliputi:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Tujuan:

- Menyimpan pilihan privasi iklan
- Menerapkan pengaturan privasi dan konfigurasi iklan UMP / AdMob

#### (4) Output subtitle yang dibuat oleh pengguna

Saat pengguna menyimpan atau mengekspor file subtitle, aplikasi dapat menulis file subtitle baru ke lokasi yang dipilih oleh pengguna, seperti:

- Downloads
- Folder lain yang dipilih melalui system picker
- Lokasi penyimpanan yang dikelola pengguna

File yang disimpan oleh pengguna ini dapat tetap berada di perangkat setelah aplikasi dihapus, kecuali pengguna menghapusnya secara manual.

#### (5) File sementara dan cache

Aplikasi dan pustaka pihak ketiga dapat membuat file sementara atau cache untuk operasi normal, seperti:

- data cache file picker
- data sementara untuk konversi subtitle
- data cache terkait pemutaran

Data ini hanya dimaksudkan untuk operasi lokal dan tidak diunggah ke server milik pengembang.

#### (6) Cache status persetujuan UMP

Di wilayah tempat Google UMP berlaku, SDK dapat menyimpan cache status persetujuan secara lokal di perangkat.

Hal ini umumnya dapat diatur ulang dengan:

- menghapus data aplikasi, atau
- mengubah pilihan persetujuan di dalam aplikasi jika tersedia entri opsi privasi

### 2-3) Pemrosesan Terkait Overlay Android dan Izin

Di Android, overlay subtitle mengambang dapat menggunakan:

- izin `SYSTEM_ALERT_WINDOW` / tampil di atas aplikasi lain
- izin `POST_NOTIFICATIONS`
- notifikasi foreground service yang diperlukan untuk layanan overlay

Tujuan:

- menampilkan overlay subtitle di atas aplikasi lain
- menjaga layanan overlay tetap berjalan
- memungkinkan Android menampilkan notifikasi overlay / layanan yang diperlukan
- membaca informasi notifikasi media saat diperlukan untuk mendukung progres subtitle

Izin-izin ini hanya digunakan untuk fitur aplikasi yang dipilih oleh pengguna untuk digunakan.

### 2-4) Iklan, Persetujuan, dan Data Terkait (SDK Pihak Ketiga)

Aplikasi ini menggunakan SDK iklan / persetujuan Google, termasuk:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

Aplikasi ini dapat menampilkan:

- iklan banner
- iklan interstisial
- iklan rewarded atau rewarded-interstitial

SDK ini dapat memproses data seperti:

- pengenal iklan (misalnya AAID / IDFA jika berlaku)
- informasi berbasis IP dan terkait jaringan
- metadata perangkat dan aplikasi
- sinyal interaksi iklan
- pilihan persetujuan

Tujuannya dapat mencakup:

- penayangan iklan
- pengukuran dan pelaporan iklan
- pembatasan frekuensi
- pencegahan penipuan
- kepatuhan hukum

Pengembang berupaya mengonfigurasi SDK ini dengan cara yang konsisten dengan pilihan persetujuan pengguna dan hukum yang berlaku.

---

## 3. Cara Kami Memproses dan Menyimpan Data

- **Pengaturan lokal dan data posisi terbaru**
  - disimpan di perangkat sampai data aplikasi dibersihkan atau aplikasi dihapus

- **File sementara / cache**
  - disimpan hanya selama diperlukan untuk operasional, lalu dihapus oleh aplikasi jika memungkinkan secara praktis atau dibersihkan kemudian oleh OS

- **File subtitle yang disimpan pengguna**
  - tetap berada di lokasi penyimpanan yang dipilih pengguna sampai dihapus oleh pengguna

- **Data iklan / persetujuan yang ditangani oleh pihak ketiga**
  - disimpan sesuai dengan kebijakan Google dan hukum yang berlaku

---

## 4. Pemrosesan oleh Pihak Ketiga dan Transfer Lintas Batas

Untuk iklan dan pengelolaan persetujuan, beberapa informasi dapat diproses oleh Google dan mitra terkait.

| Item | Detail |
|---|---|
| Penerima | Google LLC dan afiliasi / pemroses terkait |
| Tujuan | Penayangan iklan, pengukuran, pencegahan penipuan, pengelolaan persetujuan, dan kepatuhan hukum |
| Data yang mungkin diproses | Pengenal iklan, info perangkat/aplikasi, info berbasis IP, data interaksi iklan, status persetujuan |
| Tujuan transfer | Amerika Serikat dan wilayah lain tempat infrastruktur Google beroperasi |
| Masa penyimpanan | Sesuai dengan kebijakan Google dan hukum yang berlaku |

Pengembang berupaya menjaga agar pengungkapan privasi di app store tetap konsisten dengan perilaku SDK yang sebenarnya.

---

## 5. Hak dan Pilihan Anda

Bergantung pada yurisdiksi Anda, Anda mungkin memiliki hak seperti:

- akses
- koreksi
- penghapusan
- pembatasan
- portabilitas
- keberatan
- penarikan persetujuan jika persetujuan menjadi dasar hukumnya

Kontrol praktis meliputi:

- mengubah pilihan iklan / privasi di dalam aplikasi jika tersedia
- menghapus data aplikasi untuk menghapus pengaturan lokal dan preferensi yang disimpan dalam cache
- menghapus instalasi aplikasi
- menghapus secara manual file subtitle yang diekspor dari penyimpanan pengguna
- menggunakan kontrol tingkat OS seperti pengaturan notifikasi, reset ad ID, atau pengaturan personalisasi iklan

Untuk data yang diproses oleh Google, pengguna juga sebaiknya merujuk pada alat privasi dan akun milik Google sendiri jika relevan.

---

## 6. Privasi Anak

Aplikasi ini tidak terutama ditujukan untuk anak-anak.

Tujuan utamanya adalah pemutaran subtitle, pengeditan, tampilan overlay, dan fitur utilitas terkait. Jika sesuai, konfigurasi SDK iklan dapat menerapkan penanda terkait usia atau child-directed flags yang konsisten dengan persyaratan platform dan pengaturan pengembang.

---

## 7. Langkah-Langkah Keamanan

Dalam batas arsitektur aplikasi, pengembang berupaya untuk:

- meminimalkan pengumpulan data dengan menjaga sebagian besar pemrosesan subtitle dan media tetap di perangkat
- menggunakan system file picker dan akses file yang dipicu oleh pengguna
- menggunakan izin sistem secara transparan
- mengandalkan transport jaringan terenkripsi yang digunakan oleh SDK pihak ketiga jika berlaku

Tidak ada metode penyimpanan atau transmisi yang sepenuhnya aman, tetapi aplikasi ini dirancang untuk menghindari pengumpulan data yang tidak perlu oleh pengembang.

---

## 8. Perangkat Lunak Open-Source

Aplikasi ini menggunakan perangkat lunak open-source, termasuk pustaka yang terkait dengan:

- parsing dan serialisasi subtitle
- pemilihan file
- preferensi lokal
- jendela overlay
- pemutaran video
- WebView

Pemberitahuan open-source tersedia di dalam aplikasi. Untuk beberapa komponen, aplikasi dapat menggunakan salinan paket open-source yang dimodifikasi secara lokal sambil tetap mempertahankan pemberitahuan lisensi aslinya.

---

## 9. Kontak

Jika Anda memiliki pertanyaan atau permintaan terkait privasi:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Harap sertakan nama aplikasi **Subtitle Player & Editor** dalam pesan Anda.

---

## 10. Perubahan pada Kebijakan Ini

Kebijakan ini dapat diperbarui jika:

- fitur aplikasi berubah
- izin atau penggunaan SDK berubah
- persyaratan hukum atau platform berubah

Perubahan material akan tercermin pada halaman kebijakan yang diperbarui dan, jika sesuai, di dalam aplikasi.

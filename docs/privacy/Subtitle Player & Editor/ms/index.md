---
title: Dasar Privasi | Subtitle Tool
description: Dasar Privasi Subtitle Tool (Subtitle Player & Editor) - Bahasa Melayu
lang: ms
last_updated: 2026-03-11
---

# Dasar Privasi (Subtitle Tool / Subtitle Player & Editor)

- **Nama aplikasi:** Subtitle Player & Editor (juga dirujuk sebagai **Subtitle Tool** dalam Dasar ini)
- **Pembangun:** frog-im
- **Hubungan:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tarikh berkuat kuasa:** 2026-03-11

> Dasar ini disediakan dengan merujuk kepada undang-undang yang terpakai termasuk Akta Perlindungan Maklumat Peribadi Korea (PIPA), GDPR / UK GDPR, Swiss FADP, dan undang-undang privasi negeri-negeri berkaitan di A.S. Jika terdapat peraturan tempatan mandatori yang terpakai, peraturan tersebut akan diutamakan.

---

## 1. Tujuan dan Skop

Aplikasi ini menyediakan:

- Main balik dan penyuntingan sari kata
- Main balik video + sari kata daripada fail yang dipilih oleh pengguna
- Lapisan sari kata / lirik terapung yang dipaparkan di atas aplikasi lain pada Android

Pengendalian sari kata yang disokong mungkin termasuk format seperti:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

Aplikasi ini **tidak** mewujudkan akaun pengguna dan **tidak** memuat naik fail sari kata atau fail media pengguna ke pelayan milik pembangun sendiri. Penghurai sari kata, penyuntingan, pratonton, dan kebanyakan pemprosesan berkaitan main balik dilakukan **secara setempat pada peranti**.

Walau bagaimanapun, bagi tujuan pengiklanan, pengurusan persetujuan, dan pematuhan undang-undang, SDK pihak ketiga seperti **Google Mobile Ads SDK (AdMob)** dan **Google UMP** boleh memproses maklumat tertentu seperti pengecam pengiklanan, isyarat peranti, dan pilihan persetujuan.

---

## 2. Kategori Maklumat yang Kami Proses

### 2-1) Fail yang Dipilih Secara Jelas oleh Pengguna

Aplikasi ini berinteraksi dengan fail yang dipilih secara jelas oleh pengguna, termasuk:

- **Fail sari kata**
  - Contoh: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Kegunaan:
    - Main balik sari kata di dalam aplikasi
    - Penyuntingan sari kata
    - Paparan sari kata pada lapisan
    - Penukaran dan eksport sari kata

- **Fail media**
  - Contoh: fail video atau audio setempat yang dipilih oleh pengguna
  - Kegunaan:
    - Main balik video + sari kata
    - Penjajaran masa lapisan dengan media yang sedang dimainkan

Perkara penting:

- Fail yang dipilih oleh pengguna diproses secara setempat pada peranti.
- Aplikasi ini tidak memuat naik fail tersebut ke pelayan milik pembangun sendiri.
- Laluan fail dan kandungannya hanya digunakan untuk main balik, lapisan, penyuntingan, penyimpanan, dan tindakan yang diminta oleh pengguna.

### 2-2) Tetapan Tempatan dan Nilai yang Disimpan

Bagi menyediakan tetapan yang berterusan dan memulihkan keadaan terdahulu, aplikasi ini menyimpan beberapa nilai secara tempatan pada peranti menggunakan `SharedPreferences` atau storan tempatan seumpamanya yang disediakan oleh OS.

Nilai-nilai ini tidak dihantar ke pelayan milik pembangun sendiri dan biasanya akan dipadamkan jika data aplikasi dibersihkan atau aplikasi dinyahpasang.

#### (1) Tetapan lapisan

Contohnya termasuk:

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

- Memulihkan kedudukan lapisan
- Memulihkan gaya sari kata untuk lapisan dan main balik sari kata dalam aplikasi
- Mengekalkan keutamaan garis luar / fon / orientasi
- Mengawal logik kekerapan paparan iklan bagi sesetengah aliran berkaitan lapisan

#### (2) Kedudukan main balik atau lapisan terkini

Contohnya termasuk:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Tujuan:

- Memulihkan atau mencadangkan kedudukan mula sari kata/lapisan terkini
- Menyambung semula main balik video + sari kata dengan lebih mudah

#### (3) Nilai keutamaan iklan dan privasi

Contohnya mungkin termasuk:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Tujuan:

- Menyimpan pilihan privasi iklan
- Menerapkan tetapan privasi dan konfigurasi iklan UMP / AdMob

#### (4) Output sari kata yang dicipta oleh pengguna

Apabila pengguna menyimpan atau mengeksport fail sari kata, aplikasi ini boleh menulis fail sari kata baharu ke lokasi yang dipilih oleh pengguna, seperti:

- Muat turun
- Folder lain yang dipilih melalui pemilih sistem
- Lokasi storan yang diurus oleh pengguna

Fail yang disimpan oleh pengguna ini mungkin kekal pada peranti selepas aplikasi dipadamkan melainkan pengguna memadamkannya secara manual.

#### (5) Fail sementara dan cache

Aplikasi ini dan pustaka pihak ketiga boleh mencipta fail sementara atau fail cache untuk operasi biasa, seperti:

- data cache pemilih fail
- data sementara penukaran sari kata
- data cache berkaitan main balik

Ini hanya bertujuan untuk operasi setempat dan tidak dimuat naik ke pelayan milik pembangun sendiri.

#### (6) Cache status persetujuan UMP

Di rantau yang tertakluk kepada Google UMP, SDK boleh menyimpan cache status persetujuan secara tempatan pada peranti.

Perkara ini secara umum boleh ditetapkan semula dengan:

- membersihkan data aplikasi, atau
- menukar pilihan persetujuan di dalam aplikasi apabila entri pilihan privasi tersedia

### 2-3) Pemprosesan Berkaitan Lapisan Android dan Kebenaran

Pada Android, lapisan sari kata terapung boleh menggunakan:

- kebenaran `SYSTEM_ALERT_WINDOW` / paparan di atas aplikasi lain
- kebenaran `POST_NOTIFICATIONS`
- pemberitahuan perkhidmatan latar hadapan yang diperlukan untuk perkhidmatan lapisan

Tujuan:

- memaparkan lapisan sari kata di atas aplikasi lain
- memastikan perkhidmatan lapisan terus berjalan
- membolehkan Android memaparkan pemberitahuan lapisan / perkhidmatan yang diperlukan
- membaca maklumat pemberitahuan media apabila diperlukan untuk sokongan perkembangan sari kata

Kebenaran ini hanya digunakan untuk ciri aplikasi yang dipilih oleh pengguna untuk digunakan.

### 2-4) Iklan, Persetujuan, dan Data Berkaitan (SDK Pihak Ketiga)

Aplikasi ini menggunakan SDK iklan / persetujuan Google, termasuk:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

Aplikasi ini mungkin memaparkan:

- iklan sepanduk
- iklan interstisial
- iklan ganjaran atau interstisial ganjaran

SDK ini boleh memproses data seperti:

- pengecam pengiklanan (contohnya, AAID / IDFA jika berkenaan)
- maklumat berasaskan IP dan berkaitan rangkaian
- metadata peranti dan aplikasi
- isyarat interaksi iklan
- pilihan persetujuan

Tujuannya mungkin termasuk:

- penyampaian iklan
- pengukuran dan pelaporan iklan
- had kekerapan
- pencegahan penipuan
- pematuhan undang-undang

Pembangun berusaha untuk mengkonfigurasi SDK ini dengan cara yang selaras dengan pilihan persetujuan pengguna dan undang-undang yang terpakai.

---

## 3. Cara Kami Memproses dan Menyimpan Data

- **Tetapan tempatan dan data kedudukan terkini**
  - disimpan pada peranti sehingga data aplikasi dibersihkan atau aplikasi dibuang

- **Fail sementara / cache**
  - disimpan hanya setakat yang diperlukan untuk operasi, kemudian dipadamkan oleh aplikasi apabila praktikal atau dibersihkan kemudian oleh OS

- **Fail sari kata yang disimpan oleh pengguna**
  - kekal di lokasi simpanan yang dipilih oleh pengguna sehingga dipadamkan oleh pengguna

- **Data iklan / persetujuan yang dikendalikan oleh pihak ketiga**
  - disimpan mengikut dasar Google dan undang-undang yang terpakai

---

## 4. Pemprosesan oleh Pihak Ketiga dan Pemindahan Rentas Sempadan

Bagi tujuan iklan dan pengurusan persetujuan, sesetengah maklumat mungkin diproses oleh Google dan rakan kongsi berkaitan.

| Item | Butiran |
|---|---|
| Penerima | Google LLC dan sekutu / pemproses berkaitan |
| Tujuan | Penyampaian iklan, pengukuran, pencegahan penipuan, pengurusan persetujuan, dan pematuhan undang-undang |
| Data yang mungkin diproses | Pengecam pengiklanan, maklumat peranti/aplikasi, maklumat berasaskan IP, data interaksi iklan, status persetujuan |
| Destinasi | Amerika Syarikat dan rantau lain tempat infrastruktur Google beroperasi |
| Penyimpanan | Mengikut dasar Google dan undang-undang yang terpakai |

Pembangun berusaha memastikan pendedahan privasi di gedung aplikasi selaras dengan tingkah laku sebenar SDK.

---

## 5. Hak dan Pilihan Anda

Bergantung pada bidang kuasa anda, anda mungkin mempunyai hak seperti:

- akses
- pembetulan
- pemadaman
- sekatan
- kebolehportan
- bantahan
- penarikan balik persetujuan apabila persetujuan merupakan asas undang-undang

Kawalan praktikal termasuk:

- menukar pilihan iklan / privasi dalam aplikasi apabila tersedia
- membersihkan data aplikasi untuk membuang tetapan tempatan dan keutamaan yang dicache
- menyahpasang aplikasi
- memadam fail sari kata yang dieksport secara manual daripada storan pengguna
- menggunakan kawalan peringkat OS seperti tetapan pemberitahuan, tetapan semula ID iklan, atau tetapan pemperibadian iklan

Bagi data yang diproses oleh Google, pengguna juga hendaklah merujuk kepada alat privasi dan akaun Google sendiri jika berkaitan.

---

## 6. Privasi Kanak-kanak

Aplikasi ini tidak ditujukan terutamanya kepada kanak-kanak.

Tujuan utamanya ialah main balik sari kata, penyuntingan, paparan lapisan, dan ciri utiliti berkaitan. Jika sesuai, konfigurasi SDK iklan boleh menggunakan penanda berkaitan umur atau child-directed flags yang selaras dengan keperluan platform dan tetapan pembangun.

---

## 7. Langkah Keselamatan

Dalam had seni bina aplikasi ini, pembangun berusaha untuk:

- meminimumkan pengumpulan dengan memastikan kebanyakan pemprosesan sari kata dan media kekal pada peranti
- menggunakan pemilih fail sistem dan akses fail yang dimulakan oleh pengguna
- menggunakan kebenaran sistem secara telus
- bergantung pada pengangkutan rangkaian yang disulitkan yang digunakan oleh SDK pihak ketiga, jika berkenaan

Tiada kaedah penyimpanan atau penghantaran yang benar-benar selamat, tetapi aplikasi ini direka untuk mengelakkan pengumpulan yang tidak perlu oleh pembangun.

---

## 8. Perisian Sumber Terbuka

Aplikasi ini menggunakan perisian sumber terbuka, termasuk pustaka yang berkaitan dengan:

- penghuraian dan pensirian sari kata
- pemilihan fail
- keutamaan tempatan
- tetingkap lapisan
- main balik video
- WebView

Notis sumber terbuka tersedia di dalam aplikasi. Bagi sesetengah komponen, aplikasi ini mungkin menggunakan salinan pakej sumber terbuka yang diubah suai secara tempatan sambil mengekalkan notis lesen asal.

---

## 9. Hubungi

Jika anda mempunyai pertanyaan atau permintaan berkaitan privasi:

- **E-mel:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Sila sertakan nama aplikasi **Subtitle Player & Editor** dalam mesej anda.

---

## 10. Perubahan kepada Dasar Ini

Dasar ini boleh dikemas kini jika:

- ciri aplikasi berubah
- kebenaran atau penggunaan SDK berubah
- keperluan undang-undang atau platform berubah

Perubahan material akan dicerminkan pada halaman dasar yang dikemas kini dan, jika sesuai, dalam aplikasi.

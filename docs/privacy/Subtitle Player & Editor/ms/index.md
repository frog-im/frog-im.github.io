---
title: Dasar Privasi | Subtitle Tool
description: Dasar Privasi Subtitle Tool (Bahasa Melayu)
lang: ms
last_updated: 2025-12-12
---

# Dasar Privasi (Subtitle Tool / Subtitle Player & Editor)

- **Nama aplikasi:** Subtitle Tool (mungkin dipaparkan sebagai “Subtitle Player & Editor” di stor)  
- **Pembangun:** frog-im  
- **Emel hubungan:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Tarikh berkuat kuasa:** 2025-12-12  

> Dasar ini dirangka dengan merujuk kepada undang-undang yang berkaitan, termasuk Akta Perlindungan Maklumat Peribadi Korea (PIPA), GDPR / UK GDPR, FADP Switzerland dan beberapa undang-undang privasi negeri di Amerika Syarikat. Jika terdapat keperluan khusus mengikut bidang kuasa, keperluan tersebut akan mengatasi kandungan umum dasar ini.

---

## 1. Tujuan dan skop

Aplikasi ini menyediakan fungsi utama berikut:

- **Edit metadata fail audio** (tajuk, artis dan sebagainya) yang disimpan pada peranti;  
- Menunjukkan **lapisan terapung lirik/sarikata (lyrics overlay)** di atas aplikasi lain.

Aplikasi ini **tidak membuat akaun pengguna** dan **tidak memuat naik kandungan pengguna** ke pelayan milik pembangun.  
Pemprosesan lazimnya dilakukan **secara setempat pada peranti pengguna**.

Walau bagaimanapun, untuk tujuan **pengiklanan** dan **pemenuhan keperluan undang-undang**, aplikasi ini menggunakan SDK pihak ketiga seperti **Google Mobile Ads SDK (AdMob)** dan **Google UMP**, yang mungkin memproses maklumat seperti **pengenal iklan (advertising identifiers)**.

Proses pengumpulan persetujuan dan pilihan privasi mengikuti spesifikasi **Google UMP (User Messaging Platform)**.

---

## 2. Kategori maklumat yang diproses

### 2-1) Fail yang dipilih secara jelas oleh pengguna

- **Laluan dan kandungan audio/imej kulit album:**  
  Digunakan hanya di peranti untuk tujuan membaca, menyunting metadata dan menyimpan semula.  
- **FFmpegKit** digunakan secara setempat untuk pengekodan, penyuntingan metadata dan pengekstrakan thumbnail.  
- Aplikasi ini **tidak memuat naik fail-fail ini** ke pelayan pembangun.

### 2-2) Tetapan tempatan dan nilai yang disimpan

Bagi memastikan fungsi teras dan kemudahan pengguna, aplikasi menyimpan nilai berikut **secara tempatan pada peranti**.  
Nilai ini **tidak dihantar** ke pelayan pembangun dan akan **dipadam apabila aplikasi atau data aplikasinya dipadamkan**.

#### (1) Keutamaan (`shared_preferences`)

| Jenis | Kekunci / kandungan | Tujuan | Lokasi simpanan | Pemadaman |
|---|---|---|---|---|
| Kedudukan & saiz fon lapisan | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Mengembalikan kedudukan dan saiz tulisan lapisan lirik | SharedPreferences peranti | Dipadam apabila data aplikasi atau aplikasi dipadamkan |
| Tetapan iklan / privasi | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Menetapkan iklan bukan diperibadikan, tetapan RDP (AS), penandaan kandungan kanak-kanak, umur, dan had rating kandungan iklan | SharedPreferences peranti | Sama seperti di atas |

#### (2) Fail sementara (direktori sementara sistem)

- **Contoh:** `cover_*.jpg`, `tmp_*.flac`  
- **Kegunaan:** pengekstrakan kulit album, penulisan tag FLAC, dan fail pengekodan sementara  
- **Lokasi:** folder sementara sistem (`systemTemp`)  
- **Tempoh simpanan:** aplikasi cuba memadam selepas selesai digunakan; selebihnya mungkin kekal buat sementara dalam cache sistem sehingga dibersihkan oleh OS

#### (3) Lokasi simpanan yang dipilih pengguna (SAF)

- Apabila pengguna memilih “Simpan sebagai” dan seumpamanya, fail audio akhir boleh ditulis ke lokasi yang ditetapkan pengguna (contohnya folder Muat Turun atau storan awan).  
- Fail-fail ini disimpan di **storan luaran** dan **tidak akan dipadam secara automatik** apabila aplikasi dinyahpasang. Pengguna boleh memadamnya secara manual.

#### (4) Status persetujuan (cache SDK UMP)

- Di rantau EEA / UK / Switzerland, SDK UMP akan **menyimpan status persetujuan iklan pengguna secara tempatan**.  
- Pengguna boleh menetapkan semula status ini dengan memadam data aplikasi atau melalui skrin **Pilihan Privasi (Privacy Options)** dalam aplikasi (jika disediakan).

---

### 2-3) Data berkaitan iklan dan persetujuan (SDK pihak ketiga)

**Google Mobile Ads SDK (AdMob)** dan **Google UMP** mungkin mengumpul / memproses:

- Pengenal iklan (AAID / IDFA);  
- Maklumat alamat IP atau julat IP;  
- Maklumat peranti dan aplikasi;  
- Isyarat interaksi iklan (paparan, klik, dan lain-lain);  
- Status persetujuan dan tetapan yang berkaitan.

**Tujuan pemprosesan:**

- Penyampaian dan pengurusan iklan;  
- Had kekerapan paparan;  
- Pencegahan penipuan atau penyalahgunaan;  
- Pengukuran prestasi dan analisis;  
- Pemenuhan keperluan undang-undang berkaitan privasi dan persetujuan.

**Rantau yang memerlukan persetujuan (EEA / UK / Switzerland):**

- Persetujuan dikumpulkan melalui dialog UMP.  
- Skrin **Pilihan Privasi (Privacy Options)** disediakan untuk membolehkan pengguna mengubah pilihan kemudian.

**Rantau lain (contohnya Korea Selatan):**

- Skrin ini mungkin **tidak dipaparkan**, jika tidak dikehendaki oleh undang-undang.

---

## 3. Cara pemprosesan dan tempoh penyimpanan

- **Tetapan tempatan:**  
  Disimpan pada peranti sehingga pengguna memadam data aplikasi atau menyahpasang aplikasi.  
- **Fail sementara:**  
  Dihasilkan semasa proses pengekodan/pengekstrakan; dipadam sebaik sahaja selesai jika boleh, namun sebahagian mungkin kekal sementara dalam cache sistem.  
- **Data iklan/persetujuan (pihak ketiga):**  
  Disimpan dan diproses oleh pihak ketiga (contohnya Google) mengikut dasar privasi mereka sendiri.

---

## 4. Pemindahan kepada pihak ketiga & aliran data rentas sempadan

Untuk tujuan pengiklanan dan pengurusan persetujuan, sesetengah maklumat mungkin dihantar dan diproses dalam infrastruktur Google, termasuk di luar negara asal pengguna.

| Item | Butiran |
|---|---|
| **Penerima** | Google LLC dan syarikat gabungan / pemproses subkontrak |
| **Destinasi data** | Amerika Syarikat dan kawasan lain yang mempunyai pusat data Google |
| **Tujuan** | Penyampaian iklan, pengukuran prestasi, pencegahan penipuan, pematuhan undang-undang, pengurusan rekod persetujuan |
| **Jenis data** | Pengenal iklan, maklumat IP, data peranti dan aplikasi, isyarat interaksi iklan, status persetujuan, dan lain-lain |
| **Tempoh simpanan** | Mengikut dasar dalaman Google |
| **Kesan penolakan** | Iklan diperibadikan mungkin terhad; iklan tidak diperibadikan mungkin masih dipaparkan |

Kami mematuhi keperluan pendedahan **“Data safety” Google Play** dan berusaha memastikan maklumat yang dipaparkan sepadan dengan pemprosesan sebenar dalam aplikasi.

---

## 5. Hak anda dan cara menggunakannya

- **Menolak iklan diperibadikan / mengubah persetujuan**  
  - Di EEA / UK / Switzerland: gunakan menu **Tetapan → Pilihan Privasi** dalam aplikasi.  
  - Di rantau lain: gunakan tetapan sistem operasi untuk menetapkan semula ID iklan, menghadkan penjejakan, atau mematikan iklan diperibadikan.  

- **Menetapkan semula maklumat tempatan**  
  - Memadam data aplikasi atau menyahpasang aplikasi akan membersihkan kedudukan lapisan, saiz fon dan tetapan tempatan lain.

Selaras dengan **GDPR / UK GDPR / FADP Switzerland / undang-undang privasi beberapa negeri di AS**, anda mungkin mempunyai hak untuk mengakses, membetulkan, memadam, mengehadkan pemprosesan, mendapatkan salinan data (portabiliti), dan menarik balik persetujuan.  
Bagi data iklan yang diproses oleh Google, sila gunakan **mekanisme rasmi Google**.

---

## 6. Privasi kanak-kanak

Aplikasi ini **tidak ditujukan khas kepada kanak-kanak**.  
Jika kanak-kanak di bawah umur minimum undang-undang menggunakan aplikasi, dia disarankan untuk berhenti menggunakan aplikasi dan, bersama penjaga, mengaktifkan ciri had iklan pada tahap sistem operasi.  
Jika sesuai, kami mungkin menggunakan tetapan seperti **TFUA (penandaan kandungan kanak-kanak)** atau mekanisme perlindungan kanak-kanak lain.

---

## 7. Langkah-langkah keselamatan

Kami berusaha untuk:

- Mengamalkan prinsip **minimisasi data** dalam pengumpulan dan storan;  
- Mengehadkan penggunaan fail sementara dan memadamnya selepas digunakan;  
- Mengehadkan pemprosesan kepada skop keizinan yang diberikan oleh sistem operasi;  
- Menggunakan **penyulitan (contohnya TLS)** untuk penghantaran data kepada pihak ketiga (mengikut pelaksanaan SDK berkenaan).

---

## 8. Data Safety di Google Play

Kami menyediakan dan menyelenggara bahagian **“Data safety”** dalam Play Console dengan tepat dan akan mengemas kininya apabila amalan pemprosesan data kami berubah.

---

## 9. Notis sumber terbuka

Aplikasi ini menggunakan perisian sumber terbuka seperti **FFmpeg**.  
Fail maklumat (contohnya `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) di dalam aplikasi menerangkan cara mendapatkan kod sumber.  
Atas permintaan, kami akan menyediakan kod sumber seperti yang diterangkan dalam fail tersebut.

---

## 10. Maklumat hubungan

- Emel: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Perubahan kepada Dasar ini

Kami mungkin menyemak Dasar ini dari semasa ke semasa kerana perubahan undang-undang atau perubahan fungsi perkhidmatan.  
Sebarang kemas kini akan diumumkan **di dalam aplikasi** dan pada halaman dasar ini.  
Bagi perubahan yang besar, kami akan memberikan notis **sekurang-kurangnya 7 hari sebelum** tarikh kuat kuasa.

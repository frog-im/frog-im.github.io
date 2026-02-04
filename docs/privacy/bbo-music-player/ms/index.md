---
title: Dasar Privasi | LyriFloat
description: Dasar Privasi LyriFloat (Bahasa Melayu)
lang: ms
last_updated: 2025-10-30
---

# Dasar Privasi (LyriFloat)

- **Nama aplikasi:** LyriFloat  
- **Pembangun:** frog-im  
- **Hubungi:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tarikh berkuat kuasa:** 2025-10-30

> Dasar ini digubal dengan merujuk kepada undang-undang yang terpakai termasuk Akta Perlindungan Maklumat Peribadi Korea (PIPA), GDPR/UK GDPR, FADP Switzerland, serta undang-undang privasi negeri berkaitan di A.S. Jika terdapat keperluan khusus bidang kuasa, keperluan tersebut diutamakan.

---

## 1. Tujuan dan Skop

Aplikasi ini menyediakan **penyuntingan metadata fail audio** (tajuk, artis, dll.) yang disimpan pada peranti dan ciri **paparan lirik secara overlay**.  
Aplikasi ini **tidak** mencipta akaun pengguna dan **tidak** memuat naik kandungan pengguna ke mana-mana pelayan. Pemprosesan dilakukan **pada peranti pengguna** secara lalai.

Walau bagaimanapun, untuk tujuan **pengiklanan** dan **pematuhan undang-undang**, rakan pihak ketiga (cth., Google Mobile Ads SDK (AdMob), UMP) mungkin mengumpul dan memproses maklumat seperti **pengenal iklan**. Pengumpulan persetujuan dan pilihan privasi mengikuti spesifikasi **Google UMP (User Messaging Platform)**.

---

## 2. Kategori Maklumat yang Kami Proses

### 2-1) Fail yang Dipilih Secara Jelas oleh Pengguna
- **Laluan dan kandungan audio/imej kulit (cover):** diproses **secara setempat** pada peranti hanya untuk tujuan edit/simpan.  
- **FFmpegKit** digunakan secara setempat untuk pengekodan, penyuntingan metadata, dan pengekstrakan thumbnail.  
- Aplikasi ini **tidak memuat naik** fail yang dipilih pengguna ke pelayan kami.

### 2-2) Tetapan Tempatan dan Nilai Disimpan

Untuk fungsi teras dan kemudahan pengguna, aplikasi menyimpan nilai berikut **secara tempatan pada peranti**.  
Nilai ini tidak dihantar ke pelayan kami dan akan **dipadam apabila aplikasi atau datanya dipadam**.

#### (1) Keutamaan (`shared_preferences`)
| Jenis | Kunci/Kandungan | Tujuan | Storan | Pemadaman |
|---|---|---|---|---|
| Kedudukan/font overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Pulihkan kedudukan overlay dan saiz font | SharedPreferences peranti | Dipadam apabila data aplikasi atau aplikasi dipadam |
| Tetapan Iklan/Privasi | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Iklan tidak diperibadikan, RDP A.S., tag COPPA, tag umur, had penarafan kandungan iklan | SharedPreferences peranti | Sama seperti di kiri |

#### (2) Fail Sementara (direktori temp sistem)
- **Contoh:** `cover_*.jpg`, `tmp_*.flac`  
- **Kegunaan:** pengekstrakan cover art, tag FLAC, pengekodan sementara  
- **Lokasi:** folder sementara OS (`systemTemp`)  
- **Tempoh simpanan:** dipadam oleh aplikasi selepas siap apabila boleh; juga tertakluk kepada pembersihan OS

#### (3) Simpanan Dipilih Pengguna (SAF)
- Apabila pengguna memilih “Save As,” fail audio akhir mungkin ditulis ke lokasi yang ditetapkan pengguna (cth., Muat Turun, storan awan).  
- Fail ini berada dalam **storan luaran** dan **kekal selepas aplikasi dipadam**. Pengguna boleh memadamnya secara manual.

#### (4) Keadaan Persetujuan (Cache SDK UMP)
- Di wilayah EEA/UK/CH, SDK UMP **menyimpan cache keadaan persetujuan iklan pengguna secara tempatan**.  
- Ia boleh ditetapkan semula dengan memadam data aplikasi atau melalui skrin **Privacy Options** dalam aplikasi apabila tersedia.

---

### 2-3) Data Berkaitan Iklan dan Persetujuan (SDK pihak ketiga)
- **Google Mobile Ads SDK (AdMob) dan UMP** boleh mengumpul/memproses, contohnya: **pengenal iklan (AAID/IDFA)**, **julat IP**, **maklumat peranti/aplikasi**, **isyarat interaksi iklan**, **keadaan persetujuan**, dll.  
- **Tujuan:** penyampaian iklan, had kekerapan, pencegahan penipuan, pengukuran prestasi, pematuhan undang-undang  
- **Wilayah memerlukan persetujuan (EEA/UK/CH):** persetujuan dikumpul melalui prompt UMP, dan skrin **Privacy Options** disediakan apabila diperlukan.  
  Di wilayah tanpa keperluan sedemikian (cth., KR), pilihan ini **mungkin tidak dipaparkan**.

---

## 3. Pemprosesan dan Tempoh Simpanan

- **Tetapan tempatan:** disimpan pada peranti sehingga pengguna memadam data aplikasi atau menyahpasang aplikasi  
- **Fail sementara:** dicipta semasa pengekodan/pengekstrakan, dipadam selepas pemprosesan atau mungkin kekal sementara dalam cache OS  
- **Data iklan/persetujuan (pihak ketiga):** disimpan dan dilupuskan mengikut **dasar Google**

---

## 4. Pemindahan Pihak Ketiga dan Aliran Data Rentas Sempadan

Untuk pengiklanan dan pengurusan persetujuan, maklumat pengguna mungkin dihantar dan diproses pada infrastruktur Google.

| Item | Butiran |
|---|---|
| **Penerima** | Google LLC dan sekutu/sub-pemprosesnya |
| **Destinasi** | Amerika Syarikat (dan wilayah lain tempat infrastruktur Google berada) |
| **Tujuan** | Penyampaian iklan, prestasi/pengukuran, pematuhan undang-undang, pengurusan persetujuan |
| **Data** | Pengenal iklan, julat IP, maklumat peranti/aplikasi, interaksi iklan, keadaan persetujuan, dll. |
| **Tempoh simpanan** | Mengikut dasar Google |
| **Kesan penolakan** | Iklan diperibadikan mungkin dihadkan; iklan tidak diperibadikan mungkin dipaparkan |

Kami mematuhi keperluan pendedahan **Google Play Data safety** dan memastikan pendedahan selaras dengan pemprosesan sebenar.

---

## 5. Hak Anda dan Cara Melaksanakannya

- **Nyah ikut iklan diperibadikan / ubah persetujuan**  
  - Di wilayah disokong (EEA/UK/CH): ubah pilihan di **Settings → Privacy Options**.  
  - Wilayah lain: gunakan tetapan OS untuk **reset ad IDs / hadkan penjejakan iklan**.
- **Set semula maklumat tempatan:** memadam data aplikasi atau menyahpasang aplikasi akan menetapkan semula koordinat overlay, saiz font, dan tetapan tempatan lain.
- Hak di bawah **GDPR/UK GDPR/FADP Switzerland/undang-undang privasi negeri A.S.** (akses, pembetulan, pemadaman, keboleh-alihan, sekatan, tarik balik persetujuan, dll.) boleh dilaksanakan seperti yang diperuntukkan oleh undang-undang tersebut.  
  Untuk data berkaitan iklan yang diproses oleh Google, sila gunakan **proses Google**.

---

## 6. Privasi Kanak-kanak

Aplikasi ini **bukan untuk kanak-kanak**. Jika kanak-kanak di bawah umur minimum undang-undang menggunakan aplikasi ini, mereka patut berhenti dan menggunakan ciri had-iklan peringkat OS dengan penjaga. Apabila sesuai, kami boleh menggunakan **TFUA (tag perkhidmatan berorientasikan kanak-kanak)** atau pilihan perlindungan kanak-kanak yang serupa.

---

## 7. Langkah Keselamatan

- **Meminimumkan data** dalam pengumpulan dan storan  
- **Penggunaan terhad** fail sementara dan cubaan pemadaman selepas pemprosesan  
- Pemprosesan ketat **dalam skop kebenaran OS**  
- Penyulitan **TLS atau setara** semasa pemindahan untuk pemindahan pihak ketiga (mengikut piawaian SDK pihak ketiga)

---

## 8. Data Safety (Google Play)

Kami menyediakan dan menyelenggara seksyen **Data safety** di Play Console dengan tepat, dan mengemas kininya dengan segera apabila terdapat perubahan.

---

## 9. Notis Sumber Terbuka

Aplikasi ini menggunakan perisian sumber terbuka seperti **FFmpeg**. Fail maklumat (cth., `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) dalam aplikasi menerangkan cara mendapatkan kod sumber. Atas permintaan, kami akan menyediakan sumber seperti yang dinyatakan dalam fail tersebut.

---

## 10. Hubungi

- E-mel: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Perubahan kepada Dasar Ini

Kami boleh menyemak semula Dasar ini disebabkan perubahan undang-undang atau perkhidmatan. Kami akan menyiarkan kemas kini **dalam aplikasi** dan pada **halaman dasar** ini.  
Untuk perubahan material, kami akan memberi notis sekurang-kurangnya **7 hari** sebelum tarikh berkuat kuasa.

---

## Lampiran: Panduan Pengguna

- **Pautan dalam aplikasi:** buka halaman ini melalui **Settings → Privacy**.  
- **Tingkah laku mengikut wilayah:** di EEA/UK/CH, Privacy Options dipaparkan. **Di KR dan beberapa wilayah lain, butang mungkin tidak memaparkan pilihan tambahan** jika tidak diwajibkan oleh undang-undang.

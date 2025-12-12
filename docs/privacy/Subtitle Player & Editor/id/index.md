---
title: Kebijakan Privasi | Subtitle Tool
description: Kebijakan privasi untuk Subtitle Player & Editor (Subtitle Tool)
lang: id
last_updated: 2025-12-12
---

# Kebijakan Privasi (Subtitle Player & Editor / “Subtitle Tool”)

- **Nama aplikasi:** Subtitle Player & Editor (selanjutnya disebut “Subtitle Tool”)  
- **Pengembang:** frog-im  
- **Kontak:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Tanggal berlaku:** 2025-12-12  

> Kebijakan ini disusun dengan mengacu pada hukum yang berlaku, termasuk Undang-Undang Perlindungan Informasi Pribadi Korea (PIPA), GDPR/UK GDPR, hukum perlindungan data Swiss (FADP), serta berbagai undang-undang privasi negara bagian di AS.  
> Jika terdapat ketentuan khusus di yurisdiksi tertentu, ketentuan tersebut akan mengesampingkan bagian yang bertentangan dalam Kebijakan ini.

---

## 1. Tujuan dan Ruang Lingkup

Aplikasi ini menyediakan fungsi **pengeditan metadata file audio** (judul, artis, dll.) yang disimpan di perangkat, dan fungsi **overlay lirik/subtitel**.  
Aplikasi **tidak membuat akun pengguna** dan **tidak mengunggah konten pengguna** ke server kami. Pemrosesan secara default dilakukan **secara lokal di perangkat**.

Namun, untuk keperluan **periklanan** dan **kepatuhan hukum**, mitra pihak ketiga (misalnya Google Mobile Ads SDK (AdMob) dan UMP) dapat mengumpulkan dan memproses informasi seperti **pengidentifikasi iklan**.  
Pengumpulan persetujuan dan pengaturan preferensi privasi mengikuti spesifikasi **Google UMP (User Messaging Platform)**.

---

## 2. Kategori Informasi yang Kami Proses

### 2-1) File yang Dipilih Secara Eksplisit oleh Pengguna

- **Path dan konten audio/gambar sampul:** diproses **secara lokal** di perangkat hanya untuk keperluan pengeditan dan penyimpanan.  
- **FFmpegKit** digunakan secara lokal untuk encoding, pengeditan metadata, dan ekstraksi thumbnail.  
- Aplikasi **tidak mengunggah** file yang dipilih pengguna ini ke server kami.

### 2-2) Pengaturan Lokal dan Nilai yang Disimpan

Untuk fungsi inti dan kenyamanan pengguna, aplikasi menyimpan nilai-nilai berikut **secara lokal di perangkat**.  
Nilai ini tidak dikirim ke server kami dan akan **dihapus ketika data aplikasi atau aplikasinya dihapus**.

#### (1) Preferensi (`shared_preferences`)

| Jenis | Kunci/Konten | Tujuan | Penyimpanan | Penghapusan |
|---|---|---|---|---|
| Posisi/font overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Mengembalikan posisi overlay dan ukuran font | SharedPreferences di perangkat | Dihapus ketika data aplikasi atau aplikasi dihapus |
| Pengaturan iklan/privasi | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Iklan non-personalisasi, sinyal U.S. RDP, tag COPPA (konten anak), tag usia, batas rating konten iklan | SharedPreferences di perangkat | Sama seperti kolom kiri |

#### (2) File Sementara (folder sementara sistem)

- **Contoh:** `cover_*.jpg`, `tmp_*.flac`  
- **Penggunaan:** ekstraksi sampul, tagging FLAC, encoding sementara  
- **Lokasi:** folder sementara sistem operasi (`systemTemp`)  
- **Masa simpan:** diupayakan dihapus setelah pemrosesan selesai, dan juga dapat dibersihkan oleh mekanisme pembersihan OS.

#### (3) Jalur Penyimpanan yang Dipilih Pengguna (SAF)

- Saat pengguna memilih “Save As”, file audio final dapat ditulis ke lokasi yang dipilih pengguna (misalnya folder Download, penyimpanan cloud).  
- File ini berada di **penyimpanan eksternal** dan **dapat tetap ada setelah aplikasi dihapus**. Pengguna dapat menghapusnya secara manual.

#### (4) Status Persetujuan (cache UMP)

- Di wilayah EEA/UK/Swiss, SDK UMP **menyimpan status persetujuan iklan pengguna secara lokal**.  
- Status ini dapat di-reset dengan menghapus data aplikasi atau melalui layar **Opsi Privasi** di dalam aplikasi (jika tersedia).

---

### 2-3) Data Terkait Iklan dan Persetujuan (SDK Pihak Ketiga)

- **Google Mobile Ads SDK (AdMob) dan UMP** dapat mengumpulkan dan memproses, misalnya: **pengidentifikasi iklan (AAID/IDFA)**, **rentang IP**, **informasi perangkat/aplikasi**, **sinyal interaksi iklan**, **status persetujuan**, dan sebagainya.  
- **Tujuan:** penayangan iklan, pembatasan frekuensi, pencegahan penipuan, pengukuran kinerja, kepatuhan hukum.  
- **Wilayah yang mensyaratkan persetujuan (EEA/UK/Swiss):** persetujuan dikumpulkan melalui dialog UMP dan layar **Opsi Privasi** disediakan bila disyaratkan.  
  Di wilayah yang tidak memiliki persyaratan tersebut (misalnya Korea), opsi ini **mungkin tidak ditampilkan**.

---

## 3. Pemrosesan dan Retensi

- **Pengaturan lokal:** disimpan di perangkat hingga pengguna menghapus data aplikasi atau menghapus aplikasinya.  
- **File sementara:** dibuat saat encoding/ekstraksi, dihapus setelah pemrosesan atau dapat sementara tersimpan sebagai cache sistem.  
- **Data iklan/persetujuan (pihak ketiga):** disimpan dan dihapus sesuai **kebijakan Google**.

---

## 4. Transfer ke Pihak Ketiga dan Aliran Data Lintas Batas

Untuk periklanan dan pengelolaan persetujuan, sebagian informasi pengguna dapat dikirim dan diproses pada infrastruktur Google.

| Item | Rincian |
|---|---|
| **Penerima** | Google LLC dan afiliasi/sub-prosesornya |
| **Tujuan transfer** | Amerika Serikat (dan wilayah lain tempat infrastruktur Google berada) |
| **Tujuan penggunaan** | Penayangan iklan, pengukuran dan performa, kepatuhan hukum, manajemen persetujuan |
| **Data** | Pengidentifikasi iklan, rentang IP, info perangkat/aplikasi, interaksi iklan, status persetujuan, dll. |
| **Masa simpan** | Sesuai kebijakan Google |
| **Dampak penolakan** | Iklan yang dipersonalisasi dapat dibatasi; iklan non-personalisasi mungkin tetap ditampilkan |

Kami mematuhi persyaratan pengungkapan **Data safety** di Google Play dan menjaga agar pengungkapan tersebut selaras dengan pemrosesan yang sebenarnya.

---

## 5. Hak Anda dan Cara Menggunakannya

- **Menonaktifkan iklan personalisasi / mengubah persetujuan**  
  - Di wilayah yang didukung (EEA/UK/Swiss): ubah preferensi Anda melalui **Pengaturan → Opsi Privasi**.  
  - Di wilayah lain: gunakan pengaturan sistem operasi untuk **mereset ID iklan / membatasi pelacakan iklan**.
- **Mereset informasi lokal:** penghapusan data aplikasi atau penghapusan aplikasi akan mereset koordinat overlay, ukuran font, dan pengaturan lokal lainnya.  
- Berdasarkan **GDPR/UK GDPR/FADP Swiss/undang-undang privasi negara bagian di AS**, Anda mungkin memiliki hak atas akses, koreksi, penghapusan, portabilitas data, pembatasan pemrosesan, penarikan persetujuan, dan lain-lain (sejauh diatur dalam hukum yang berlaku).  
  Untuk data iklan yang diproses oleh Google, gunakan **mekanisme yang disediakan oleh Google**.

---

## 6. Privasi Anak

Aplikasi ini **tidak ditujukan untuk anak-anak**.  
Jika seorang anak di bawah usia minimum hukum menggunakan aplikasi ini, ia disarankan untuk berhenti menggunakannya dan, bersama wali, menggunakan pengaturan pembatasan iklan pada sistem operasi.  
Jika relevan, kami dapat menerapkan label seperti **TFUA (child-directed tag)** atau opsi perlindungan anak lainnya.

---

## 7. Langkah-langkah Keamanan

- **Minimisasi data** dalam pengumpulan dan penyimpanan  
- Penggunaan file sementara secara terbatas dan penghapusan setelah pemrosesan bila memungkinkan  
- Pemrosesan hanya dilakukan **dalam lingkup izin sistem operasi**  
- Enkripsi **TLS atau yang setara** saat mentransmisikan data ke pihak ketiga (sesuai standar SDK terkait)

---

## 8. Keamanan Data (Google Play)

Kami menyiapkan dan memelihara bagian **Data safety** dalam Google Play Console secara akurat dan memperbaruinya segera ketika terjadi perubahan dalam pemrosesan.

---

## 9. Pemberitahuan Perangkat Lunak Sumber Terbuka

Aplikasi ini menggunakan perangkat lunak sumber terbuka seperti **FFmpeg**.  
Di dalam aplikasi terdapat berkas informasi (misalnya `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) yang menjelaskan cara memperoleh kode sumber.  
Atas permintaan, kami akan menyediakan kode sumber sesuai petunjuk dalam berkas tersebut.

---

## 10. Kontak

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Perubahan atas Kebijakan Ini

Kami dapat merevisi Kebijakan ini karena perubahan hukum atau perubahan layanan.  
Pembaruan akan diumumkan **di dalam aplikasi** dan pada **halaman kebijakan** ini.  
Untuk perubahan yang bersifat material, kami akan memberikan pemberitahuan **setidaknya 7 hari sebelum** tanggal mulai berlakunya.

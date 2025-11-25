---
title: Kebijakan Privasi | LyriFloat
description: Kebijakan Privasi LyriFloat (Bahasa Indonesia)
lang: id
last_updated: 2025-10-30
---

# Kebijakan Privasi (LyriFloat)

- **Nama aplikasi:** LyriFloat
- **Pengembang:** frog-im  
- **Kontak:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tanggal berlaku:** 2025-10-30

> Kebijakan ini disusun dengan merujuk pada hukum yang berlaku, termasuk Undang-Undang Perlindungan Informasi Pribadi Korea (PIPA), GDPR/UK GDPR, FADP Swiss, dan undang-undang privasi negara bagian di AS. Jika terdapat persyaratan khusus yurisdiksi, persyaratan tersebut berlaku terlebih dahulu.

---

## 1. Tujuan dan Ruang Lingkup Pemrosesan

Aplikasi ini menyediakan fitur **pengeditan metadata** (judul, artis, dll.) untuk file audio yang **disimpan di perangkat**, serta **overlay lirik**.  
Aplikasi **tidak** membuat akun pengguna dan **tidak** mengunggah konten pengguna ke server kami. Pemrosesan secara bawaan dilakukan **di perangkat pengguna**.

Namun, untuk **periklanan** dan **kepatuhan hukum**, mitra pihak ketiga (mis. Google Mobile Ads SDK (AdMob), UMP) dapat mengumpulkan dan memproses informasi seperti **pengidentifikasi iklan**. Pengumpulan persetujuan dan pilihan privasi mengikuti spesifikasi **Google UMP (User Messaging Platform)**.

---

## 2. Kategori Informasi yang Diproses

### 2-1) File yang Dipilih Secara Eksplisit oleh Pengguna
- **Path dan konten audio/gambar sampul:** diproses **secara lokal** di perangkat hanya untuk tujuan pengeditan/penyimpanan.  
- **FFmpegKit** digunakan secara lokal untuk encoding, pengeditan metadata, dan ekstraksi thumbnail.  
- Aplikasi **tidak mengunggah** file yang dipilih pengguna ke server kami.

### 2-2) Pengaturan Lokal dan Nilai yang Disimpan

Untuk fungsi inti dan kenyamanan, aplikasi menyimpan nilai berikut **secara lokal di perangkat**.  
Nilai ini tidak dikirim ke server kami dan **akan dihapus saat data aplikasi dihapus atau aplikasi dicopot**.

#### (1) Preferensi (`shared_preferences`)
| Jenis | Kunci/Konten | Tujuan | Lokasi Penyimpanan | Penghapusan |
|---|---|---|---|---|
| Posisi/font overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Memulihkan posisi overlay dan ukuran font | SharedPreferences di perangkat | Terhapus saat data aplikasi dihapus atau aplikasi dicopot |
| Iklan/Privasi | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Iklan non-personalisasi, US RDP, tag COPPA, tag usia, batas rating konten iklan | SharedPreferences di perangkat | Sama seperti kiri |

#### (2) File Sementara (direktori sementara sistem)
- **Contoh:** `cover_*.jpg`, `tmp_*.flac`  
- **Penggunaan:** ekstraksi cover art, tagging FLAC, encoding sementara  
- **Lokasi:** folder sementara OS (`systemTemp`)  
- **Retensi:** dihapus setelah proses selesai jika memungkinkan; OS juga dapat membersihkan secara berkala

#### (3) Penyimpanan yang Dipilih Pengguna (SAF)
- Dengan “Simpan sebagai,” file akhir dapat ditulis ke lokasi yang dipilih pengguna (mis. Unduhan, cloud).  
- File ini berada di **penyimpanan eksternal** dan **tetap ada setelah aplikasi dicopot**. Pengguna dapat menghapusnya secara manual.

#### (4) Status Persetujuan (cache SDK UMP)
- Di wilayah EEA/UK/CH, SDK UMP **menyimpan cache** status persetujuan iklan secara lokal.  
- Dapat di-reset dengan menghapus data aplikasi atau melalui layar **Opsi Privasi (Privacy Options)** di dalam aplikasi bila tersedia.

---

### 2-3) Data Iklan dan Persetujuan (SDK Pihak Ketiga)
- **Google Mobile Ads SDK (AdMob) dan UMP** dapat mengumpulkan/memproses, misalnya: **pengidentifikasi iklan (AAID/IDFA)**, **rentang IP**, **info perangkat/aplikasi**, **sinyal interaksi iklan**, **status persetujuan**, dll.  
- **Tujuan:** penayangan iklan, pembatasan frekuensi, pencegahan penipuan, pengukuran kinerja, kepatuhan hukum  
- **Wilayah yang memerlukan persetujuan (EEA/UK/CH):** persetujuan dikumpulkan melalui UMP dan layar **Opsi Privasi** ditampilkan bila diwajibkan.  
  Di wilayah tanpa kewajiban tersebut (mis. KR), **opsi ini mungkin tidak ditampilkan**.

---

## 3. Pemrosesan dan Jangka Waktu Penyimpanan

- **Pengaturan lokal:** disimpan di perangkat hingga pengguna menghapus data aplikasi atau mencopot aplikasi  
- **File sementara:** dibuat selama proses encoding/ekstraksi; dihapus setelah selesai atau dapat sementara tersisa di cache OS  
- **Data iklan/persetujuan (pihak ketiga):** sesuai **kebijakan Google**

---

## 4. Penerusan ke Pihak Ketiga dan Transfer Lintas Batas

Untuk periklanan dan manajemen persetujuan, informasi pengguna dapat dikirim ke dan diproses pada infrastruktur Google.

| Item | Detail |
|---|---|
| **Penerima** | Google LLC dan afiliasi/sub-pemrosesnya |
| **Tujuan transfer** | Amerika Serikat (dan wilayah lain tempat infrastruktur Google berada) |
| **Tujuan penggunaan** | Penayangan iklan, kinerja/pengukuran, kepatuhan hukum, manajemen persetujuan |
| **Data** | Pengidentifikasi iklan, rentang IP, info perangkat/aplikasi, interaksi iklan, status persetujuan, dll. |
| **Retensi** | Sesuai kebijakan Google |
| **Dampak penolakan** | Personalisasi terbatas; iklan non-personalisasi dapat ditampilkan |

Kami mematuhi persyaratan pengungkapan **“Keamanan data” Google Play** dan menjaga kesesuaian pengungkapan dengan praktik pemrosesan aktual.

---

## 5. Hak Anda dan Cara Menggunakannya

- **Menonaktifkan iklan personalisasi / mengubah persetujuan**  
  - Di wilayah yang didukung (EEA/UK/CH): ubah preferensi di **Pengaturan → Opsi Privasi**.  
  - Wilayah lain: gunakan pengaturan OS untuk **mereset ID iklan / membatasi pelacakan**.
- **Reset informasi lokal:** menghapus data aplikasi atau mencopot aplikasi akan mereset koordinat overlay, ukuran font, dan pengaturan lokal lainnya.
- Hak berdasarkan **GDPR/UK GDPR/FADP Swiss/undang-undang privasi negara bagian AS** (akses, perbaikan, penghapusan, portabilitas, pembatasan, penarikan persetujuan, dll.) dapat dijalankan sesuai prosedur yang berlaku.  
  Untuk data iklan yang diproses Google, gunakan **prosedur Google**.

---

## 6. Privasi Anak

Aplikasi ini **tidak ditujukan untuk anak-anak**. Anak di bawah usia minimum hukum harus berhenti menggunakan aplikasi dan, bersama wali, menggunakan fitur pembatasan iklan di tingkat OS. Bila perlu, kami dapat menerapkan **TFUA (child-directed tag)** atau opsi perlindungan anak sejenis.

---

## 7. Langkah Keamanan

- **Minimasi data** dalam pengumpulan dan penyimpanan  
- **Penggunaan terbatas** file sementara dan upaya penghapusan setelah pemrosesan  
- Pemrosesan **dalam cakupan izin OS**  
- **Enkripsi saat transit** (TLS atau setara) untuk transfer pihak ketiga sesuai standar SDK

---

## 8. Keamanan Data (Google Play)

Kami menyiapkan dan memelihara bagian **“Keamanan data”** di Play Console secara akurat, serta memperbaruinya segera ketika terdapat perubahan.

---

## 9. Pemberitahuan Open-Source

Aplikasi menggunakan perangkat lunak open-source seperti **FFmpeg**. Berkas informasi (mis. `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) di dalam aplikasi menjelaskan cara memperoleh kode sumber. Atas permintaan, kami akan menyediakan sumber sesuai petunjuk pada berkas tersebut.

---

## 10. Kontak

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Perubahan Kebijakan Ini

Kami dapat merevisi Kebijakan ini karena perubahan hukum atau layanan. Pembaruan akan dipublikasikan **di dalam aplikasi** dan pada **halaman kebijakan** ini.  
Untuk perubahan material, pemberitahuan akan diberikan **setidaknya 7 hari sebelum** tanggal berlaku.

---

## Lampiran: Panduan Pengguna

- **Tautan dalam aplikasi:** buka halaman ini dari **Pengaturan → Privasi**.  
- **Perilaku regional:** di EEA/UK/CH, Opsi Privasi ditampilkan. **Di KR dan beberapa wilayah lain, tombol mungkin tidak menampilkan opsi tambahan** bila tidak diwajibkan secara hukum.




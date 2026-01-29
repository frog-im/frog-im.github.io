---
title: Kebijakan Privasi | Power lucky lotto
description: Kebijakan Privasi Power lucky lotto (Bahasa Indonesia)
lang: id
last_updated: 2026-01-29
---

# Kebijakan Privasi (Power lucky lotto)

- **Nama aplikasi:** Power lucky lotto  
- **Pengembang:** frog-im  
- **Kontak:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Tanggal berlaku:** 2026-01-29  

> Kebijakan ini disusun dengan merujuk pada hukum privasi yang berlaku seperti Korea PIPA, GDPR/UK GDPR, FADP Swiss, serta hukum privasi negara bagian di AS yang relevan.  
> Jika wilayah Anda memiliki persyaratan wajib tertentu, persyaratan tersebut yang berlaku.

---

## 1. Tujuan dan ruang lingkup

Power lucky lotto adalah aplikasi untuk mengelola permainan lotre dan melihat catatan. Fitur utama meliputi:

- Pemilihan negara/permainan dan pengaturan (misalnya, KR 6/45, US Powerball)  
- Pembuatan/penyimpanan angka serta melihat log (riwayat)  
- Melihat dan menghapus tabel log (daftar tabel/detail)  
- Mengedit/mengelola data hasil permainan melalui JSON (untuk statistik/visualisasi)  
- Iklan (termasuk iklan berhadiah) dan pengelolaan persetujuan (jika diperlukan)

Aplikasi ini **tidak memerlukan pembuatan akun** dan, secara default, **tidak mengunggah data Anda ke server pengembang.**  
Sebagian besar pemrosesan terjadi **di perangkat Anda**.

Namun, untuk **periklanan**, **pengelolaan persetujuan**, dan **kepatuhan hukum**, SDK pihak ketiga seperti  
**Google Mobile Ads SDK (AdMob)** dan **Google UMP (User Messaging Platform)** dapat mengumpulkan dan memproses data tertentu (misalnya, pengenal iklan).

---

## 2. Jenis data yang diproses

### 2-1) Data yang disimpan di perangkat Anda (penyimpanan lokal)

Aplikasi menyimpan beberapa data **secara lokal di perangkat Anda** untuk menyediakan fitur dan meningkatkan kenyamanan.  
Data ini umumnya **tidak dikirim ke server pengembang** dan akan dihapus saat Anda menghapus data aplikasi atau mencopot pemasangan aplikasi (kecuali file yang Anda ekspor ke tempat lain).

#### (1) Pengaturan (SharedPreferences)

| Kategori | Kunci (contoh) | Tujuan | Penyimpanan | Penghapusan |
|---|---|---|---|---|
| Penyiapan selesai | `setup_done` | Menyimpan status penyiapan awal | SharedPreferences | Dihapus saat hapus data aplikasi/copot pemasangan |
| Riwayat negara | `selected_countries` | Menyimpan negara yang baru dipilih | Sama | Sama |
| Negara aktif | `active_country` | Menyimpan negara yang sedang dipilih | Sama | Sama |
| Permainan terpilih | `selected_lotto_ids` | Menyimpan ID permainan yang dicentang | Sama | Sama |
| Permainan aktif | `active_lotto_id` | Menyimpan ID permainan yang aktif | Sama | Sama |
| **Pemilihan waktu seed (opsional)** | `birth_datetime_iso` | Menyimpan waktu referensi seed yang dipilih pengguna (dapat digunakan untuk seeding/personalization) | Sama | Sama |

> **Catatan:** “Pemilihan waktu seed (opsional)” hanya diproses jika pengguna memilih untuk mengaturnya dan mungkin tidak diperlukan untuk penggunaan inti aplikasi.

#### (2) Data log (SQLite)

Aplikasi dapat menyimpan catatan yang dihasilkan/disimpan dalam basis data SQLite lokal.

- Contoh tabel: `log_...`  
- Contoh kolom:  
  - `id`, `date_id` atau `date_text` (timestamp), `choice1..choiceN` (angka yang dipilih), `isFinger` (flag terkait sidik jari, dll.)

Anda dapat melihat log pada layar daftar/detail tabel dan menghapusnya (per tabel atau per baris) jika diinginkan.

#### (3) File data JSON (per permainan)

Aplikasi dapat menyimpan data JSON per permainan pada direktori dokumen aplikasi.

- Contoh: `game_json/<gameId>.json`  
- Tujuan: data undian/hasil yang dikelola dan dapat diedit oleh pengguna (misalnya untuk statistik/visualisasi)

File ini disimpan di perangkat dan umumnya terhapus saat aplikasi dicopot, tergantung perilaku OS/backup.

---

### 2-2) Iklan, persetujuan, dan data terkait (SDK pihak ketiga)

Aplikasi menggunakan **Google Mobile Ads SDK (AdMob)** dan **Google UMP** untuk:

- Menampilkan iklan (termasuk **iklan berhadiah**)  
- Mengelola persetujuan yang diwajibkan secara hukum untuk periklanan

SDK ini dapat mengumpulkan/memproses, misalnya:

- **ID Iklan** (misalnya AAID, IDFA)  
- Info berbasis IP, perkiraan lokasi, info jaringan  
- Info perangkat/aplikasi (versi OS, versi aplikasi, bahasa, info diagnostik)  
- Interaksi iklan (tayangan, klik, penyelesaian reward)  
- Pilihan persetujuan yang dicatat oleh UMP

Di beberapa wilayah (misalnya EEA/UK/CH), formulir persetujuan UMP dapat ditampilkan dan entri **Privacy Options** dapat disediakan sesuai kebutuhan.

---

## 3. Retensi

- **Pengaturan lokal (SharedPreferences):** disimpan hingga penghapusan data aplikasi atau copot pemasangan  
- **Data log (SQLite):** disimpan hingga Anda menghapusnya atau mencopot/menghapus data aplikasi  
- **File JSON:** disimpan di direktori dokumen aplikasi; sering kali terhapus saat copot pemasangan, tetapi ekspor/backup dikelola pengguna  
- **Data iklan/persetujuan (pihak ketiga):** disimpan sesuai kebijakan Google dan hukum yang berlaku

---

## 4. Berbagi dengan pihak ketiga dan transfer internasional

Untuk iklan dan pengelolaan persetujuan, sebagian data dapat diproses oleh **Google dan mitranya**.

| Item | Rincian |
|---|---|
| **Penerima** | Google LLC, afiliasi, dan subprosesor |
| **Tujuan transfer** | Amerika Serikat dan wilayah lain tempat infrastruktur Google berada |
| **Tujuan** | Penyajian iklan, pengukuran, pencegahan fraud, pengelolaan persetujuan, kepatuhan |
| **Data** | ID iklan, info berbasis IP, info perangkat/aplikasi, data interaksi iklan, status persetujuan |
| **Retensi** | Sesuai kebijakan Google dan hukum yang berlaku |
| **Dampak jika menolak** | Iklan yang dipersonalisasi dapat dibatasi; iklan non-personalisasi atau lebih sedikit iklan dapat ditampilkan |

---

## 5. Hak Anda dan cara menjalankannya

Bergantung pada hukum yang berlaku, Anda dapat memiliki hak seperti akses, koreksi, penghapusan, pembatasan, keberatan, portabilitas, dan penarikan persetujuan (jika persetujuan menjadi dasar hukum).

Contoh:

- **Mengubah pilihan iklan/persetujuan:** melalui Privacy Options di dalam aplikasi (jika tersedia) atau pengaturan iklan OS (reset ID iklan, batasi personalisasi).  
- **Mereset data lokal:** hapus data aplikasi atau copot pemasangan aplikasi untuk menghapus pengaturan/log/file lokal yang disimpan aplikasi.

---

## 6. Privasi anak

Aplikasi ini **tidak dirancang untuk anak-anak**. Jika anak menggunakan aplikasi ini, wali sebaiknya mempertimbangkan kontrol orang tua tingkat OS dan fitur pembatasan iklan.

---

## 7. Langkah keamanan

Dalam cakupan aplikasi, kami berupaya untuk:

- Menyimpan data minimum yang diperlukan secara lokal  
- Mempertahankan pemrosesan di perangkat jika memungkinkan  
- Mengandalkan TLS/transport aman untuk komunikasi jaringan SDK (sesuai kemampuan SDK)

---

## 8. Data safety Google Play

Jika didistribusikan melalui Google Play, kami berupaya agar pengungkapan Data safety akurat dan selalu diperbarui, terutama saat SDK atau praktik pemrosesan berubah.

---

## 9. Pemberitahuan open-source

Aplikasi dapat menggunakan pustaka open-source untuk ikon negara, penyimpanan, iklan/persetujuan, dan UI.  
Pemberitahuan lisensi tersedia di layar “Open-source licenses” (atau yang setara) di dalam aplikasi.

---

## 10. Kontak

Untuk pertanyaan privasi:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Harap sebutkan **“Power lucky lotto”** dalam pesan Anda.

---

## 11. Perubahan kebijakan ini

Kebijakan ini dapat berubah karena pembaruan hukum, perubahan fitur (misalnya SDK baru), atau penyesuaian kebijakan internal.  
Perubahan kecil akan dipublikasikan di aplikasi atau halaman ini; perubahan material akan diumumkan sebelumnya sesuai yang diwajibkan.

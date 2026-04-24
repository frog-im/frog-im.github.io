---
title: Dasar Privasi | Power lucky lotto
description: Dasar Privasi Power lucky lotto (Bahasa Melayu)
lang: ms
last_updated: 2026-01-29
---

# Dasar Privasi (Power lucky lotto)

- **Nama aplikasi:** Power lucky lotto  
- **Pembangun:** frog-im  
- **Hubungi:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Tarikh berkuat kuasa:** 2026-01-29  

> Dasar ini disediakan dengan merujuk kepada undang-undang privasi yang berkenaan seperti Korea PIPA, GDPR/UK GDPR, Swiss FADP, serta undang-undang privasi negeri tertentu di AS.  
> Jika wilayah anda mempunyai keperluan mandatori tertentu, keperluan tersebut diutamakan.

---

## 1. Tujuan dan skop

Power lucky lotto ialah aplikasi untuk mengurus permainan loteri dan melihat rekod. Ciri utama termasuk:

- Pemilihan negara/permainan dan persediaan (cth. KR 6/45, US Powerball)  
- Penjanaan/penyimpanan nombor dan paparan log (sejarah)  
- Melihat dan memadam jadual log (senarai jadual/perincian)  
- Mengedit/mengurus data keputusan permainan melalui JSON (untuk statistik/visualisasi)  
- Iklan (termasuk iklan ganjaran) dan pengurusan persetujuan (jika diperlukan)

Aplikasi ini **tidak memerlukan pendaftaran akaun** dan secara lalai **tidak memuat naik data anda ke pelayan pembangun.**  
Kebanyakan pemprosesan berlaku **pada peranti anda**.

Walau bagaimanapun, untuk **pengiklanan**, **pengurusan persetujuan**, dan **pematuhan undang-undang**, SDK pihak ketiga seperti  
**Google Mobile Ads SDK (AdMob)** dan **Google UMP (User Messaging Platform)** mungkin mengumpul dan memproses data tertentu (cth. pengenal iklan).

---

## 2. Jenis data yang diproses

### 2-1) Data yang disimpan pada peranti anda (storan tempatan)

Aplikasi menyimpan sesetengah data **secara tempatan pada peranti anda** untuk menyediakan ciri dan meningkatkan kebolehgunaan.  
Data ini lazimnya **tidak dihantar ke pelayan pembangun** dan akan dipadam apabila anda memadam data aplikasi atau menyahpasang aplikasi (kecuali fail yang anda eksport ke tempat lain).

[Local Settings and Stored Values](https://frog-im.github.io/privacy/Power%20lucky%20lotto/en/local/)

### 2-2) Iklan, persetujuan dan data berkaitan (SDK pihak ketiga)

Aplikasi menggunakan **Google Mobile Ads SDK (AdMob)** dan **Google UMP** untuk:

- Memaparkan iklan (termasuk **iklan ganjaran**)  
- Mengurus persetujuan yang diperlukan oleh undang-undang untuk pengiklanan

SDK ini mungkin mengumpul/memproses, sebagai contoh:

- **ID Pengiklanan** (cth. AAID, IDFA)  
- Maklumat berasaskan IP, lokasi anggaran, maklumat rangkaian  
- Maklumat peranti/aplikasi (versi OS, versi aplikasi, bahasa, maklumat diagnostik)  
- Interaksi iklan (paparan, klik, ganjaran selesai)  
- Pilihan persetujuan yang direkod melalui UMP

Di sesetengah wilayah (cth. EEA/UK/CH), borang persetujuan UMP mungkin dipaparkan dan entri **Privacy Options** mungkin disediakan jika diperlukan.

---

## 3. Tempoh simpanan

- **Tetapan tempatan (SharedPreferences):** disimpan sehingga padam data aplikasi atau nyahpasang  
- **Data log (SQLite):** disimpan sehingga anda memadamnya atau nyahpasang/padam data aplikasi  
- **Fail JSON:** disimpan dalam direktori dokumen aplikasi; sering dipadam semasa nyahpasang, tetapi eksport/sandaran diurus pengguna  
- **Data iklan/persetujuan (pihak ketiga):** disimpan mengikut dasar Google dan undang-undang terpakai

---

## 4. Perkongsian pihak ketiga dan pemindahan antarabangsa

Untuk iklan dan pengurusan persetujuan, sesetengah data mungkin diproses oleh **Google dan rakan kongsinya**.

| Item | Butiran |
|---|---|
| **Penerima** | Google LLC, syarikat berkaitan, dan pemproses subkontrak |
| **Destinasi pemindahan** | Amerika Syarikat dan wilayah lain di mana infrastruktur Google berada |
| **Tujuan** | Penyampaian iklan, pengukuran, pencegahan penipuan, pengurusan persetujuan, pematuhan |
| **Data** | ID Pengiklanan, maklumat berasaskan IP, maklumat peranti/aplikasi, data interaksi iklan, status persetujuan |
| **Simpanan** | Mengikut dasar Google dan undang-undang terpakai |
| **Kesan jika menolak** | Iklan diperibadikan mungkin terhad; iklan tidak diperibadikan atau iklan yang lebih sedikit mungkin dipaparkan |

---

## 5. Hak anda dan cara melaksanakannya

Bergantung pada undang-undang terpakai, anda mungkin mempunyai hak seperti akses, pembetulan, pemadaman, sekatan pemprosesan, bantahan, kebolehalihan data, dan penarikan balik persetujuan (jika persetujuan ialah asas undang-undang).

Contoh:

- **Laraskan pilihan iklan/persetujuan:** melalui Privacy Options dalam aplikasi (jika tersedia) atau tetapan iklan OS (set semula ID iklan, hadkan pemperibadian).  
- **Tetapkan semula data tempatan:** padam data aplikasi atau nyahpasang untuk membuang tetapan/log/fail tempatan yang disimpan aplikasi.

---

## 6. Privasi kanak-kanak

Aplikasi ini **bukan direka untuk kanak-kanak**. Jika kanak-kanak menggunakannya, penjaga harus mempertimbangkan kawalan ibu bapa pada peringkat OS dan ciri had iklan.

---

## 7. Langkah keselamatan

Dalam skop aplikasi, kami berusaha untuk:

- Menyimpan hanya data minimum yang perlu secara tempatan  
- Mengekalkan pemprosesan pada peranti apabila boleh  
- Bergantung pada TLS/pengangkutan selamat untuk komunikasi rangkaian SDK (dalam keupayaan SDK)

---

## 8. Google Play Data safety

Jika diedarkan di Google Play, kami berhasrat memastikan pendedahan Data safety tepat dan dikemas kini, khususnya apabila SDK atau amalan pemprosesan berubah.

---

## 9. Notis sumber terbuka

Aplikasi mungkin menggunakan perpustakaan sumber terbuka untuk ikon negara, storan, iklan/persetujuan dan UI.  
Notis lesen tersedia dalam skrin “Open-source licenses” (atau setara) di dalam aplikasi.

---

## 10. Hubungi

Untuk pertanyaan privasi:

- **E-mel:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Sila nyatakan **“Power lucky lotto”** dalam mesej anda.

---

## 11. Perubahan dasar ini

Dasar ini mungkin berubah disebabkan kemas kini undang-undang, perubahan ciri (cth. SDK baharu), atau pelarasan dasar dalaman.  
Perubahan kecil akan disiarkan dalam aplikasi atau pada halaman ini; perubahan material akan diumumkan lebih awal sebagaimana diperlukan.

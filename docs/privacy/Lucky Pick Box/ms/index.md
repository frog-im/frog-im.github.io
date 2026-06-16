---
title: Dasar Privasi | Lucky Pick Box
description: Lucky Pick Box Dasar Privasi
lang: ms
last_updated: 2026-06-15
---

# Dasar Privasi (Lucky Pick Box / 뽑기박스)

- **Nama Aplikasi:** Lucky Pick Box / 뽑기박스
- **Pembangun:** frog-im
- **Pegawai Perlindungan Maklumat Peribadi / Orang Untuk Dihubungi:** frog-im
- **Hubungi:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tarikh Berkuat Kuasa:** 2026-06-12
- **Kemas Kini Terakhir:** 2026-06-15

> Dasar ini disediakan berdasarkan maklumat yang diproses oleh aplikasi dan ciri-ciri yang berkaitan dengannya.  
> Jika terdapat mana-mana undang-undang atau peraturan mandatori yang terpakai di negara atau wilayah tertentu, undang-undang atau peraturan tersebut boleh mengatasi dasar ini.

---

## 1. Tujuan dan Skop

Lucky Pick Box ialah alat santai untuk pilihan rawak, cabutan, pemilihan giliran, pembahagian pasukan, dadu, syiling, tangga, roda dan permainan keputusan harian atau berkumpulan yang serupa. Aplikasi tidak menyediakan perjudian wang sebenar, pertaruhan, transaksi kewangan, hadiah tunai atau ganjaran setara tunai.

### A. Ciri utama

- Input pantas: teks yang ditaip pengguna atau dibaca daripada imej yang dipilih.
- Permainan pilihan rawak: tangga, roda, plinko, cabutan ringkas, dadu, syiling, nombor rawak, pembahagi pasukan, pemilih giliran, kad, bom dan ya/tidak.
- Sejarah keputusan: jenis permainan, tajuk, peserta/item, ringkasan keputusan dan masa ciptaan boleh disimpan.
- Slot tetapan: sesetengah permainan boleh menyimpan peserta, senarai, julat, kuantiti, pasukan, pemberat dan tetapan serupa dalam sehingga 3 slot setempat.

Aplikasi tidak memerlukan pendaftaran atau log masuk. Kami tidak mengendalikan pelayan yang menerima nama, nombor telefon, alamat e-mel, kenalan, input permainan, imej yang dipilih atau keputusan permainan daripada aplikasi.

Untuk menyediakan ciri, aplikasi boleh menyimpan input permainan, label peserta, keputusan terkini, tetapan permainan yang disimpan, tetapan animasi, pilihan privasi iklan dan status berkaitan persetujuan dalam storan setempat peranti anda. Sejarah keputusan terkini dihadkan oleh aplikasi dan tidak dihantar ke pelayan yang dikendalikan oleh pembangun.

---

## 2. Kategori Maklumat Peribadi yang Diproses

### 2-1) Maklumat yang Dimasukkan Secara Terus oleh Pengguna

Aplikasi tidak memerlukan pendaftaran atau log masuk. Kami tidak mengendalikan pelayan yang menerima nama, nombor telefon, alamat e-mel, kenalan, input permainan, imej yang dipilih atau keputusan permainan daripada aplikasi.

### 2-2) Fail yang Dipilih pada Peranti

Jika anda memilih untuk membaca teks daripada imej, aplikasi meminta anda memilih imej daripada pustaka foto. Imej yang dipilih digunakan untuk pengecaman teks pada peranti melalui pemilih imej platform dan komponen Google ML Kit. Pembangun tidak memuat naik imej ke pelayan yang dikendalikan pembangun dan tidak menyimpannya dalam akaun jauh.

### 2-3) Data yang Disimpan Secara Setempat dalam Aplikasi

Untuk menyediakan ciri, aplikasi boleh menyimpan input permainan, label peserta, keputusan terkini, tetapan permainan yang disimpan, tetapan animasi, pilihan privasi iklan dan status berkaitan persetujuan dalam storan setempat peranti anda. Sejarah keputusan terkini dihadkan oleh aplikasi dan tidak dihantar ke pelayan yang dikendalikan oleh pembangun.

### B. Data setempat pada peranti

| Lokasi atau kunci | Data | Tujuan | Pemadaman |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, jenis permainan, tajuk, peserta/item, ringkasan, masa; sehingga 50 keputusan terkini. | Papar keputusan terkini dan sejarah. | Padam sejarah dalam aplikasi, kosongkan data atau nyahpasang |
| `game_settings.<gameId>.slot_<n>` | Tetapan permainan, masa simpan, senarai, julat, kuantiti, pasukan, pemberat; sehingga 3 slot. | Muat semula tetapan permainan. | Kosongkan slot, kosongkan data atau nyahpasang |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Tetapan animasi dan skrin penuh. | Kekalkan pilihan paparan. | Tukar tetapan, kosongkan data atau nyahpasang |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Pilihan privasi iklan dan kiraan kekerapan iklan. | Guna pilihan serantau dan kawal kekerapan. | Tukar tetapan, kosongkan data atau nyahpasang |
| Pemilih imej dan OCR | Laluan imej dipilih dan teks dikenali boleh diproses sementara. | Tambah teks imej ke input pantas. | Cache aplikasi/OS atau pengosongan data |

Teks input pantas tidak dihantar ke pelayan pembangun. Ia hanya boleh menjadi data setempat jika digunakan dalam keputusan permainan atau tetapan yang disimpan.

### 2-4) Maklumat yang Mungkin Diproses Secara Automatik Semasa Pengurusan Pengiklanan dan Persetujuan

Pada platform yang disokong, pada masa ini Android, aplikasi menggunakan Google AdMob dan Google User Messaging Platform (UMP). Google dan rakan pengiklanan boleh memproses pengecam iklan, pengecam kejadian aplikasi, alamat IP, lokasi anggaran, maklumat peranti dan rangkaian, versi aplikasi, sistem operasi, bahasa, paparan iklan, klik dan interaksi, diagnostik, status persetujuan dan tetapan privasi iklan serantau untuk penyampaian iklan, had kekerapan, pencegahan penipuan, pengurusan persetujuan, pengukuran, analitik, keselamatan dan pematuhan undang-undang.

Amalan privasi Google diterangkan di https://policies.google.com/privacy dan https://policies.google.com/technologies/ads.

---

## 3. Tujuan Pemprosesan Maklumat Peribadi

Lucky Pick Box ialah alat santai untuk pilihan rawak, cabutan, pemilihan giliran, pembahagian pasukan, dadu, syiling, tangga, roda dan permainan keputusan harian atau berkumpulan yang serupa. Aplikasi tidak menyediakan perjudian wang sebenar, pertaruhan, transaksi kewangan, hadiah tunai atau ganjaran setara tunai.

### A. Ciri utama

- Input pantas: teks yang ditaip pengguna atau dibaca daripada imej yang dipilih.
- Permainan pilihan rawak: tangga, roda, plinko, cabutan ringkas, dadu, syiling, nombor rawak, pembahagi pasukan, pemilih giliran, kad, bom dan ya/tidak.
- Sejarah keputusan: jenis permainan, tajuk, peserta/item, ringkasan keputusan dan masa ciptaan boleh disimpan.
- Slot tetapan: sesetengah permainan boleh menyimpan peserta, senarai, julat, kuantiti, pasukan, pemberat dan tetapan serupa dalam sehingga 3 slot setempat.

Pada platform yang disokong, pada masa ini Android, aplikasi menggunakan Google AdMob dan Google User Messaging Platform (UMP). Google dan rakan pengiklanan boleh memproses pengecam iklan, pengecam kejadian aplikasi, alamat IP, lokasi anggaran, maklumat peranti dan rangkaian, versi aplikasi, sistem operasi, bahasa, paparan iklan, klik dan interaksi, diagnostik, status persetujuan dan tetapan privasi iklan serantau untuk penyampaian iklan, had kekerapan, pencegahan penipuan, pengurusan persetujuan, pengukuran, analitik, keselamatan dan pematuhan undang-undang.

Amalan privasi Google diterangkan di https://policies.google.com/privacy dan https://policies.google.com/technologies/ads.

---

## 4. Tempoh Penyimpanan dan Retensi Maklumat Peribadi

Sejarah setempat dan tetapan boleh kekal pada peranti sehingga anda memadam sejarah, mengosongkan data aplikasi atau menyahpasang aplikasi. Anda boleh mengubah pilihan privasi iklan yang tersedia dalam tetapan aplikasi, membuka pilihan privasi Google apabila diperlukan dan mengurus atau menetapkan semula pengecam iklan dalam tetapan privasi peranti. Penyimpanan maklumat yang diproses oleh Google tertakluk pada dasar dan kewajipan undang-undang Google.

### B. Data setempat pada peranti

| Lokasi atau kunci | Data | Tujuan | Pemadaman |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, jenis permainan, tajuk, peserta/item, ringkasan, masa; sehingga 50 keputusan terkini. | Papar keputusan terkini dan sejarah. | Padam sejarah dalam aplikasi, kosongkan data atau nyahpasang |
| `game_settings.<gameId>.slot_<n>` | Tetapan permainan, masa simpan, senarai, julat, kuantiti, pasukan, pemberat; sehingga 3 slot. | Muat semula tetapan permainan. | Kosongkan slot, kosongkan data atau nyahpasang |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Tetapan animasi dan skrin penuh. | Kekalkan pilihan paparan. | Tukar tetapan, kosongkan data atau nyahpasang |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Pilihan privasi iklan dan kiraan kekerapan iklan. | Guna pilihan serantau dan kawal kekerapan. | Tukar tetapan, kosongkan data atau nyahpasang |
| Pemilih imej dan OCR | Laluan imej dipilih dan teks dikenali boleh diproses sementara. | Tambah teks imej ke input pantas. | Cache aplikasi/OS atau pengosongan data |

Teks input pantas tidak dihantar ke pelayan pembangun. Ia hanya boleh menjadi data setempat jika digunakan dalam keputusan permainan atau tetapan yang disimpan.

---

## 5. Prosedur dan Kaedah Pemadaman Maklumat Peribadi

Sejarah setempat dan tetapan boleh kekal pada peranti sehingga anda memadam sejarah, mengosongkan data aplikasi atau menyahpasang aplikasi. Anda boleh mengubah pilihan privasi iklan yang tersedia dalam tetapan aplikasi, membuka pilihan privasi Google apabila diperlukan dan mengurus atau menetapkan semula pengecam iklan dalam tetapan privasi peranti. Penyimpanan maklumat yang diproses oleh Google tertakluk pada dasar dan kewajipan undang-undang Google.

### C. Kebenaran, SDK, sandaran dan keselamatan

Aplikasi boleh menggunakan `INTERNET`, `ACCESS_NETWORK_STATE` dan `com.google.android.gms.permission.AD_ID` untuk iklan dan notis undang-undang. Akses foto atau pemilih imej hanya digunakan apabila pengguna memilih membaca teks daripada imej.

Google Mobile Ads SDK boleh memproses alamat IP, interaksi iklan, diagnostik dan pengecam peranti/akaun untuk iklan, analitik dan pencegahan penipuan. UMP boleh memproses status persetujuan dan pilihan privasi.

Data setempat boleh dipadam melalui ciri aplikasi, pengosongan data aplikasi oleh sistem operasi atau nyahpasang. Sandaran sistem, tangkapan skrin atau fail dikongsi pengguna boleh kekal mengikut dasar penyedia. Elakkan memasukkan data sensitif dalam medan teks bebas.

---

## 6. Penyediaan kepada Pihak Ketiga, Pemprosesan Secara Penyumberan Luar, dan Pemindahan Rentas Sempadan

Kami tidak menjual input permainan, label peserta, keputusan permainan atau imej yang dipilih. Apabila ciri iklan atau persetujuan diminta, Google LLC, ahli gabungan Google dan penyedia perkhidmatan mereka boleh memproses maklumat iklan dan persetujuan di negara di luar negara atau rantau anda. Lihat "Notis Pemindahan Data Antarabangsa" dalam aplikasi untuk butiran lanjut.

| Perkara | Butiran |
|---|---|
| **Penerima / Pihak yang Diamanahkan** | Google LLC dan syarikat sekutunya (pengendali AdMob / UMP) |
| **Negara Pemindahan** | Amerika Syarikat dan wilayah tempat infrastruktur Google dikendalikan |
| **Masa Pemindahan** | Secara berterusan semasa permintaan iklan, semakan status persetujuan, pemulaan SDK, dan operasi |
| **Kaedah Pemindahan** | Penghantaran melalui komunikasi rangkaian antara aplikasi dan pelayan pihak ketiga |
| **Asas Undang-Undang untuk Pemindahan Rentas Sempadan** | Diproses dalam skop yang perlu untuk menyediakan perkhidmatan di bawah asas undang-undang yang terpakai, atau apabila perlu, berdasarkan persetujuan subjek data |
| **Tujuan** | Penyiaran iklan, pengukuran iklan, pengurusan persetujuan, pencegahan penipuan, dan pematuhan terhadap dasar / undang-undang |
| **Kategori Data (Contoh)** | Pengecam pengiklanan (AAID / IDFA), maklumat IP / rangkaian, maklumat peranti / aplikasi, maklumat interaksi iklan, status persetujuan |
| **Tempoh Penyimpanan** | Tertakluk kepada dasar Google dan undang-undang yang terpakai |
| **Kesan Penolakan** | Iklan diperibadikan mungkin dihadkan, iklan tidak diperibadikan mungkin dipaparkan, atau sesetengah ciri berkaitan iklan mungkin dihadkan |

---

## 7. Maklumat tentang Kebenaran yang Digunakan

### C. Kebenaran, SDK, sandaran dan keselamatan

Aplikasi boleh menggunakan `INTERNET`, `ACCESS_NETWORK_STATE` dan `com.google.android.gms.permission.AD_ID` untuk iklan dan notis undang-undang. Akses foto atau pemilih imej hanya digunakan apabila pengguna memilih membaca teks daripada imej.

Google Mobile Ads SDK boleh memproses alamat IP, interaksi iklan, diagnostik dan pengecam peranti/akaun untuk iklan, analitik dan pencegahan penipuan. UMP boleh memproses status persetujuan dan pilihan privasi.

Data setempat boleh dipadam melalui ciri aplikasi, pengosongan data aplikasi oleh sistem operasi atau nyahpasang. Sandaran sistem, tangkapan skrin atau fail dikongsi pengguna boleh kekal mengikut dasar penyedia. Elakkan memasukkan data sensitif dalam medan teks bebas.

---

## 8. Pemasangan, Pengendalian, dan Penolakan Mekanisme Pengumpulan Automatik

Pada platform yang disokong, pada masa ini Android, aplikasi menggunakan Google AdMob dan Google User Messaging Platform (UMP). Google dan rakan pengiklanan boleh memproses pengecam iklan, pengecam kejadian aplikasi, alamat IP, lokasi anggaran, maklumat peranti dan rangkaian, versi aplikasi, sistem operasi, bahasa, paparan iklan, klik dan interaksi, diagnostik, status persetujuan dan tetapan privasi iklan serantau untuk penyampaian iklan, had kekerapan, pencegahan penipuan, pengurusan persetujuan, pengukuran, analitik, keselamatan dan pematuhan undang-undang.

Amalan privasi Google diterangkan di https://policies.google.com/privacy dan https://policies.google.com/technologies/ads.

Sejarah setempat dan tetapan boleh kekal pada peranti sehingga anda memadam sejarah, mengosongkan data aplikasi atau menyahpasang aplikasi. Anda boleh mengubah pilihan privasi iklan yang tersedia dalam tetapan aplikasi, membuka pilihan privasi Google apabila diperlukan dan mengurus atau menetapkan semula pengecam iklan dalam tetapan privasi peranti. Penyimpanan maklumat yang diproses oleh Google tertakluk pada dasar dan kewajipan undang-undang Google.

---

## 9. Hak Pengguna dan Cara Menggunakannya

Sejarah setempat dan tetapan boleh kekal pada peranti sehingga anda memadam sejarah, mengosongkan data aplikasi atau menyahpasang aplikasi. Anda boleh mengubah pilihan privasi iklan yang tersedia dalam tetapan aplikasi, membuka pilihan privasi Google apabila diperlukan dan mengurus atau menetapkan semula pengecam iklan dalam tetapan privasi peranti. Penyimpanan maklumat yang diproses oleh Google tertakluk pada dasar dan kewajipan undang-undang Google.

---

## 10. Langkah-Langkah Keselamatan

### C. Kebenaran, SDK, sandaran dan keselamatan

Aplikasi boleh menggunakan `INTERNET`, `ACCESS_NETWORK_STATE` dan `com.google.android.gms.permission.AD_ID` untuk iklan dan notis undang-undang. Akses foto atau pemilih imej hanya digunakan apabila pengguna memilih membaca teks daripada imej.

Google Mobile Ads SDK boleh memproses alamat IP, interaksi iklan, diagnostik dan pengecam peranti/akaun untuk iklan, analitik dan pencegahan penipuan. UMP boleh memproses status persetujuan dan pilihan privasi.

Data setempat boleh dipadam melalui ciri aplikasi, pengosongan data aplikasi oleh sistem operasi atau nyahpasang. Sandaran sistem, tangkapan skrin atau fail dikongsi pengguna boleh kekal mengikut dasar penyedia. Elakkan memasukkan data sensitif dalam medan teks bebas.

### C. Kebenaran, SDK, sandaran dan keselamatan

Aplikasi boleh menggunakan `INTERNET`, `ACCESS_NETWORK_STATE` dan `com.google.android.gms.permission.AD_ID` untuk iklan dan notis undang-undang. Akses foto atau pemilih imej hanya digunakan apabila pengguna memilih membaca teks daripada imej.

Google Mobile Ads SDK boleh memproses alamat IP, interaksi iklan, diagnostik dan pengecam peranti/akaun untuk iklan, analitik dan pencegahan penipuan. UMP boleh memproses status persetujuan dan pilihan privasi.

Data setempat boleh dipadam melalui ciri aplikasi, pengosongan data aplikasi oleh sistem operasi atau nyahpasang. Sandaran sistem, tangkapan skrin atau fail dikongsi pengguna boleh kekal mengikut dasar penyedia. Elakkan memasukkan data sensitif dalam medan teks bebas.

---

## 11. Maklumat Berkaitan Data Sensitif

Aplikasi ini tidak memerlukan pengguna untuk memasukkan data sensitif.  
Pengguna dinasihatkan agar tidak memasukkan kandungan sensitif seperti maklumat kesihatan, pandangan politik, agama, maklumat biometrik, atau maklumat yang berkaitan dengan kehidupan seksual ke dalam nota atau medan input bebas.

Jika pengguna secara sukarela memasukkan kandungan sensitif, maklumat tersebut boleh disimpan sebagai data setempat pada peranti yang diuruskan secara langsung oleh pengguna.

---


## 12. Perlindungan Maklumat Peribadi Kanak-Kanak

Aplikasi ini tidak direka terutamanya untuk kanak-kanak.  
Penjaga boleh mengurus penggunaan melalui ciri kawalan ibu bapa yang disediakan oleh peranti atau gedung aplikasi.

---


## 13. Pembuatan Keputusan Automatik

Aplikasi ini tidak menjalankan pembuatan keputusan automatik berdasarkan maklumat peribadi yang menghasilkan kesan undang-undang atau kesan penting yang serupa.

---


## 14. Notis Keselamatan Data (Google Play, dsb.)

Pembangun berusaha mengekalkan dan mengemas kini item pendedahan keselamatan data di gedung aplikasi (seperti Google Play) selaras dengan amalan pemprosesan sebenar aplikasi dan amalan pemprosesan sebenar SDK pihak ketiga.

Walau bagaimanapun, maklumat yang dipaparkan di gedung aplikasi mungkin berbeza bergantung pada versi aplikasi, negara pengedaran, konfigurasi SDK pihak ketiga, dan perubahan dasar.

---


## 15. Notis Sumber Terbuka

Aplikasi ini menggunakan beberapa pustaka sumber terbuka.  
Maklumat tentang lesen yang berkaitan boleh didapati pada skrin berkaitan dalam aplikasi atau dalam notis yang disediakan melalui saluran pengedaran.

---


## 16. Hubungi

Untuk pertanyaan berkaitan Dasar Privasi ini:

- **Pegawai Perlindungan Maklumat Peribadi / Orang Untuk Dihubungi:** frog-im
- **E-mel:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---


## 17. Perubahan terhadap Dasar Privasi ini

Dasar ini boleh disemak semula disebabkan perubahan pada undang-undang / dasar, ciri aplikasi, atau SDK pihak ketiga.  
Jika terdapat perubahan material, notis boleh diberikan melalui notis dalam aplikasi, halaman pengedaran, atau kemas kini pada halaman dasar.

Kemas Kini Terakhir: **2026-06-15**

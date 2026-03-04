---
title: Dasar Privasi | know_me
description: know_me (PeopleNote, Memory for People) Dasar Privasi (Bahasa Melayu)
---

# Dasar Privasi (know_me / PeopleNote, Memory for People)

- **Nama Aplikasi:** know_me (PeopleNote, Memory for People)
- **Pembangun:** frog-im
- **Pegawai Perlindungan Maklumat Peribadi / Orang Untuk Dihubungi:** frog-im
- **Hubungi:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Tarikh Berkuat Kuasa:** 2026-03-04
- **Kemas Kini Terakhir:** 2026-03-04

> Dasar ini disediakan berdasarkan maklumat yang diproses oleh aplikasi dan ciri-ciri yang berkaitan dengannya.  
> Jika terdapat mana-mana undang-undang atau peraturan mandatori yang terpakai di negara atau wilayah tertentu, undang-undang atau peraturan tersebut boleh mengatasi dasar ini.

---

## 1. Tujuan dan Skop

`know_me` ialah aplikasi yang direka untuk membantu pengguna merekod dan mengurus maklumat tentang orang, dan apabila perlu, membuat sandaran, memulihkan, serta berkongsi maklumat tersebut dalam bentuk fail PDF.

Ciri utamanya termasuk:

- Menyimpan maklumat khusus bagi individu (seperti nama, teks pengenalan, nota, ciri personaliti, negara, jantina, maklumat hubungan, dan sebagainya)
- Pengelasan folder, carian, dan fungsi gabung
- Melampirkan foto dan mengurus penerangan
- Mengeksport dan mengimport sandaran (`.knm`)
- Mengeksport PDF
- Kunci aplikasi (kata laluan / corak)
- Pengurusan pengiklanan dan persetujuan (AdMob / UMP)

Aplikasi ini tidak memerlukan pendaftaran akaun yang berasingan, dan data teras pengguna secara amnya disimpan secara setempat pada peranti pengguna.  
Walau bagaimanapun, sesetengah SDK pihak ketiga yang disertakan untuk tujuan pengurusan pengiklanan dan persetujuan mungkin memproses sebahagian maklumat.

---

## 2. Kategori Maklumat Peribadi yang Diproses

### 2-1) Maklumat yang Dimasukkan Secara Terus oleh Pengguna

Maklumat berikut hanya disimpan apabila pengguna memasukkannya secara langsung:

- Nama
- Teks pengenalan (seperti rupa / ciri yang digunakan sebagai teks nota)
- Nota
- Ciri personaliti, negara, jantina
- Nombor telefon
- Teks yang berkaitan dengan waktu kemunculan / waktu pertemuan
- Maklumat platform / laman
- Nama / warna folder
- Penerangan imej (caption)

### 2-2) Fail yang Dipilih pada Peranti

- Fail imej yang dipilih oleh pengguna semasa melampirkan foto
- Fail sandaran `.knm` yang dipilih oleh pengguna semasa mengimport sandaran
- Laluan simpanan dan fail tersimpan yang dipilih oleh pengguna semasa mengeksport PDF / sandaran

### 2-3) Data yang Disimpan Secara Setempat dalam Aplikasi

Data berikut boleh disimpan pada peranti pengguna untuk menyediakan ciri-ciri aplikasi:

- Pangkalan data SQLite (`people_note.db`): metadata berkaitan orang / folder / platform / laman / imej
- Fail imej: disulitkan dan disimpan dalam folder dokumen aplikasi (`.enc`)
- Tetapan aplikasi (`SharedPreferences`): tema, pengisihan, pilihan privasi / iklan, pilihan penapisan PDF, dasar kunci aplikasi, dan sebagainya
- Maklumat kunci aplikasi: nilai hash dan salt untuk kata laluan / corak (`SharedPreferences`)
- Kunci penyulitan setempat: disimpan dalam `flutter_secure_storage`
- Fail sementara: pratonton nyahsulit imej, fail cache import / eksport, dan sebagainya (folder sementara)

### 2-4) Maklumat yang Mungkin Diproses Secara Automatik Semasa Pengurusan Pengiklanan dan Persetujuan

Apabila ciri pengiklanan atau pengurusan persetujuan diaktifkan, SDK milik Google LLC dan rakan kongsi berkaitan (seperti AdMob dan UMP) mungkin memproses maklumat berikut secara automatik:

- Pengecam pengiklanan (AAID / IDFA, dan sebagainya)
- Alamat IP dan maklumat rangkaian
- Maklumat peranti (versi OS, model peranti, versi aplikasi, dan sebagainya)
- Maklumat interaksi iklan (paparan, klik, dan sebagainya)
- Status persetujuan dan maklumat pilihan privasi
- Maklumat berkaitan diagnostik, prestasi, dan keselamatan

Rekod teras pengguna aplikasi ini secara amnya tidak dimuat naik ke pelayan pembangun, tetapi sebahagian daripada maklumat di atas mungkin dihantar kepada perkhidmatan pihak ketiga semasa ciri pengiklanan / persetujuan sedang digunakan.

---

## 3. Tujuan Pemprosesan Maklumat Peribadi

Aplikasi ini memproses maklumat peribadi atau maklumat berkaitan untuk tujuan berikut:

- Merekod dan menyemak imbas maklumat berkaitan orang yang berpusat pada kenalan / nota
- Menyediakan ciri pengurusan seperti pengelasan folder, carian, dan penggabungan
- Melampirkan dan memaparkan foto
- Menjalankan fungsi yang diminta oleh pengguna seperti sandaran / pemulihan dan eksport PDF
- Menyediakan ciri keselamatan kunci aplikasi
- Menyediakan pengiklanan, mengurus persetujuan, mencegah aktiviti penipuan, dan mematuhi kewajipan undang-undang

---

## 4. Tempoh Penyimpanan dan Retensi Maklumat Peribadi

- Data dalaman aplikasi (SQLite, tetapan setempat, imej yang disulitkan): disimpan pada peranti pengguna sehingga aplikasi dipadamkan, data aplikasi dipadamkan, atau pengguna memadam data tersebut secara langsung
- Fail sementara: dipadamkan selepas tugasan berkaitan selesai atau dibersihkan mengikut dasar cache sistem operasi
- Fail yang dieksport oleh pengguna (PDF, fail sandaran): mungkin kekal di lokasi simpanan yang dipilih oleh pengguna dan mesti dipadamkan sendiri oleh pengguna
- Data berkaitan pengiklanan / persetujuan (diproses oleh pihak ketiga): tertakluk kepada dasar setiap penyedia perkhidmatan dan undang-undang yang terpakai

Pada dasarnya, aplikasi ini tidak menyimpan rekod teras pengguna pada pelayan pembangun.  
Walau bagaimanapun, fail yang disimpan terus oleh pengguna ke storan luaran diuruskan dalam persekitaran pengguna sendiri.

---

## 5. Prosedur dan Kaedah Pemadaman Maklumat Peribadi

Apabila tujuan pemprosesan telah tercapai atau apabila pengguna meminta pemadaman, aplikasi akan memusnahkan maklumat berkaitan atau memprosesnya supaya ia tidak lagi dirujuk, seperti berikut.

### 5-1) Prosedur Pemadaman

- Apabila pengguna memadamkan rekod individu, folder, imej, data sandaran, dan sebagainya secara langsung, data tersebut dianggap tertakluk kepada pemadaman segera.
- Apabila pengguna memadam aplikasi atau mengosongkan data aplikasi daripada tetapan peranti, data yang disimpan dalam ruang storan dalaman aplikasi akan dipadamkan mengikut prosedur pemadaman sistem operasi.
- Fail sementara akan tertakluk kepada pembersihan selepas tugasan berkaitan tamat, dan sesetengah data cache mungkin kekal sehingga satu tempoh tertentu bergantung pada dasar sistem operasi.

### 5-2) Kaedah Pemadaman

- Data SQLite: pemadaman rekod yang berkaitan
- Tetapan aplikasi (`SharedPreferences`): pemadaman kunci yang berkaitan atau semua tetapan
- Nilai dalam `flutter_secure_storage`: pemadaman item storan selamat yang berkaitan
- Fail dalaman aplikasi (imej yang disulitkan, fail sementara, dan sebagainya): pemadaman fail yang berkaitan
- Fail PDF / sandaran yang disimpan terus oleh pengguna ke storan luaran: tidak dipadamkan secara automatik oleh aplikasi dan mesti dipadamkan sendiri oleh pengguna

Melainkan dikehendaki sebaliknya oleh undang-undang yang terpakai, pembangun tidak menyimpan rekod teras pengguna secara berasingan pada pelayan pembangun.

---

## 6. Penyediaan kepada Pihak Ketiga, Pemprosesan Secara Penyumberan Luar, dan Pemindahan Rentas Sempadan

Aplikasi ini mungkin menggunakan perkhidmatan Google untuk pengurusan pengiklanan dan persetujuan.

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

Pembangun tidak mengumpul atau menjual data teras rekod orang dalam aplikasi ini melalui pelayannya sendiri.

---

## 7. Maklumat tentang Kebenaran yang Digunakan

Aplikasi ini mungkin menggunakan kebenaran berikut:

- `INTERNET`: komunikasi untuk SDK pengiklanan dan ciri rangkaian berkaitan
- `com.google.android.gms.permission.AD_ID`: penggunaan pengecam pengiklanan (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 dan ke bawah): untuk melampirkan / memilih foto

Kebenaran hanya digunakan dalam skop yang perlu untuk menyediakan ciri-ciri berkaitan.

---

## 8. Pemasangan, Pengendalian, dan Penolakan Mekanisme Pengumpulan Automatik

Aplikasi ini tidak secara langsung menggunakan kuki laman web umum.  
Walau bagaimanapun, berkaitan dengan ciri pengiklanan dan pengurusan persetujuan, SDK pihak ketiga mungkin memproses pengecam pengiklanan, maklumat rangkaian, maklumat peranti, dan data seumpamanya secara automatik.

Pengguna boleh melaraskan tetapan berkaitan melalui cara berikut:

- Menukar pilihan dalam tetapan privasi aplikasi atau skrin pengurusan persetujuan (jika disediakan)
- Menetapkan semula atau memadam pengecam pengiklanan dalam tetapan sistem operasi peranti
- Mengehadkan iklan diperibadikan atau melaraskan pilihan privasi berkaitan dalam tetapan sistem operasi peranti

Jika pengguna mengehadkan iklan diperibadikan, iklan tidak diperibadikan mungkin dipaparkan, atau sesetengah ciri berkaitan iklan mungkin dihadkan.

---

## 9. Hak Pengguna dan Cara Menggunakannya

Tertakluk kepada undang-undang yang terpakai, pengguna mungkin mempunyai hak-hak berikut:

- Meminta akses kepada, pembetulan terhadap, atau pemadaman maklumat peribadi
- Meminta penggantungan atau sekatan pemprosesan
- Menarik balik persetujuan bagi pemprosesan berasaskan persetujuan
- Menukar pilihan pengiklanan / persetujuan

Hak-hak ini boleh dilaksanakan melalui cara berikut:

- Mengubah atau memadam data secara langsung dalam aplikasi
- Memulakan semula data setempat dengan memadam data aplikasi atau menyahpasang aplikasi
- Menukar persetujuan pengiklanan melalui tetapan privasi / skrin persetujuan aplikasi (di wilayah yang menyediakannya)
- Menetapkan semula / memadam pengecam pengiklanan atau mengehadkan iklan diperibadikan melalui tetapan OS peranti
- Hubungi: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Langkah-Langkah Keselamatan

Pembangun melaksanakan atau berusaha melaksanakan langkah-langkah berikut:

- Rekod pengguna secara amnya disimpan secara setempat pada peranti
- Fail imej yang dilampirkan disimpan secara setempat dalam bentuk disulitkan (berasaskan AES-GCM)
- Maklumat kunci aplikasi disimpan dalam bentuk hash, bukan teks biasa
- Fail sandaran disimpan selepas disulitkan berdasarkan kata laluan pengguna
- Komunikasi dengan SDK pihak ketiga disulitkan (HTTPS / TLS)
- Kebenaran digunakan dengan skop akses minimum yang diperlukan

Walau bagaimanapun, risiko yang timbul daripada keadaan keselamatan peranti pengguna (seperti rooting / jailbreaking, aplikasi berniat jahat, atau pendedahan storan kongsi) tidak dapat dihapuskan sepenuhnya.

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

Kemas Kini Terakhir: **2026-03-04**
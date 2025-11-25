---
title: Gizlilik Politikası | LyriFloat
description: LyriFloat Gizlilik Politikası (Türkçe)
lang: tr
last_updated: 2025-10-30
---

# Gizlilik Politikası (LyriFloat)

- **Uygulama adı:** LyriFloat
- **Geliştirici:** frog-im  
- **İletişim:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Yürürlük tarihi:** 2025-10-30

> Bu Politika; Kore Kişisel Bilgilerin Korunması Kanunu (PIPA), GDPR/UK GDPR, İsviçre FADP ve ilgili ABD eyalet gizlilik yasaları dâhil uygulanabilir düzenlemeler dikkate alınarak hazırlanmıştır. Yargı alanına özgü ek gereklilikler bulunması halinde, bu gereklilikler önceliklidir.

---

## 1. İşleme amacı ve kapsamı

Uygulama, **cihazda saklanan ses dosyalarının meta verilerini** (başlık, sanatçı vb.) düzenleme ve **şarkı sözlerini örtü (overlay) olarak gösterme** işlevleri sunar.  
Uygulama **kullanıcı hesabı oluşturmaz** ve kullanıcı içeriğini **sunucularımıza yüklemez**; işleme varsayılan olarak **kullanıcının cihazında** yapılır.

Bununla birlikte **reklam sunumu** ve **yasal uyum** amaçlarıyla, üçüncü taraf ortaklar (ör. Google Mobile Ads SDK (AdMob), UMP) **reklam tanımlayıcıları** gibi bilgileri toplayıp işleyebilir. Onay toplama ve gizlilik seçenekleri **Google UMP (User Messaging Platform)** özelliklerine göre yürütülür.

---

## 2. İşlenen bilgi kategorileri

### 2-1) Kullanıcının açıkça seçtiği dosyalar
- **Ses/kapak görseli yolları ve içerikleri:** yalnızca **yerel olarak** düzenleme/kaydetme amacıyla işlenir.  
- **FFmpegKit**, kodlama, meta düzenleme ve küçük görsel (thumbnail) çıkarma için **cihaz içinde** kullanılır.  
- Uygulama, kullanıcı tarafından seçilen dosyaları **sunucularımıza yüklemez**.

### 2-2) Yerel ayarlar ve saklanan kalemler

Çekirdek işlevler ve kullanım kolaylığı için aşağıdaki değerler **cihazda yerel olarak** saklanır.  
Bu değerler sunucularımıza gönderilmez ve **uygulama verileri silindiğinde veya uygulama kaldırıldığında** kaldırılır.

#### (1) Tercihler (`shared_preferences`)
| Tür | Anahtar/İçerik | Amaç | Saklama yeri | Silme yöntemi |
|---|---|---|---|---|
| Örtü konumu/yazı tipi | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Örtü konumu ve yazı tipi boyutunu geri yükleme | Cihazdaki SharedPreferences | Uygulama verileri silindiğinde veya kaldırıldığında |
| Reklam/Gizlilik | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Kişiselleştirilmemiş reklamlar (NPA), ABD **Kısıtlı Veri İşleme (RDP)**, COPPA etiketi, yaş etiketi, reklam içerik derecesi sınırı | Cihazdaki SharedPreferences | Aynı |

#### (2) Geçici dosyalar (sistem geçici dizini)
- **Örnekler:** `cover_*.jpg`, `tmp_*.flac`  
- **Kullanım:** kapak görseli çıkarma, FLAC etiketleme, geçici kodlamalar  
- **Konum:** işletim sisteminin geçici klasörü (`systemTemp`)  
- **Saklama süresi:** işlem tamamlandıktan sonra uygulama tarafından silinmeye çalışılır; ayrıca işletim sistemi periyodik temizleme yapabilir

#### (3) Kullanıcı tarafından seçilen kaydetme (SAF)
- “Farklı kaydet” ile çıktı dosyaları kullanıcının belirlediği konumlara (ör. İndirilenler, bulut) yazılabilir.  
- Bu dosyalar **harici depolamada** bulunur ve **uygulama kaldırıldıktan sonra da kalabilir**. Kullanıcı bunları manuel silebilir.

#### (4) Onay durumu (UMP SDK önbelleği)
- AEA/BK/İsviçre bölgelerinde UMP SDK, kullanıcının **reklam onay durumunu cihazda önbelleğe alır**.  
- Uygulama verilerini silerek veya uygulamadaki **Gizlilik Seçenekleri (Privacy Options)** ekranından sıfırlanabilir.

---

### 2-3) Reklam ve onay verileri (üçüncü taraf SDK’lar)
- **Google Mobile Ads SDK (AdMob) ve UMP**; **reklam tanımlayıcıları (AAID/IDFA)**, **IP aralıkları**, **cihaz/uygulama bilgileri**, **reklam etkileşim sinyalleri**, **onay durumu** vb. verileri toplayıp işleyebilir.  
- **Amaçlar:** reklam sunumu, sıklık sınırlandırma, sahtecilik önleme, performans ölçümü, yasal gerekliliklere uyum  
- **Onay gerektiren bölgeler (AEA/BK/İsviçre):** UMP üzerinden onay alınır ve gerektiğinde **Gizlilik Seçenekleri** ekranı sağlanır.  
  Bu gerekliliklerin bulunmadığı bölgelerde (ör. KR) **seçenek görünmeyebilir**.

---

## 3. İşleme ve saklama süreleri

- **Yerel ayarlar:** kullanıcı uygulama verilerini silene veya uygulamayı kaldırana kadar cihazda saklanır  
- **Geçici dosyalar:** kodlama/çıkarma sırasında oluşturulur; işlemden sonra silinir veya kısa süre OS önbelleklerinde kalabilir  
- **Reklam/onay verileri (üçüncü taraf):** **Google** politikalarına tabidir

---

## 4. Üçüncü tarafa sağlama ve sınır ötesi aktarımlar

Reklam ve onay yönetimi için kullanıcı bilgileri Google altyapısına iletilebilir ve orada işlenebilir.

| Kalem | Detay |
|---|---|
| **Alıcı** | Google LLC ve bağlı/alt işleyenleri |
| **Hedef ülke/bölge** | Amerika Birleşik Devletleri (ve Google altyapısının bulunduğu diğer bölgeler) |
| **Amaç** | Reklam sunumu, performans/ölçüm, yasal uyum, onay yönetimi |
| **Aktarılan veriler** | Reklam tanımlayıcıları, IP aralıkları, cihaz/uygulama bilgileri, reklam etkileşimleri, onay durumu vb. |
| **Saklama** | Google politikalarına göre |
| **Reddin etkisi** | Kişiselleştirme sınırlanabilir; yalnızca kişiselleştirilmemiş reklamlar gösterilebilir |

Uygulama, **Google Play “Veri güvenliği”** bölümünün açıklama gerekliliklerine uyar ve beyanları fiilî işleme faaliyetleriyle uyumlu tutar.

---

## 5. Kullanıcının hakları ve kullanım yolları

- **Kişiselleştirilmiş reklamlardan vazgeçme/onayı değiştirme**  
  - Desteklenen bölgelerde (AEA/BK/İsviçre): **Ayarlar → Gizlilik Seçenekleri** üzerinden tercihleri değiştirebilirsiniz.  
  - Diğer bölgelerde: işletim sistemi ayarlarından **Reklam Kimliği’ni sıfırlama/izlemeyi kısıtlama** kullanılabilir.
- **Yerel bilgileri sıfırlama:** uygulama verilerini silmek veya uygulamayı kaldırmak, örtü koordinatlarını, yazı boyutunu ve diğer yerel ayarları sıfırlar.
- **GDPR/UK GDPR/İsviçre FADP/ABD eyalet gizlilik yasaları** kapsamındaki haklar (erişim, düzeltme, silme, taşınabilirlik, işlemeyi kısıtlama, onayı geri çekme vb.) ilgili mevzuata göre kullanılabilir.  
  Google’ın işlediği reklam verileri için **Google’ın süreçlerini** kullanınız.

---

## 6. Çocukların kişisel verileri

Bu uygulama **çocukları hedeflemez**. Yasal asgari yaşın altındaki çocuklar uygulamayı kullanmayı bırakmalı ve veliyle birlikte OS düzeyindeki reklam sınırlama özelliklerini kullanmalıdır. Gerektiğinde **TFUA (çocuklara yönelik etiket)** veya benzeri koruma seçenekleri uygulanabilir.

---

## 7. Güvenlik tedbirleri

- Toplama ve saklamada **veri minimizasyonu**  
- Geçici dosyaların **sınırlı kullanımı** ve işlem sonrası silme girişimleri  
- **OS izin kapsamı** içinde işleme  
- Üçüncü taraf aktarımında **iletişim sırasında şifreleme** (TLS veya muadili; ilgili SDK standartlarına uygun)

---

## 8. Veri açıklamaları (Google Play)

Play Console’daki **“Veri güvenliği”** bölümünü doğru şekilde hazırlar ve değişikliklerde ivedilikle güncelleriz.

---

## 9. Açık kaynak bildirimleri

Uygulama **FFmpeg** gibi açık kaynak yazılımlar kullanır. Uygulama içinde yer alan bir bilgilendirme dosyası (örn. `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) kaynak koda erişim yolunu açıklar; talep hâlinde bu dosyadaki usule göre kaynak kodu sağlarız.

---

## 10. İletişim

- E-posta: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Değişiklik bildirimi

Mevzuat veya hizmet değişiklikleri nedeniyle bu Politikayı güncelleyebiliriz. Değişiklikleri **uygulama içinde** ve **bu politika sayfasında** yayımlarız.  
Önemli değişikliklerde **yürürlük tarihinden en az 7 gün önce** bildirim yaparız.

---

## Ek: Kullanıcıya yönelik bilgilendirme

- **Uygulama içi bağlantı:** **Ayarlar → Gizlilik** ekranından bu sayfayı açabilirsiniz.  
- **Bölgesel davranış:** AEA/BK/İsviçre’de Gizlilik Seçenekleri gösterilir. **KR ve bazı bölgelerde, yasal gereklilik yoksa buton ek seçenek göstermeyebilir**.



---
title: Gizlilik Politikası | Subtitle Tool
description: Subtitle Player & Editor (Subtitle Tool) için gizlilik politikası
lang: tr
last_updated: 2025-12-12
---

# Gizlilik Politikası (Subtitle Player & Editor / “Subtitle Tool”)

- **Uygulama adı:** Subtitle Player & Editor (bundan sonra “Subtitle Tool” olarak anılacaktır)  
- **Geliştirici:** frog-im  
- **İletişim:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Yürürlük tarihi:** 2025-12-12  

> Bu Politika; Kore Kişisel Bilgileri Koruma Kanunu (PIPA), GDPR/UK GDPR, İsviçre FADP ve çeşitli ABD eyalet gizlilik yasaları gibi ilgili mevzuat esas alınarak hazırlanmıştır.  
> Belirli bir ülke/bölge hukukunda özel ve bağlayıcı hükümler bulunması hâlinde, bu hükümler işbu Politikanın ilgili hükümlerine üstün gelir.

---

## 1. Amaç ve Kapsam

Bu uygulama, cihazda saklanan ses dosyalarının **meta verilerini (başlık, sanatçı vb.) düzenleme** ve **şarkı sözü/altyazı örtüşmesi (overlay) gösterme** fonksiyonları sağlar.  
Uygulama **kullanıcı hesabı oluşturmaz** ve **kullanıcı içeriğini sunucularımıza yüklemez**. İşleme, varsayılan olarak **kullanıcının cihazında yerel olarak** gerçekleştirilir.

Ancak, **reklam** ve **hukuki yükümlülüklerin yerine getirilmesi** amaçlarıyla; üçüncü taraf iş ortakları (örneğin Google Mobile Ads SDK (AdMob) ve UMP) **reklam tanımlayıcıları** gibi bilgileri toplayabilir ve işleyebilir.  
Aydınlatma metinleri, onay ekranları ve gizlilik tercihleri, **Google UMP (User Messaging Platform)** çerçevesinde yönetilir.

---

## 2. İşlediğimiz Bilgi Kategorileri

### 2-1) Kullanıcının Açıkça Seçtiği Dosyalar

- **Ses dosyası/kapak görseli yolları ve içerikleri:** yalnızca düzenleme ve kaydetme amacıyla **cihaz üzerinde yerel olarak** işlenir.  
- **FFmpegKit**, kodlama, meta veri düzenleme ve küçük resim çıkarma için yerel olarak kullanılır.  
- Uygulama, bu kullanıcı-seçimli dosyaları sunucularımıza **yüklemez**.

### 2-2) Yerel Ayarlar ve Saklanan Değerler

Temel işlevler ve kullanım kolaylığı için, uygulama aşağıdaki değerleri **cihazda yerel olarak** saklar.  
Bu veriler sunucularımıza gönderilmez ve **uygulama veya uygulama verileri silindiğinde kaldırılır**.

#### (1) Tercihler (`shared_preferences`)

| Tür | Anahtar/İçerik | Amaç | Saklama | Silme |
|---|---|---|---|---|
| Örtüşme konumu/yazı tipi | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Örtüşme kutusunun konumunu ve yazı tipi boyutunu geri yükleme | Cihazdaki SharedPreferences | Uygulama verileri veya uygulama silindiğinde kaldırılır |
| Reklam/gizlilik ayarları | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Kişiselleştirilmemiş reklamlar, ABD RDP sinyali, COPPA çocuk etiketi, yaş etiketi, reklam içerik derecelendirme sınırı | Cihazdaki SharedPreferences | Sol sütunda belirtilen şekilde |

#### (2) Geçici Dosyalar (sistem geçici klasörü)

- **Örnekler:** `cover_*.jpg`, `tmp_*.flac`  
- **Kullanım:** kapak görseli çıkarma, FLAC etiketleme, geçici kodlama  
- **Konum:** işletim sisteminin geçici klasörü (`systemTemp`)  
- **Saklama süresi:** işlem tamamlandıktan sonra uygulama tarafından mümkün olduğunca silinir; ayrıca işletim sisteminin temizlik mekanizmaları tarafından da kaldırılabilir.

#### (3) Kullanıcı Tarafından Seçilen Kayıt Yolu (SAF)

- Kullanıcı “Farklı kaydet” özelliğini kullandığında, son ses dosyaları kullanıcı tarafından seçilen konuma (örneğin İndirilenler klasörü, bulut depolama) kaydedilebilir.  
- Bu dosyalar **harici depolama alanında** bulunur ve uygulama kaldırıldıktan sonra **varlığını sürdürebilir**. Kullanıcı bu dosyaları manuel olarak silebilir.

#### (4) Onay Durumu (UMP önbelleği)

- EEA/İngiltere/İsviçre bölgelerinde UMP SDK **kullanıcının reklam onay durumunu yerel olarak önbelleğe alır**.  
- Bu durum, uygulama verilerinin silinmesiyle veya uygulama içindeki **Gizlilik Seçenekleri** ekranından (varsa) sıfırlanabilir.

---

### 2-3) Reklam ve Onaya İlişkin Veriler (Üçüncü Taraf SDK’lar)

- **Google Mobile Ads SDK (AdMob) ve UMP**, örneğin **reklam tanımlayıcıları (AAID/IDFA)**, **IP aralıkları**, **cihaz/uygulama bilgisi**, **reklam etkileşim sinyalleri**, **onay durumu** gibi verileri toplayıp işleyebilir.  
- **Amaçlar:** reklam sunumu, gösterim sıklığı sınırlaması, dolandırıcılığın önlenmesi, performans ölçümü, yasal yükümlülüklerin yerine getirilmesi.  
- **Onayın zorunlu olduğu bölgeler (EEA/İngiltere/İsviçre):** onay, UMP ekranları aracılığıyla toplanır ve gerektiğinde **Gizlilik Seçenekleri** ekranı sağlanır.  
  İlgili yasal zorunluluğun bulunmadığı bölgelerde (örneğin Kore) bu seçenek **görünmeyebilir**.

---

## 3. İşleme ve Saklama

- **Yerel ayarlar:** kullanıcı uygulama verilerini silene veya uygulamayı kaldırana kadar cihazda saklanır.  
- **Geçici dosyalar:** kodlama/çıkarma işlemleri sırasında oluşturulur, işlem tamamlandıktan sonra silinir veya bir süre sistem önbelleğinde kalabilir.  
- **Reklam/onay verileri (üçüncü taraf):** **Google politikalarına** göre saklanır ve silinir.

---

## 4. Üçüncü Taraflara Aktarım ve Sınır Ötesi Veri Akışı

Reklam ve onay yönetimi amaçlarıyla, kullanıcıya ait bazı bilgiler Google altyapısına aktarılabilir ve burada işlenebilir.

| Kalem | Ayrıntı |
|---|---|
| **Alıcı** | Google LLC ve bağlı şirketleri/alt işleyicileri |
| **Hedef bölge** | Amerika Birleşik Devletleri (ve Google altyapısının bulunduğu diğer bölgeler) |
| **Amaç** | Reklam sunumu, ölçüm ve performans, yasal uyum, onay yönetimi |
| **Veriler** | Reklam tanımlayıcıları, IP aralıkları, cihaz/uygulama bilgisi, reklam etkileşimleri, onay durumu vb. |
| **Saklama süresi** | Google’ın ilgili politikalarına göre |
| **Reddetmenin etkisi** | Kişiselleştirilmiş reklamlar sınırlanabilir; kişiselleştirilmemiş reklamlar gösterilmeye devam edebilir |

Google Play’deki **“Data safety” (Veri güvenliği)** bölümüne ilişkin gereklilikleri karşılar ve beyanlarımızı fiilî işleme faaliyetleriyle uyumlu tutarız.

---

## 5. Haklarınız ve Bunları Nasıl Kullanacağınız

- **Kişiselleştirilmiş reklamlardan vazgeçme / onayı değiştirme**  
  - İlgili bölgelerde (EEA/İngiltere/İsviçre): **Ayarlar → Gizlilik Seçenekleri** menüsünden tercihlerinizi değiştirebilirsiniz.  
  - Diğer bölgelerde: işletim sistemi ayarlarından **reklam kimliğini sıfırlama / reklam takibini sınırlama** işlemlerini kullanabilirsiniz.
- **Yerel bilgilerin sıfırlanması:** uygulama verilerinin silinmesi veya uygulamanın kaldırılması, overlay koordinatları, yazı tipi boyutu ve diğer yerel ayarları sıfırlar.  
- **GDPR/UK GDPR/İsviçre FADP/ABD eyalet gizlilik yasaları** uyarınca, geçerli olduğu ölçüde erişim, düzeltme, silme, veri taşınabilirliği, işlem kısıtlama, onayı geri çekme vb. haklara sahip olabilirsiniz.  
  Google tarafından işlenen reklam verileri için, **Google’ın sunduğu süreç ve araçları** kullanmanız gerekir.

---

## 6. Çocukların Gizliliği

Bu uygulama **çocukları hedeflememektedir**.  
Yasal asgari yaştan küçük bir çocuk uygulamayı kullanıyorsa, kullanımı bırakması ve bir veli eşliğinde işletim sisteminin sunduğu reklam sınırlandırma özelliklerini kullanması tavsiye edilir.  
Gerektiğinde, **TFUA (child-directed etiketi)** veya benzeri çocuk koruma etiketleri uygulanabilir.

---

## 7. Güvenlik Önlemleri

- Toplama ve saklama süreçlerinde **veri minimizasyonu**  
- Geçici dosyaların sınırlı süreyle kullanımı ve mümkün olduğunda işlem sonrasında silinmesi  
- İşlemenin, işletim sisteminin izin verdiği **yetki kapsamı** içinde tutulması  
- Üçüncü taraflara veri aktarımında **TLS veya eşdeğer şifreleme** kullanılması (ilgili SDK standartlarına göre)

---

## 8. Veri Güvenliği (Google Play)

Google Play Console’daki **“Data safety”** bölümünü doğru ve güncel tutar; işleme faaliyetlerinde değişiklik olduğunda gerekli güncellemeleri zamanında yaparız.

---

## 9. Açık Kaynak Yazılımlara İlişkin Bilgi

Uygulama, **FFmpeg** gibi açık kaynaklı yazılımlar kullanır.  
Uygulama içinde yer alan bir bilgilendirme dosyası (örneğin `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`), kaynak koda nasıl ulaşılacağını açıklar.  
Talep edilmesi hâlinde, bu dosyada belirtilen usule göre ilgili kaynak kodu sağlarız.

---

## 10. İletişim

- E-posta: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Bu Politikanın Değiştirilmesi

Hukuki mevzuat veya hizmet kapsamındaki değişiklikler nedeniyle bu Politikayı güncelleyebiliriz.  
Güncellemeleri **uygulama içinde** ve bu **politika sayfasında** duyururuz.  
Önemli değişiklikler için, yeni yürürlük tarihinden **en az 7 gün önce** bildirim yapmaya çalışırız.

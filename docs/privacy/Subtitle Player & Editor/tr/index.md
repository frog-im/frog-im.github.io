---
title: Gizlilik Politikası | Subtitle Tool
description: Subtitle Tool (Subtitle Player & Editor) Gizlilik Politikası - Türkçe
lang: tr
last_updated: 2026-03-11
---

# Gizlilik Politikası (Subtitle Tool / Subtitle Player & Editor)

- **Uygulama adı:** Subtitle Player & Editor (bu Politikada ayrıca **Subtitle Tool** olarak da anılır)
- **Geliştirici:** frog-im
- **İletişim:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Yürürlük tarihi:** 2026-03-11

> Bu Politika, Kore Kişisel Bilgilerin Korunması Yasası (PIPA), GDPR / UK GDPR, İsviçre FADP ve ilgili ABD eyalet gizlilik yasaları dahil olmak üzere yürürlükteki yasalara atıfla hazırlanmıştır. Zorunlu yerel kurallar uygulanıyorsa, bu kurallar öncelikli olur.

---

## 1. Amaç ve Kapsam

Bu uygulama aşağıdakileri sağlar:

- Altyazı oynatma ve düzenleme
- Kullanıcının seçtiği dosyalardan video + altyazı oynatma
- Android'de diğer uygulamaların üzerinde gösterilen kayan altyazı / şarkı sözü katmanı

Desteklenen altyazı işleme formatları şunları içerebilir:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

Uygulama **kullanıcı hesabı oluşturmaz** ve **kullanıcının altyazı veya medya dosyalarını geliştiricinin kendi sunucularına yüklemez**. Altyazı ayrıştırma, düzenleme, önizleme ve oynatmayla ilgili işlemlerin çoğu **cihaz üzerinde yerel olarak** gerçekleştirilir.

Bununla birlikte, reklam, izin/onay yönetimi ve yasal uyumluluk amaçları doğrultusunda **Google Mobile Ads SDK (AdMob)** ve **Google UMP** gibi üçüncü taraf SDK'lar; reklam tanımlayıcıları, cihaz sinyalleri ve onay tercihleri gibi belirli bilgileri işleyebilir.

---

## 2. İşlediğimiz Bilgi Kategorileri

### 2-1) Kullanıcının Açıkça Seçtiği Dosyalar

Uygulama, kullanıcının açıkça seçtiği dosyalarla etkileşime girer; bunlar şunları içerir:

- **Altyazı dosyaları**
  - Örnekler: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Kullanımlar:
    - Uygulama içinde altyazı oynatma
    - Altyazı düzenleme
    - Katman altyazısı gösterimi
    - Altyazı dönüştürme ve dışa aktarma

- **Medya dosyaları**
  - Örnekler: kullanıcının seçtiği yerel video veya ses dosyaları
  - Kullanımlar:
    - Video + altyazı oynatma
    - Katman zamanlamasının o anda oynatılan medya ile hizalanması

Önemli noktalar:

- Kullanıcının seçtiği dosyalar cihaz üzerinde yerel olarak işlenir.
- Uygulama bu dosyaları geliştiricinin kendi sunucularına yüklemez.
- Dosya yolları ve içerikleri yalnızca oynatma, katman, düzenleme, kaydetme ve kullanıcının talep ettiği işlemler için kullanılır.

### 2-2) Yerel Ayarlar ve Saklanan Değerler

Kalıcı ayarlar sağlamak ve önceki durumu geri yüklemek için uygulama, bazı değerleri cihaz üzerinde `SharedPreferences` veya işletim sistemi tarafından sağlanan benzer yerel depolama yöntemleriyle yerel olarak saklar.

Bu değerler geliştiricinin kendi sunucularına gönderilmez ve genellikle uygulama verileri temizlendiğinde veya uygulama kaldırıldığında silinir.

#### (1) Katman ayarları

Örnekler şunları içerir:

- `overlay_box_x`
- `overlay_box_y`
- `overlay_text_font`
- `overlay_text_color`
- `overlay_outline_enabled`
- `overlay_outline_color`
- `overlay_outline_width`
- `overlay_force_landscape`
- `overlay_interstitial_count`

Amaç:

- Katman konumunu geri yüklemek
- Katman ve uygulama içi altyazı oynatma için altyazı stilini geri yüklemek
- Kenarlık / yazı tipi / yön tercihlerini korumak
- Bazı katmanla ilgili akışlarda reklam gösterim sıklığı mantığını kontrol etmek

#### (2) Son oynatma veya katman konumları

Örnekler şunları içerir:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Amaç:

- Son altyazı/katman başlangıç konumlarını geri yüklemek veya önermek
- Video + altyazı oynatmayı daha rahat sürdürmek

#### (3) Reklam ve gizlilik tercih değerleri

Örnekler şunları içerebilir:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Amaç:

- Reklam gizlilik tercihlerini saklamak
- UMP / AdMob gizlilik ve reklam yapılandırma ayarlarını uygulamak

#### (4) Kullanıcı tarafından oluşturulan altyazı çıktısı

Kullanıcı altyazı dosyalarını kaydettiğinde veya dışa aktardığında, uygulama yeni altyazı dosyalarını kullanıcının seçtiği bir konuma yazabilir; örneğin:

- İndirilenler
- Sistem seçicisi üzerinden seçilen başka bir klasör
- Kullanıcının yönettiği bir depolama konumu

Kullanıcının kaydettiği bu dosyalar, kullanıcı bunları manuel olarak silmedikçe uygulama silindikten sonra da cihazda kalabilir.

#### (5) Geçici dosyalar ve önbellekler

Uygulama ve üçüncü taraf kütüphaneler, normal çalışma için geçici dosyalar veya önbellek dosyaları oluşturabilir; örneğin:

- dosya seçici önbellek verileri
- geçici altyazı dönüştürme verileri
- oynatmayla ilgili önbellek verileri

Bunlar yalnızca yerel çalışma amacıyla kullanılır ve geliştiricinin kendi sunucularına yüklenmez.

#### (6) UMP onay durumu önbelleği

Google UMP'nin geçerli olduğu bölgelerde SDK, onay durumunu cihaz üzerinde yerel olarak önbelleğe alabilir.

Bu genellikle şu yollarla sıfırlanabilir:

- uygulama verilerini temizlemek, veya
- uygulama içinde gizlilik seçenekleri girişi mevcutsa onay tercihlerini değiştirmek

### 2-3) Android Katmanı ve İzinlerle İlgili İşleme

Android'de kayan altyazı katmanı şunları kullanabilir:

- `SYSTEM_ALERT_WINDOW` / diğer uygulamaların üzerinde gösterme izni
- `POST_NOTIFICATIONS` izni
- katman hizmeti için gerekli bir foreground service bildirimi

Amaç:

- altyazı katmanını diğer uygulamaların üzerinde göstermek
- katman hizmetinin çalışmasını sürdürmek
- Android'in gerekli katman / hizmet bildirimlerini göstermesine olanak tanımak
- altyazı ilerleme desteği gerektiğinde medya bildirimi bilgilerini okumak

Bu izinler yalnızca kullanıcının kullanmayı seçtiği uygulama özellikleri için kullanılır.

### 2-4) Reklamlar, Onay ve İlgili Veriler (Üçüncü Taraf SDK'lar)

Uygulama aşağıdakiler dahil Google reklam / onay SDK'larını kullanır:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

Uygulama şunları gösterebilir:

- banner reklamlar
- geçiş reklamları
- ödüllü veya ödüllü geçiş reklamları

Bu SDK'lar şu tür verileri işleyebilir:

- reklam tanımlayıcıları (örneğin, geçerli olduğunda AAID / IDFA)
- IP tabanlı ve ağla ilgili bilgiler
- cihaz ve uygulama meta verileri
- reklam etkileşim sinyalleri
- onay tercihleri

Amaçlar şunları içerebilir:

- reklam sunumu
- reklam ölçümü ve raporlama
- sıklık sınırlaması
- dolandırıcılığın önlenmesi
- yasal uyumluluk

Geliştirici, bu SDK'ları kullanıcının onay tercihleri ve yürürlükteki hukuka uygun şekilde yapılandırmayı amaçlar.

---

## 3. Verileri Nasıl İşliyor ve Saklıyoruz

- **Yerel ayarlar ve son konum verileri**
  - uygulama verileri temizlenene veya uygulama kaldırılana kadar cihazda saklanır

- **Geçici dosyalar / önbellek**
  - çalışma için gerektiği sürece saklanır, ardından mümkün olduğu ölçüde uygulama tarafından kaldırılır veya daha sonra işletim sistemi tarafından temizlenir

- **Kullanıcının kaydettiği altyazı dosyaları**
  - kullanıcı tarafından silinene kadar kullanıcının seçtiği kayıt konumunda kalır

- **Üçüncü taraflarca işlenen reklam / onay verileri**
  - Google politikalarına ve yürürlükteki hukuka uygun olarak saklanır

---

## 4. Üçüncü Taraf İşleme ve Sınır Ötesi Aktarımlar

Reklam ve onay yönetimi için bazı bilgiler Google ve ilgili iş ortakları tarafından işlenebilir.

| Öğe | Ayrıntılar |
|---|---|
| Alıcı | Google LLC ve ilgili bağlı kuruluşlar / işleyiciler |
| Amaç | Reklam sunumu, ölçüm, dolandırıcılığın önlenmesi, onay yönetimi ve yasal uyumluluk |
| Olası veriler | Reklam tanımlayıcıları, cihaz/uygulama bilgileri, IP tabanlı bilgiler, reklam etkileşim verileri, onay durumu |
| Hedef | Google altyapısının faaliyet gösterdiği Amerika Birleşik Devletleri ve diğer bölgeler |
| Saklama | Google politikalarına ve yürürlükteki hukuka uygun olarak |

Geliştirici, uygulama mağazası gizlilik açıklamalarını gerçek SDK davranışıyla tutarlı tutmayı amaçlar.

---

## 5. Haklarınız ve Seçenekleriniz

Yargı bölgenize bağlı olarak şu haklara sahip olabilirsiniz:

- erişim
- düzeltme
- silme
- kısıtlama
- taşınabilirlik
- itiraz
- onayın yasal dayanak olduğu durumlarda onayı geri çekme

Uygulanabilir pratik kontroller şunları içerir:

- mevcut olduğu durumlarda uygulama içinde reklam / gizlilik tercihlerini değiştirmek
- yerel ayarları ve önbelleğe alınmış tercihleri kaldırmak için uygulama verilerini temizlemek
- uygulamayı kaldırmak
- dışa aktarılan altyazı dosyalarını kullanıcı depolamasından manuel olarak silmek
- bildirim ayarları, reklam kimliği sıfırlama veya reklam kişiselleştirme ayarları gibi işletim sistemi düzeyindeki kontrolleri kullanmak

Google tarafından işlenen veriler için kullanıcıların, ilgili olduğu durumlarda Google'ın kendi gizlilik ve hesap araçlarına da başvurması gerekir.

---

## 6. Çocukların Gizliliği

Bu uygulama öncelikli olarak çocuklara yönelik değildir.

Temel amacı altyazı oynatma, düzenleme, katman gösterimi ve ilgili yardımcı işlevlerdir. Uygun olduğunda, reklam SDK yapılandırması platform gereklilikleri ve geliştirici ayarlarıyla tutarlı biçimde yaşla ilgili veya çocuklara yönelik işaretler uygulayabilir.

---

## 7. Güvenlik Önlemleri

Uygulamanın mimarisinin sınırları içinde geliştirici şunları amaçlar:

- altyazı ve medya işlemenin çoğunu cihaz üzerinde tutarak veri toplamayı en aza indirmek
- sistem dosya seçicilerini ve kullanıcı tarafından başlatılan dosya erişimini kullanmak
- sistem izinlerini şeffaf biçimde kullanmak
- uygun olduğu durumlarda üçüncü taraf SDK'lar tarafından kullanılan şifreli ağ aktarımına dayanmak

Hiçbir depolama veya iletim yöntemi tamamen güvenli değildir, ancak uygulama geliştirici tarafından gereksiz veri toplanmasını önleyecek şekilde tasarlanmıştır.

---

## 8. Açık Kaynak Yazılım

Uygulama, aşağıdakilerle ilgili kütüphaneler dahil açık kaynak yazılımlar kullanır:

- altyazı ayrıştırma ve serileştirme
- dosya seçme
- yerel tercihler
- katman pencereleri
- video oynatma
- WebView

Açık kaynak bildirimleri uygulama içinde mevcuttur. Bazı bileşenler için uygulama, orijinal lisans bildirimini koruyarak açık kaynaklı bir paketin yerel olarak değiştirilmiş kopyasını kullanabilir.

---

## 9. İletişim

Gizlilikle ilgili sorularınız veya talepleriniz varsa:

- **E-posta:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Lütfen mesajınıza uygulama adı olan **Subtitle Player & Editor** bilgisini ekleyin.

---

## 10. Bu Politikadaki Değişiklikler

Bu Politika şu durumlarda güncellenebilir:

- uygulama özellikleri değişirse
- izinler veya SDK kullanımı değişirse
- yasal veya platform gereklilikleri değişirse

Önemli değişiklikler güncellenmiş politika sayfasına ve uygun olduğunda uygulama içine yansıtılacaktır.

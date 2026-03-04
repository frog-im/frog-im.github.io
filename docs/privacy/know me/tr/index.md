---
title: Gizlilik Politikası | know_me
description: know_me (PeopleNote, Memory for People) Gizlilik Politikası (Türkçe)
---

# Gizlilik Politikası (know_me / PeopleNote, Memory for People)

- **Uygulama Adı:** know_me (PeopleNote, Memory for People)
- **Geliştirici:** frog-im
- **Kişisel Verilerin Korunmasından Sorumlu Kişi / İrtibat Kişisi:** frog-im
- **İletişim:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Yürürlük Tarihi:** 2026-03-04
- **Son Güncelleme Tarihi:** 2026-03-04

> Bu Politika, uygulama tarafından işlenen bilgiler ve ilgili özellikler esas alınarak hazırlanmıştır.  
> Belirli bir ülke veya bölgede uygulanması zorunlu olan kanunlar ya da düzenlemeler varsa, söz konusu kanunlar veya düzenlemeler öncelikli olarak uygulanabilir.

---

## 1. Amaç ve Kapsam

`know_me`, kullanıcıların kişiler hakkında bilgi kaydetmesine ve bu bilgileri yönetmesine yardımcı olmak; gerektiğinde ise bu bilgileri yedeklemek, geri yüklemek ve PDF dosyaları olarak paylaşmak amacıyla tasarlanmış bir uygulamadır.

Başlıca özellikleri şunlardır:

- Kişiye özel bilgilerin saklanması (ad, tanımlayıcı metin, notlar, kişilik özellikleri, ülke, cinsiyet, iletişim bilgileri vb.)
- Klasör sınıflandırma, arama ve birleştirme işlevleri
- Fotoğraf ekleme ve açıklama yönetimi
- Yedeklerin (`.knm`) dışa aktarılması ve içe aktarılması
- PDF dışa aktarma
- Uygulama kilidi (şifre / desen)
- Reklam ve onay yönetimi (AdMob / UMP)

Uygulama, ayrı bir hesap kaydı gerektirmez ve uygulamanın temel kullanıcı verileri genel olarak kullanıcının cihazında yerel olarak saklanır.  
Bununla birlikte, reklam ve onay yönetimi amacıyla dâhil edilen bazı üçüncü taraf SDK'lar belirli bilgileri işleyebilir.

---

## 2. İşlenen Kişisel Veri Kategorileri

### 2-1) Kullanıcı Tarafından Doğrudan Girilen Bilgiler

Aşağıdaki bilgiler yalnızca kullanıcı tarafından doğrudan girildiğinde saklanır:

- Ad
- Tanımlayıcı metin (örneğin not metni olarak kullanılan görünüm / özellikler)
- Notlar
- Kişilik özellikleri, ülke, cinsiyet
- Telefon numarası
- Görünme zamanı / karşılaşma zamanı ile ilgili metin
- Platform / site bilgileri
- Klasör adı / rengi
- Görsel açıklaması (caption)

### 2-2) Cihaz Üzerinde Seçilen Dosyalar

- Fotoğraf eklenirken kullanıcı tarafından seçilen görsel dosyaları
- Yedek içe aktarılırken kullanıcı tarafından seçilen `.knm` yedek dosyaları
- PDF / yedek dışa aktarılırken kullanıcı tarafından seçilen kayıt yolları ve kaydedilen dosyalar

### 2-3) Uygulama İçinde Yerel Olarak Saklanan Veriler

Uygulama özelliklerinin sunulabilmesi için aşağıdaki veriler kullanıcının cihazında saklanabilir:

- SQLite veritabanı (`people_note.db`): kişiler / klasörler / platformlar / siteler / görsellerle ilgili meta veriler
- Görsel dosyaları: şifrelenmiş olarak uygulamanın belge klasöründe saklanır (`.enc`)
- Uygulama ayarları (`SharedPreferences`): tema, sıralama, gizlilik / reklam seçenekleri, PDF maskeleme seçenekleri, uygulama kilidi politikaları vb.
- Uygulama kilidi bilgileri: şifre / desen için hash değerleri ve salt değerleri (`SharedPreferences`)
- Yerel şifreleme anahtarları: `flutter_secure_storage` içinde saklanır
- Geçici dosyalar: görsel şifre çözme önizlemeleri, içe aktarma / dışa aktarma önbellek dosyaları vb. (geçici klasör)

### 2-4) Reklam ve Onay Yönetimi Sırasında Otomatik Olarak İşlenebilecek Bilgiler

Reklam veya onay yönetimi özellikleri etkin olduğunda, Google LLC ve ilgili iş ortaklarının SDK'ları (örneğin AdMob ve UMP) aşağıdaki bilgileri otomatik olarak işleyebilir:

- Reklam tanımlayıcıları (AAID / IDFA vb.)
- IP adresi ve ağ bilgileri
- Cihaz bilgileri (işletim sistemi sürümü, cihaz modeli, uygulama sürümü vb.)
- Reklam etkileşim bilgileri (gösterimler, tıklamalar vb.)
- Onay durumu ve gizlilik tercih bilgileri
- Tanılama, performans ve güvenlikle ilgili bilgiler

Uygulamanın temel kullanıcı kayıtları genel olarak geliştiricinin sunucusuna yüklenmez; ancak reklam / onay özellikleri kullanımdayken yukarıdaki bilgilerin bir kısmı üçüncü taraf hizmetlere aktarılabilir.

---

## 3. Kişisel Verilerin İşlenme Amaçları

Uygulama, kişisel verileri veya ilgili bilgileri aşağıdaki amaçlarla işler:

- İletişim / not odaklı kişi bilgilerinin kaydedilmesi ve görüntülenmesi
- Klasör sınıflandırma, arama ve birleştirme gibi düzenleme özelliklerinin sağlanması
- Fotoğraf eklenmesi ve görüntülenmesi
- Yedekleme / geri yükleme ve PDF dışa aktarma gibi kullanıcı tarafından talep edilen işlevlerin yerine getirilmesi
- Uygulama kilidi güvenlik özelliklerinin sağlanması
- Reklam sunulması, onay yönetimi, hileli faaliyetlerin önlenmesi ve yasal yükümlülüklere uyulması

---

## 4. Kişisel Verilerin Saklama ve Muhafaza Süresi

- Uygulama içi veriler (SQLite, yerel ayarlar, şifrelenmiş görseller): uygulama silinene, uygulama verileri temizlenene veya kullanıcı verileri doğrudan silene kadar kullanıcının cihazında tutulur
- Geçici dosyalar: ilgili işlem tamamlandıktan sonra silinir veya işletim sisteminin önbellek politikasına göre temizlenir
- Kullanıcı tarafından dışa aktarılan dosyalar (PDF'ler, yedek dosyaları): kullanıcının seçtiği depolama konumunda kalabilir ve kullanıcı tarafından doğrudan silinmelidir
- Reklam / onay ile ilgili veriler (üçüncü taraflarca işlenen): her hizmet sağlayıcının politikalarına ve yürürlükteki yasalara tabidir

İlke olarak, uygulama temel kullanıcı kayıtlarını geliştiricinin sunucusunda saklamaz.  
Bununla birlikte, kullanıcının doğrudan harici depolamaya kaydettiği dosyalar kullanıcının kendi ortamında yönetilir.

---

## 5. Kişisel Verilerin Silinmesine İlişkin Prosedürler ve Yöntemler

İşleme amacı yerine getirildiğinde veya kullanıcı silme talebinde bulunduğunda, uygulama ilgili bilgileri aşağıdaki şekilde siler ya da artık başvurulmayacak şekilde işler.

### 5-1) Silme Prosedürleri

- Kullanıcı tekil kişi kayıtlarını, klasörleri, görselleri, yedek verilerini vb. doğrudan sildiğinde, bu veriler derhâl silinecek veri olarak değerlendirilir.
- Kullanıcı uygulamayı sildiğinde veya cihaz ayarlarından uygulama verilerini temizlediğinde, uygulamanın dahili depolama alanında saklanan veriler işletim sisteminin silme prosedürlerine göre kaldırılır.
- Geçici dosyalar ilgili işlem tamamlandıktan sonra temizleme kapsamına alınır ve bazı önbellek verileri işletim sistemi politikasına bağlı olarak belirli bir süre daha kalabilir.

### 5-2) Silme Yöntemleri

- SQLite verileri: ilgili kayıtların silinmesi
- Uygulama ayarları (`SharedPreferences`): ilgili anahtarın veya tüm ayarların silinmesi
- `flutter_secure_storage` içindeki değerler: ilgili güvenli depolama öğelerinin silinmesi
- Uygulama içi dosyalar (şifrelenmiş görseller, geçici dosyalar vb.): ilgili dosyaların silinmesi
- Kullanıcının doğrudan harici depolamaya kaydettiği PDF / yedek dosyaları: uygulama tarafından otomatik olarak silinmez ve kullanıcı tarafından doğrudan silinmelidir

Yürürlükteki yasalar aksini gerektirmedikçe, geliştirici temel kullanıcı kayıtlarını geliştiricinin sunucusunda ayrıca saklamaz.

---

## 6. Üçüncü Taraflara Aktarım, Dış Kaynak Kullanımı ve Sınır Ötesi Aktarım

Uygulama, reklam ve onay yönetimi amacıyla Google hizmetlerini kullanabilir.

| Öğe | Ayrıntılar |
|---|---|
| **Alıcı / Yetkilendirilen Taraf** | Google LLC ve bağlı kuruluşları (AdMob / UMP işletmecileri) |
| **Aktarım Yapılan Ülke** | Amerika Birleşik Devletleri ve Google altyapısının işletildiği bölgeler |
| **Aktarım Zamanı** | Reklam talepleri, onay durumu kontrolleri, SDK başlatma ve işletim sırasında sürekli olarak |
| **Aktarım Yöntemi** | Uygulama ile üçüncü taraf sunucular arasındaki ağ iletişimi yoluyla aktarım |
| **Sınır Ötesi Aktarımın Hukuki Dayanağı** | Hizmetin sunulması için gerekli kapsamda yürürlükteki hukuki dayanaklar uyarınca işlenir veya gerekli hâllerde veri sahibinin açık rızasına dayanır |
| **Amaç** | Reklam sunumu, reklam ölçümü, onay yönetimi, dolandırıcılığın önlenmesi ve politika / yasalara uyum |
| **Veri Kategorileri (Örnekler)** | Reklam tanımlayıcıları (AAID / IDFA), IP / ağ bilgileri, cihaz / uygulama bilgileri, reklam etkileşim bilgileri, onay durumu |
| **Saklama Süresi** | Google politikalarına ve yürürlükteki yasalara tabidir |
| **Reddetmenin Etkisi** | Kişiselleştirilmiş reklamlar sınırlandırılabilir, kişiselleştirilmemiş reklamlar gösterilebilir veya bazı reklamla ilgili özellikler kısıtlanabilir |

Geliştirici, uygulamanın temel kişi kaydı verilerini kendi sunucusu aracılığıyla toplamaz veya satmaz.

---

## 7. Kullanılan İzinlere İlişkin Bilgiler

Uygulama aşağıdaki izinleri kullanabilir:

- `INTERNET`: reklam SDK'ları ve ilgili ağ özellikleri için iletişim
- `com.google.android.gms.permission.AD_ID`: reklam tanımlayıcılarının kullanımı (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 ve altı): fotoğraf ekleme / seçme

İzinler yalnızca ilgili özelliklerin sunulması için gerekli kapsamda kullanılır.

---

## 8. Otomatik Toplama Mekanizmalarının Kurulumu, İşletimi ve Reddedilmesi

Bu uygulama, genel web sitesi çerezlerini doğrudan kullanmaz.  
Bununla birlikte, reklam ve onay yönetimi özellikleriyle bağlantılı olarak üçüncü taraf SDK'lar reklam tanımlayıcılarını, ağ bilgilerini, cihaz bilgilerini ve benzer verileri otomatik olarak işleyebilir.

Kullanıcılar ilgili ayarları aşağıdaki şekillerde değiştirebilir:

- Uygulamanın gizlilik seçenekleri veya onay yönetimi ekranındaki seçimleri değiştirmek (sunuluyorsa)
- Cihaz işletim sistemi ayarlarında reklam tanımlayıcısını sıfırlamak veya silmek
- Cihaz işletim sistemi ayarlarında kişiselleştirilmiş reklamları sınırlamak veya ilgili gizlilik seçeneklerini ayarlamak

Kullanıcı kişiselleştirilmiş reklamları sınırlandırırsa, kişiselleştirilmemiş reklamlar gösterilebilir veya bazı reklamla ilgili özellikler kısıtlanabilir.

---

## 9. Kullanıcı Hakları ve Bunların Nasıl Kullanılacağı

Yürürlükteki yasalara tabi olarak, kullanıcılar aşağıdaki haklara sahip olabilir:

- Kişisel verilere erişim, düzeltme veya silme talebinde bulunmak
- İşlemenin durdurulmasını veya sınırlandırılmasını talep etmek
- Açık rızaya dayalı işleme için verilen onayı geri çekmek
- Reklam / onay tercihlerini değiştirmek

Bu haklar aşağıdaki yollarla kullanılabilir:

- Uygulama içinde verileri doğrudan değiştirmek veya silmek
- Uygulama verilerini silerek veya uygulamayı kaldırarak yerel verileri sıfırlamak
- Uygulamanın gizlilik seçenekleri / onay ekranı üzerinden reklam onayını değiştirmek (sunulduğu bölgelerde)
- Cihaz işletim sistemi ayarları üzerinden reklam tanımlayıcısını sıfırlamak / silmek veya kişiselleştirilmiş reklamları sınırlamak
- İletişim: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Güvenlik Önlemleri

Geliştirici aşağıdaki önlemleri uygular veya uygulamaya çalışır:

- Kullanıcı kayıtları genel olarak cihaz üzerinde yerel olarak saklanır
- Eklenen görsel dosyaları yerel olarak şifrelenmiş biçimde saklanır (AES-GCM tabanlı)
- Uygulama kilidi bilgileri düz metin yerine hash biçiminde saklanır
- Yedek dosyaları, kullanıcı parolasına dayalı olarak şifrelendikten sonra saklanır
- Üçüncü taraf SDK'larla iletişim şifrelenir (HTTPS / TLS)
- İzinler, asgari erişim kapsamıyla kullanılır

Bununla birlikte, kullanıcının cihaz güvenlik durumundan kaynaklanan riskler (örneğin root / jailbreak, kötü amaçlı uygulamalar veya paylaşılan depolamanın açığa çıkması) tamamen ortadan kaldırılamaz.

---

## 11. Hassas Bilgilere İlişkin Bilgilendirme

Bu uygulama hassas bilgilerin girilmesini gerektirmez.  
Kullanıcılara, notlara veya serbest giriş alanlarına sağlık bilgileri, siyasi görüşler, din, biyometrik bilgiler ya da cinsel yaşama ilişkin bilgiler gibi hassas içerikler girmemeleri tavsiye edilir.

Bir kullanıcı gönüllü olarak hassas içerik girerse, bu bilgiler kullanıcının doğrudan yönettiği cihaz üzerinde yerel veri olarak saklanabilir.

---

## 12. Çocukların Kişisel Verilerinin Korunması

Bu uygulama öncelikli olarak çocuklar için tasarlanmamıştır.  
Veliler, cihaz veya uygulama mağazası tarafından sağlanan ebeveyn kontrolü özellikleri aracılığıyla kullanımı yönetebilir.

---

## 13. Otomatik Karar Verme

Bu uygulama, kişisel verilere dayanarak hukuki sonuç doğuran veya benzer derecede önemli etkiler yaratan otomatik karar verme işlemleri gerçekleştirmez.

---

## 14. Veri Güvenliği Bildirimi (Google Play vb.)

Geliştirici, uygulama pazar yerlerinde (örneğin Google Play) yer alan veri güvenliği açıklamalarını, uygulamanın fiilî işleme uygulamalarına ve üçüncü taraf SDK'ların fiilî işleme uygulamalarına uygun şekilde korumaya ve güncellemeye çalışır.

Bununla birlikte, uygulama mağazalarında gösterilen bilgiler uygulama sürümüne, dağıtım ülkesine, üçüncü taraf SDK yapılandırmasına ve politika değişikliklerine bağlı olarak farklılık gösterebilir.

---

## 15. Açık Kaynak Bildirimi

Uygulama belirli açık kaynak kütüphaneler kullanır.  
İlgili lisanslara ilişkin bilgiler, uygulama içindeki ilgili ekranda veya dağıtım kanalı üzerinden sağlanan bildirimlerde bulunabilir.

---

## 16. İletişim

Bu Gizlilik Politikası ile ilgili sorular için:

- **Kişisel Verilerin Korunmasından Sorumlu Kişi / İrtibat Kişisi:** frog-im
- **E-posta:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 17. Bu Gizlilik Politikasındaki Değişiklikler

Bu Politika; yasa / politika, uygulama özellikleri veya üçüncü taraf SDK'lardaki değişiklikler nedeniyle revize edilebilir.  
Önemli değişiklikler olması hâlinde, uygulama içi bildirimler, dağıtım sayfası veya politika sayfasındaki güncellemeler aracılığıyla bildirim yapılabilir.

Son Güncelleme Tarihi: **2026-03-04**
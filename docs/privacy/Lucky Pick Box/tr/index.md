---
title: Gizlilik Politikası | Lucky Pick Box
description: Lucky Pick Box Gizlilik Politikası
lang: tr
last_updated: 2026-06-15
---

# Gizlilik Politikası (Lucky Pick Box / 뽑기박스)

- **Uygulama Adı:** Lucky Pick Box / 뽑기박스
- **Geliştirici:** frog-im
- **Kişisel Verilerin Korunmasından Sorumlu Kişi / İrtibat Kişisi:** frog-im
- **İletişim:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Yürürlük Tarihi:** 2026-06-12
- **Son Güncelleme Tarihi:** 2026-06-15

> Bu Politika, uygulama tarafından işlenen bilgiler ve ilgili özellikler esas alınarak hazırlanmıştır.  
> Belirli bir ülke veya bölgede uygulanması zorunlu olan kanunlar ya da düzenlemeler varsa, söz konusu kanunlar veya düzenlemeler öncelikli olarak uygulanabilir.

---

## 1. Amaç ve Kapsam

Lucky Pick Box rastgele seçimler, çekilişler, sıra belirleme, takım ayırma, zar, yazı tura, merdiven, çark ve benzer günlük veya grup karar oyunları için basit bir araçtır. Uygulama gerçek parayla kumar, bahis, finansal işlem, nakit ödül veya nakit eşdeğeri ödül sunmaz.

### A. Kapsanan ana özellikler

- Hızlı öğe girişi: kullanıcının yazdığı metin veya seçilen görüntüden okunan metin.
- Rastgele seçim oyunları: merdiven, çark, plinko, basit çekiliş, zar, yazı tura, rastgele sayı, takım ayırma, sıra seçme, kart, bomba ve evet/hayır.
- Sonuç geçmişi: oyun türü, başlık, katılımcılar/öğeler, sonuç özeti ve oluşturma zamanı saklanabilir.
- Ayar yuvaları: bazı oyunlar katılımcıları, listeleri, aralıkları, miktarları, takımları, ağırlıkları ve benzer ayarları en fazla 3 yerel yuvada saklayabilir.

Uygulama kayıt veya giriş gerektirmez. Uygulamadan adınızı, telefon numaranızı, e-posta adresinizi, kişilerinizi, oyun girdilerinizi, seçilen görüntüleri veya oyun sonuçlarını alan bir sunucu işletmiyoruz.

Uygulama özelliklerini sağlamak için oyun girdileri, katılımcı etiketleri, son sonuçlar, kaydedilmiş oyun ayarları, animasyon ayarları, reklam gizliliği seçimleri ve onayla ilgili durum cihazınızın yerel depolamasında saklanabilir. Sonuç geçmişi uygulama tarafından sınırlandırılır ve geliştirici tarafından işletilen bir sunucuya gönderilmez.

---

## 2. İşlenen Kişisel Veri Kategorileri

### 2-1) Kullanıcı Tarafından Doğrudan Girilen Bilgiler

Uygulama kayıt veya giriş gerektirmez. Uygulamadan adınızı, telefon numaranızı, e-posta adresinizi, kişilerinizi, oyun girdilerinizi, seçilen görüntüleri veya oyun sonuçlarını alan bir sunucu işletmiyoruz.

### 2-2) Cihaz Üzerinde Seçilen Dosyalar

Bir görüntüden metin okumayı seçerseniz uygulama fotoğraf kitaplığınızdan bir görüntü seçmenizi ister. Seçilen görüntü, platform görüntü seçicisi ve Google ML Kit metin tanıma bileşenleriyle cihaz üzerinde işlenir. Geliştirici görüntüyü kendi sunucusuna yüklemez ve uzak bir hesapta saklamaz.

### 2-3) Uygulama İçinde Yerel Olarak Saklanan Veriler

Uygulama özelliklerini sağlamak için oyun girdileri, katılımcı etiketleri, son sonuçlar, kaydedilmiş oyun ayarları, animasyon ayarları, reklam gizliliği seçimleri ve onayla ilgili durum cihazınızın yerel depolamasında saklanabilir. Sonuç geçmişi uygulama tarafından sınırlandırılır ve geliştirici tarafından işletilen bir sunucuya gönderilmez.

### B. Cihazdaki yerel veriler

| Konum veya anahtar | Veri | Amaç | Silme |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, oyun türü, başlık, katılımcılar/öğeler, özet, zaman; en fazla 50 sonuç. | Sonuçları ve geçmişi göstermek. | Uygulama içi silme, uygulama verilerini temizleme veya kaldırma |
| `game_settings.<gameId>.slot_<n>` | Oyun ayarları, kayıt zamanı, listeler, aralıklar, miktarlar, takımlar, ağırlıklar; en fazla 3 yuva. | Ayarları yeniden yüklemek. | Yuvayı boşaltma, veri temizleme veya kaldırma |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Animasyon ve tam ekran ayarları. | Görüntü tercihlerini korumak. | Ayar değiştirme, veri temizleme veya kaldırma |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Reklam gizlilik seçimleri ve reklam sıklığı sayacı. | Bölgesel seçimleri uygulamak ve sıklığı kontrol etmek. | Ayar değiştirme, veri temizleme veya kaldırma |
| Görüntü seçici ve OCR | Seçilen görüntü yolu ve tanınan metin geçici olarak işlenebilir. | Görüntü metnini hızlı girişe eklemek. | Uygulama/OS önbelleği veya veri temizleme |

Hızlı giriş metni geliştirici sunucusuna gönderilmez. Yalnızca oyun sonucunda veya kayıtlı ayarda kullanılırsa yerel veri olabilir.

### 2-4) Reklam ve Onay Yönetimi Sırasında Otomatik Olarak İşlenebilecek Bilgiler

Desteklenen platformlarda, şu anda Android'de, uygulama Google AdMob ve Google User Messaging Platform (UMP) kullanır. Google ve reklam ortakları reklam tanımlayıcıları, uygulama örneği tanımlayıcıları, IP adresi, yaklaşık konum, cihaz ve ağ bilgileri, uygulama sürümü, işletim sistemi, dil, reklam gösterimleri, tıklamalar ve etkileşimler, tanılama bilgileri, onay durumu ve bölgesel reklam gizliliği ayarlarını reklam sunumu, frekans sınırlama, dolandırıcılığı önleme, onay yönetimi, ölçüm, analiz, güvenlik ve yasal uyum için işleyebilir.

Google'ın gizlilik uygulamaları https://policies.google.com/privacy ve https://policies.google.com/technologies/ads adreslerinde açıklanmıştır.

---

## 3. Kişisel Verilerin İşlenme Amaçları

Lucky Pick Box rastgele seçimler, çekilişler, sıra belirleme, takım ayırma, zar, yazı tura, merdiven, çark ve benzer günlük veya grup karar oyunları için basit bir araçtır. Uygulama gerçek parayla kumar, bahis, finansal işlem, nakit ödül veya nakit eşdeğeri ödül sunmaz.

### A. Kapsanan ana özellikler

- Hızlı öğe girişi: kullanıcının yazdığı metin veya seçilen görüntüden okunan metin.
- Rastgele seçim oyunları: merdiven, çark, plinko, basit çekiliş, zar, yazı tura, rastgele sayı, takım ayırma, sıra seçme, kart, bomba ve evet/hayır.
- Sonuç geçmişi: oyun türü, başlık, katılımcılar/öğeler, sonuç özeti ve oluşturma zamanı saklanabilir.
- Ayar yuvaları: bazı oyunlar katılımcıları, listeleri, aralıkları, miktarları, takımları, ağırlıkları ve benzer ayarları en fazla 3 yerel yuvada saklayabilir.

Desteklenen platformlarda, şu anda Android'de, uygulama Google AdMob ve Google User Messaging Platform (UMP) kullanır. Google ve reklam ortakları reklam tanımlayıcıları, uygulama örneği tanımlayıcıları, IP adresi, yaklaşık konum, cihaz ve ağ bilgileri, uygulama sürümü, işletim sistemi, dil, reklam gösterimleri, tıklamalar ve etkileşimler, tanılama bilgileri, onay durumu ve bölgesel reklam gizliliği ayarlarını reklam sunumu, frekans sınırlama, dolandırıcılığı önleme, onay yönetimi, ölçüm, analiz, güvenlik ve yasal uyum için işleyebilir.

Google'ın gizlilik uygulamaları https://policies.google.com/privacy ve https://policies.google.com/technologies/ads adreslerinde açıklanmıştır.

---

## 4. Kişisel Verilerin Saklama ve Muhafaza Süresi

Yerel geçmiş ve ayarlar, geçmişi silene, uygulama verilerini temizleyene veya uygulamayı kaldırana kadar cihazınızda kalabilir. Geçerli olduğu yerlerde uygulama ayarlarında reklam gizliliği seçimlerini değiştirebilir, gerektiğinde Google gizlilik seçeneklerini açabilir ve cihaz gizlilik ayarlarında reklam tanımlayıcılarını yönetebilir veya sıfırlayabilirsiniz. Google tarafından işlenen bilgilerin saklanması Google politikaları ve yasal yükümlülükleriyle yönetilir.

### B. Cihazdaki yerel veriler

| Konum veya anahtar | Veri | Amaç | Silme |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, oyun türü, başlık, katılımcılar/öğeler, özet, zaman; en fazla 50 sonuç. | Sonuçları ve geçmişi göstermek. | Uygulama içi silme, uygulama verilerini temizleme veya kaldırma |
| `game_settings.<gameId>.slot_<n>` | Oyun ayarları, kayıt zamanı, listeler, aralıklar, miktarlar, takımlar, ağırlıklar; en fazla 3 yuva. | Ayarları yeniden yüklemek. | Yuvayı boşaltma, veri temizleme veya kaldırma |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Animasyon ve tam ekran ayarları. | Görüntü tercihlerini korumak. | Ayar değiştirme, veri temizleme veya kaldırma |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Reklam gizlilik seçimleri ve reklam sıklığı sayacı. | Bölgesel seçimleri uygulamak ve sıklığı kontrol etmek. | Ayar değiştirme, veri temizleme veya kaldırma |
| Görüntü seçici ve OCR | Seçilen görüntü yolu ve tanınan metin geçici olarak işlenebilir. | Görüntü metnini hızlı girişe eklemek. | Uygulama/OS önbelleği veya veri temizleme |

Hızlı giriş metni geliştirici sunucusuna gönderilmez. Yalnızca oyun sonucunda veya kayıtlı ayarda kullanılırsa yerel veri olabilir.

---

## 5. Kişisel Verilerin Silinmesine İlişkin Prosedürler ve Yöntemler

Yerel geçmiş ve ayarlar, geçmişi silene, uygulama verilerini temizleyene veya uygulamayı kaldırana kadar cihazınızda kalabilir. Geçerli olduğu yerlerde uygulama ayarlarında reklam gizliliği seçimlerini değiştirebilir, gerektiğinde Google gizlilik seçeneklerini açabilir ve cihaz gizlilik ayarlarında reklam tanımlayıcılarını yönetebilir veya sıfırlayabilirsiniz. Google tarafından işlenen bilgilerin saklanması Google politikaları ve yasal yükümlülükleriyle yönetilir.

### C. İzinler, SDK'lar, yedekler ve güvenlik

Uygulama reklamlar ve yasal bildirimler için `INTERNET`, `ACCESS_NETWORK_STATE` ve `com.google.android.gms.permission.AD_ID` kullanabilir. Fotoğraf erişimi veya görüntü seçici yalnızca kullanıcı görüntüden metin okumayı seçtiğinde kullanılır.

Google Mobile Ads SDK reklam, analiz ve dolandırıcılık önleme için IP adresi, reklam etkileşimleri, tanılama ve cihaz/hesap tanımlayıcılarını işleyebilir. UMP onay durumunu ve gizlilik seçimlerini işleyebilir.

Yerel veriler uygulama içi silme, işletim sistemi uygulama verisi silme veya kaldırma yoluyla silinebilir. Sistem yedekleri, ekran görüntüleri veya kullanıcının paylaştığı dosyalar sağlayıcı politikalarına göre kalabilir. Serbest metin alanlarına hassas bilgi girmeyin.

---

## 6. Üçüncü Taraflara Aktarım, Dış Kaynak Kullanımı ve Sınır Ötesi Aktarım

Oyun girdilerinizi, katılımcı etiketlerinizi, oyun sonuçlarınızı veya seçilen görüntülerinizi satmayız. Reklam veya onay özellikleri istendiğinde Google LLC, Google iştirakleri ve hizmet sağlayıcıları reklam ve onay bilgilerini ülkeniz veya bölgeniz dışında işleyebilir. Ayrıntılar için uygulamadaki "Uluslararası Veri Aktarımı Bildirimi"ne bakın.

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

---

## 7. Kullanılan İzinlere İlişkin Bilgiler

### C. İzinler, SDK'lar, yedekler ve güvenlik

Uygulama reklamlar ve yasal bildirimler için `INTERNET`, `ACCESS_NETWORK_STATE` ve `com.google.android.gms.permission.AD_ID` kullanabilir. Fotoğraf erişimi veya görüntü seçici yalnızca kullanıcı görüntüden metin okumayı seçtiğinde kullanılır.

Google Mobile Ads SDK reklam, analiz ve dolandırıcılık önleme için IP adresi, reklam etkileşimleri, tanılama ve cihaz/hesap tanımlayıcılarını işleyebilir. UMP onay durumunu ve gizlilik seçimlerini işleyebilir.

Yerel veriler uygulama içi silme, işletim sistemi uygulama verisi silme veya kaldırma yoluyla silinebilir. Sistem yedekleri, ekran görüntüleri veya kullanıcının paylaştığı dosyalar sağlayıcı politikalarına göre kalabilir. Serbest metin alanlarına hassas bilgi girmeyin.

---

## 8. Otomatik Toplama Mekanizmalarının Kurulumu, İşletimi ve Reddedilmesi

Desteklenen platformlarda, şu anda Android'de, uygulama Google AdMob ve Google User Messaging Platform (UMP) kullanır. Google ve reklam ortakları reklam tanımlayıcıları, uygulama örneği tanımlayıcıları, IP adresi, yaklaşık konum, cihaz ve ağ bilgileri, uygulama sürümü, işletim sistemi, dil, reklam gösterimleri, tıklamalar ve etkileşimler, tanılama bilgileri, onay durumu ve bölgesel reklam gizliliği ayarlarını reklam sunumu, frekans sınırlama, dolandırıcılığı önleme, onay yönetimi, ölçüm, analiz, güvenlik ve yasal uyum için işleyebilir.

Google'ın gizlilik uygulamaları https://policies.google.com/privacy ve https://policies.google.com/technologies/ads adreslerinde açıklanmıştır.

Yerel geçmiş ve ayarlar, geçmişi silene, uygulama verilerini temizleyene veya uygulamayı kaldırana kadar cihazınızda kalabilir. Geçerli olduğu yerlerde uygulama ayarlarında reklam gizliliği seçimlerini değiştirebilir, gerektiğinde Google gizlilik seçeneklerini açabilir ve cihaz gizlilik ayarlarında reklam tanımlayıcılarını yönetebilir veya sıfırlayabilirsiniz. Google tarafından işlenen bilgilerin saklanması Google politikaları ve yasal yükümlülükleriyle yönetilir.

---

## 9. Kullanıcı Hakları ve Bunların Nasıl Kullanılacağı

Yerel geçmiş ve ayarlar, geçmişi silene, uygulama verilerini temizleyene veya uygulamayı kaldırana kadar cihazınızda kalabilir. Geçerli olduğu yerlerde uygulama ayarlarında reklam gizliliği seçimlerini değiştirebilir, gerektiğinde Google gizlilik seçeneklerini açabilir ve cihaz gizlilik ayarlarında reklam tanımlayıcılarını yönetebilir veya sıfırlayabilirsiniz. Google tarafından işlenen bilgilerin saklanması Google politikaları ve yasal yükümlülükleriyle yönetilir.

---

## 10. Güvenlik Önlemleri

### C. İzinler, SDK'lar, yedekler ve güvenlik

Uygulama reklamlar ve yasal bildirimler için `INTERNET`, `ACCESS_NETWORK_STATE` ve `com.google.android.gms.permission.AD_ID` kullanabilir. Fotoğraf erişimi veya görüntü seçici yalnızca kullanıcı görüntüden metin okumayı seçtiğinde kullanılır.

Google Mobile Ads SDK reklam, analiz ve dolandırıcılık önleme için IP adresi, reklam etkileşimleri, tanılama ve cihaz/hesap tanımlayıcılarını işleyebilir. UMP onay durumunu ve gizlilik seçimlerini işleyebilir.

Yerel veriler uygulama içi silme, işletim sistemi uygulama verisi silme veya kaldırma yoluyla silinebilir. Sistem yedekleri, ekran görüntüleri veya kullanıcının paylaştığı dosyalar sağlayıcı politikalarına göre kalabilir. Serbest metin alanlarına hassas bilgi girmeyin.

### C. İzinler, SDK'lar, yedekler ve güvenlik

Uygulama reklamlar ve yasal bildirimler için `INTERNET`, `ACCESS_NETWORK_STATE` ve `com.google.android.gms.permission.AD_ID` kullanabilir. Fotoğraf erişimi veya görüntü seçici yalnızca kullanıcı görüntüden metin okumayı seçtiğinde kullanılır.

Google Mobile Ads SDK reklam, analiz ve dolandırıcılık önleme için IP adresi, reklam etkileşimleri, tanılama ve cihaz/hesap tanımlayıcılarını işleyebilir. UMP onay durumunu ve gizlilik seçimlerini işleyebilir.

Yerel veriler uygulama içi silme, işletim sistemi uygulama verisi silme veya kaldırma yoluyla silinebilir. Sistem yedekleri, ekran görüntüleri veya kullanıcının paylaştığı dosyalar sağlayıcı politikalarına göre kalabilir. Serbest metin alanlarına hassas bilgi girmeyin.

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

Son Güncelleme Tarihi: **2026-06-15**

---
title: Gizlilik Politikası | Power lucky lotto
description: Power lucky lotto Gizlilik Politikası (Türkçe)
lang: tr
last_updated: 2026-01-29
---

# Gizlilik Politikası (Power lucky lotto)

- **Uygulama adı:** Power lucky lotto  
- **Geliştirici:** frog-im  
- **İletişim:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Yürürlük tarihi:** 2026-01-29  

> Bu politika; Kore PIPA, GDPR/UK GDPR, İsviçre FADP ve ilgili ABD eyalet gizlilik yasaları gibi uygulanabilir mevzuatlar dikkate alınarak hazırlanmıştır.  
> Bölgenizde zorunlu özel gereklilikler varsa, öncelik bu gerekliliklerdedir.

---

## 1. Amaç ve kapsam

Power lucky lotto, piyango oyunlarını yönetmek ve kayıtları görüntülemek için bir uygulamadır. Başlıca özellikler:

- Ülke/oyun seçimi ve kurulum (ör. KR 6/45, US Powerball)  
- Numara üretme/kaydetme ve log (geçmiş) görüntüleme  
- Log tablolarını görüntüleme ve silme (tablo listesi/detay)  
- İstatistik/görselleştirme için JSON üzerinden oyun sonuç verilerini düzenleme/yönetme  
- Reklamlar (ödüllü reklamlar dahil) ve gerektiğinde onay (consent) yönetimi

Uygulama **hesap oluşturmayı gerektirmez** ve varsayılan olarak **verilerinizi geliştiricinin sunucularına yüklemez.**  
İşlemlerin çoğu **cihazınızda** gerçekleşir.

Ancak **reklam**, **onay yönetimi** ve **yasal uyumluluk** için  
**Google Mobile Ads SDK (AdMob)** ve **Google UMP (User Messaging Platform)** gibi üçüncü taraf SDK’lar, belirli verileri (ör. reklam tanımlayıcıları) toplayıp işleyebilir.

---

## 2. İşlenen veri türleri

### 2-1) Cihazınızda saklanan veriler (yerel depolama)

Uygulama, özellikleri sağlamak ve kullanılabilirliği artırmak için bazı verileri **cihazınızda yerel olarak** saklar.  
Bu veriler genellikle **geliştirici sunucularına iletilmez** ve uygulama verilerini sildiğinizde veya uygulamayı kaldırdığınızda silinir (başka yere dışa aktardığınız dosyalar hariç).

[Local Settings and Stored Values](https://frog-im.github.io/privacy/Power%20lucky%20lotto/en/local/)

### 2-2) Reklam, onay ve ilgili veriler (üçüncü taraf SDK’lar)

Uygulama, **Google Mobile Ads SDK (AdMob)** ve **Google UMP** kullanarak:

- Reklam gösterir ( **ödüllü reklamlar** dahil )  
- Reklamcılık için yasal olarak gerekli onayı yönetir

Bu SDK’lar örneğin şunları toplayıp/işleyebilir:

- **Reklam Kimliği** (ör. AAID, IDFA)  
- IP tabanlı bilgiler, yaklaşık konum, ağ bilgileri  
- Cihaz/uygulama bilgileri (OS sürümü, uygulama sürümü, dil, teşhis bilgileri)  
- Reklam etkileşimleri (gösterim, tıklama, ödül tamamlanması)  
- UMP ile kaydedilen onay tercihleri

Bazı bölgelerde (ör. EEA/UK/CH) UMP onay formu gösterilebilir ve gerektiğinde **Privacy Options** girişi sağlanabilir.

---

## 3. Saklama süresi

- **Yerel ayarlar (SharedPreferences):** uygulama verisi silinene veya uygulama kaldırılana kadar  
- **Log verileri (SQLite):** siz silene kadar veya uygulamayı kaldırıp/veriyi temizleyene kadar  
- **JSON dosyaları:** uygulama doküman dizininde saklanır; çoğu durumda kaldırmada silinir, ancak dışa aktarma/yedekler kullanıcı tarafından yönetilir  
- **Reklam/onay verileri (üçüncü taraf):** Google politikaları ve uygulanabilir yasalara göre saklanır

---

## 4. Üçüncü taraf paylaşımı ve uluslararası aktarım

Reklam ve onay yönetimi için bazı veriler **Google ve iş ortakları** tarafından işlenebilir.

| Öğeler | Detaylar |
|---|---|
| **Alıcılar** | Google LLC, bağlı kuruluşlar ve alt işleyiciler |
| **Aktarım hedefleri** | ABD ve Google altyapısının bulunduğu diğer bölgeler |
| **Amaç** | Reklam sunumu, ölçüm, sahtekarlık önleme, onay yönetimi, uyum |
| **Veriler** | Reklam Kimliği, IP tabanlı bilgi, cihaz/uygulama bilgisi, reklam etkileşim verileri, onay durumu |
| **Saklama** | Google politikaları ve uygulanabilir yasalara göre |
| **Reddederseniz etkisi** | Kişiselleştirilmiş reklamlar sınırlanabilir; kişiselleştirilmemiş reklamlar veya daha az reklam gösterilebilir |

---

## 5. Haklarınız ve kullanma yöntemleri

Uygulanabilir yasalara bağlı olarak erişim, düzeltme, silme, kısıtlama, itiraz, taşınabilirlik ve (onayın hukuki dayanak olduğu durumlarda) onayı geri çekme gibi haklarınız olabilir.

Örnekler:

- **Reklam/onay tercihlerini ayarlama:** uygulama içi Privacy Options (varsa) veya OS reklam ayarları (reklam kimliğini sıfırlama, kişiselleştirmeyi sınırlama) üzerinden.  
- **Yerel verileri sıfırlama:** uygulama verisini temizleyin veya uygulamayı kaldırın.

---

## 6. Çocukların gizliliği

Bu uygulama **çocuklar için tasarlanmamıştır**. Bir çocuk kullanıyorsa, veli OS düzeyindeki ebeveyn kontrolleri ve reklam sınırlama özelliklerini kullanmayı değerlendirmelidir.

---

## 7. Güvenlik önlemleri

Uygulama kapsamı içinde:

- Gerekli minimum veriyi yerel olarak saklamaya  
- Mümkün olduğunda işlemleri cihaz üzerinde tutmaya  
- SDK ağ iletişimi için TLS/güvenli aktarımı kullanmaya (SDK kabiliyetleri dahilinde) çalışırız

---

## 8. Google Play Data safety

Google Play’de dağıtılırsa, özellikle SDK’lar veya işleme uygulamaları değiştiğinde Data safety beyanlarının doğru ve güncel olmasını hedefleriz.

---

## 9. Açık kaynak bildirimleri

Uygulama; ülke ikonları, depolama, reklam/onay ve UI için açık kaynak kütüphaneler kullanabilir.  
Lisans bildirimleri uygulama içindeki “Open-source licenses” (veya eşdeğeri) ekranda bulunur.

---

## 10. İletişim

Gizlilik soruları için:

- **E-posta:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Lütfen mesajınızda **“Power lucky lotto”** belirtin.

---

## 11. Politika değişiklikleri

Bu politika; yasal güncellemeler, özellik değişiklikleri (ör. yeni SDK’lar) veya iç politika düzenlemeleri nedeniyle değişebilir.  
Küçük değişiklikler uygulama içinde veya bu sayfada yayınlanır; önemli değişiklikler gereken şekilde önceden duyurulur.

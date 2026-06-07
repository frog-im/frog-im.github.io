---
title: Gizlilik Politikası | TimeBack
description: TimeBack Gizlilik Politikası
lang: tr
last_updated: 2026-06-06
---

# Gizlilik Politikası (TimeBack)

- **Uygulama adı:** TimeBack
- **Geliştirici:** frog-im
- **İletişim:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Geçerlilik tarihi:** 03.06.2026
- **Son güncelleme:** 2026-06-06

Bu Gizlilik Politikası, TimeBack uygulamasının mevcut uygulamasını temel almaktadır. TimeBack, ekran süresini inceleme, günlük hedefler, geri kazanılan zaman kayıtları, yansımalar, zorluklar, bildirimler, paylaşım ve reklam özellikleri sağlar.

## 1. Özellikler

TimeBack aşağıdaki özellikleri sağlar:

- Android kullanım erişim izni aracılığıyla uygulama kullanım süresi incelemesi
- Günlük kullanım hedefleri, hatırlatıcılar ve durum çubuğu kullanım bildirimleri
- Kesin sınır uyarı bildirimleri ve yer paylaşımı ekranı
- Yer paylaşımı istisnası uygulama seçimi
- Geri kazanılan zaman etkinliği kayıtları
- Günlük yansıma kayıtları
- Mücadele ilerlemesi ve kontrol listesi yönetimi
- Kullanım istatistikleri görsel paylaşımı
- Google AdMob reklamları ve UMP tabanlı gizlilik seçenekleri

## 2. İşlediğimiz Bilgiler

### 2-1. Kullanım Erişim İzni Yoluyla Okunan Bilgiler

Kullanıcı Android `PACKAGE_USAGE_STATS` izni verirse uygulama, cihazdan aşağıdaki bilgileri okuyabilir:

- Uygulama paketi adı
- Uygulama adı
- Uygulama kullanım süresi
- Kullanım toplama için kullanılan tarih ve saat aralığı

Bu bilgiler, kullanım istatistiklerini sağlamak ve kullanımı kullanıcı hedefleriyle karşılaştırmak için kullanılır.

### 2-2. Kullanıcı Tarafından Girilen veya Yapılandırılan Bilgiler

- Günlük kullanım hedefi
- Kullanım hatırlatıcısının etkinleştirildiği durum ve aralık
- Durum çubuğu kullanım ekranı ayarı
- Geri kazanılan zaman etkinliği kategorisi, başlığı, başlangıç ​​zamanı ve süresi
- Günlük yansıma metni
- İlerlemeyi ve kontrol listesi girişlerini sorgulayın
- Yer paylaşımı istisnası uygulama listesi

### 2-3. Cihazda Saklanan Bilgiler

Uygulama aşağıdaki bilgileri yerel bir SQLite veritabanında veya SharedPreferences'ta saklayabilir:

- Uygulama kullanım süresi kayıtları
- Günlük hedefler ve ayarlar
- Geri kazanılan zaman etkinliği kayıtları
- Günlük yansıma kayıtları
- İlerlemeyi ve kontrol listesi durumunu sorgulama
- İlk katılım tamamlanma durumu
- Kullanım hatırlatıcıları, kesin sınır uyarıları, durum çubuğu ekranı ve yer paylaşımı istisna uygulamaları gibi ayarlar
- Yerel reklam izni ve gizlilik seçeneği durumu

Mevcut uygulamaya göre, bu yerel kayıtlar frog-im sunucularına otomatik olarak yüklenmemektedir.

### 2-4. Reklam ve Rıza Verileri

Google Mobil Reklamlar SDK (AdMob) ve UMP kullanıldığında, Google veya satış ortakları aşağıdaki gibi bilgileri işleyebilir:

- Android AD_ID gibi reklam tanımlayıcıları
- IP adres ve ağ bilgileri
- Cihaz bilgileri, OS sürümü ve uygulama bilgileri
- Reklam gösterimleri, tıklamalar, ölçüm verileri ve hata sinyalleri
- Reklam izni ve gizlilik seçeneği durumu
- Yaklaşık konum

## 3. İşleme Amaçları

Uygulama, bilgileri aşağıdaki amaçlarla işler:

- Kullanım süresini okuma, istatistikleri gösterme ve kullanımı hedeflerle karşılaştırma
- Kullanıcı tarafından girilen geri kazanılan zaman ve yansıma kayıtlarının saklanması
- Mücadele ilerlemesini yönetme
- Hatırlatıcılar ve durum çubuğu bildirimleri sağlama
- Kesin sınır uyarı bildirimleri, yer paylaşımı ekranı ve yer paylaşımı istisna yönetimi sağlama
- Kullanıcı tarafından talep edildiğinde kullanım istatistikleri görsellerinin paylaşılması
- Reklam sunma, reklam performansını ölçme ve reklam izni seçeneklerini uygulama
- Uygulama kararlılığını koruma ve hatalara yanıt verme

## 4. Yerel Depolama ve Harici İşleme

### 4-1. Yerel Depolama

TimeBack, kullanıcı verilerini öncelikle uygulamanın cihazdaki dahili deposunda saklar. Mevcut uygulamaya dayalı olarak kullanım kayıtları, hedefler, yansımalar ve meydan okuma bilgileri, frog-im sunucularına otomatik olarak yüklenmez.

Yerel depolama aşağıdakileri içerebilir.

| Depolamak | Saklanan öğeler | Amaç | Silme yöntemi |
|---|---|---|---|
| SQLite veritabanı | Uygulama kullanım kayıtları, paket adları, uygulama adları, kullanım süresi, tarihe dayalı toplamlar | Kullanım istatistiklerini gösterin ve kullanımı hedeflerle karşılaştırın | Uygulama içi silme özellikleri, uygulama verilerini temizleme veya uygulamayı kaldırma |
| SQLite veritabanı | Geri kazanılan zaman etkinlikleri, düşünceler, mücadele ilerlemesi, kontrol listesi girişleri | Kayıtları gösterin ve ilerlemeyi yönetin | Uygulama içi silme özellikleri, uygulama verilerini temizleme veya uygulamayı kaldırma |
| PaylaşılanTercihler | İlk katılım tamamlanma durumu, hatırlatıcı ayarları, kesin sınır uyarı ayarları, durum çubuğu görüntüleme ayarları, yer paylaşımı istisna uygulama listesi, yerel reklam izni durumu | Uygulama ayarlarını koru | Uygulama verilerini temizleme veya uygulamayı kaldırma |
| Geçici dosyalar/önbellek | Paylaşılan kullanım istatistikleri görselleri ve benzeri geçici dosyalar | Kullanıcının talep ettiği paylaşımı gerçekleştirin | Mümkün olduğunda paylaşımdan sonra veya OS/app temizleme politikalarına göre silindi |

Kullanıcı uygulama verilerini temizlediğinde veya uygulamayı kaldırdığında uygulamanın dahili deposunda saklanan veriler genellikle silinir. Ancak Android yedekleme, üretici yedekleme, bulut yedekleme veya doğrudan kullanıcı tarafından paylaşılan dosyalar, bu hizmetlerin politikalarına göre ayrı ayrı saklanabilir.

Kullanım kayıtları ve yansıma metni kişisel rutinleri veya ilgi alanlarını ortaya çıkarabilir. Paylaşılan cihazlarda kullanıcılar, cihaz kilidi veya ayrı OS hesapları gibi uygun güvenlik önlemlerini kullanmalıdır.

### 4-2. Sunucu Yüklemeleri

Mevcut projeye bağlı olarak TimeBack, kullanım kayıtlarını, yansımaları veya sorgulama kayıtlarını frog-im sunucularına otomatik olarak yüklemez. Kullanıcı paylaşım özelliğini kullanıyorsa oluşturulan istatistik görüntüsü, kullanıcı tarafından seçilen harici uygulamaya veya hizmete aktarılabilir.

### 4-3. Reklam İşleme

Uygulama içi reklamcılık ve izin yönetimi için Google AdMob ve UMP kullanılır. Reklamlarla ilgili bilgiler Google altyapısında işlenebilir.

## 5. Üçüncü Taraf Hizmetler ve İşleyiciler

### 5-1. Google AdMob / UMP

Amaç:

- Banner reklam yayını
- Reklam izni ve gizlilik seçeneği yönetimi
- Reklam performansı ölçümü ve sahtekarlığın önlenmesi

İşlenebilecek bilgiler:

- Reklam tanımlayıcıları
- Cihaz ve ağ bilgileri
- Reklam etkileşim bilgileri
- Onay ve gizlilik seçeneği durumu

### 5-2. Hedef Uygulamaları veya Hizmetleri Paylaşma

Kullanıcı doğrudan kullanım istatistikleri görseli paylaşım özelliğini kullanıyorsa seçilen harici uygulama veya hizmet, paylaşılan görseli işleyebilir. Bu işleme, seçilen hizmetin gizlilik politikasına tabidir.

## 6. Sınır Ötesi Transfer Bildirimi

Aşağıdaki durumlarda bilgiler kullanıcının ülkesi dışında işlenebilir.

| Öğe | Detaylar |
|---|---|
| Alıcı | Google LLC ve bağlı kuruluşları |
| Varış noktası | Amerika Birleşik Devletleri ve Google altyapısının bulunduğu diğer ülkeler/bölgeler |
| Zamanlama | Uygulama çalıştığında, reklam istediğinde, reklamları gösterdiğinde veya ölçtüğünde, tıklamaları işlediğinde veya izinleri işlediğinde |
| Yöntem | Şifreli ağ iletişimi (HTTPS/TLS) |
| Amaç | Reklam dağıtımı, kişiselleştirme durumu yönetimi, ölçüm, analiz, hizmet istikrarının iyileştirilmesi, yasal uyumluluk |
| Veri | Reklam tanımlayıcıları, cihaz/uygulama/ağ bilgileri, reklam etkileşimi bilgileri, izin durumu, yaklaşık konum vb. |
| Tutulma | Google'ın politikalarına ve geçerli yasalara uygun olarak |

Ayrıntılar için lütfen [Cross-Border Transfer Notice](./policy/)'a bakın.

## 7. Yüklü Uygulama Listesi ve Yer Paylaşımı İstisnaları

Android'de, kullanıcı yer paylaşımı istisna uygulamalarını yapılandırırsa uygulama, bir seçim listesi görüntülemek için cihazdaki başlatılabilir uygulamaların paket adlarını ve uygulama adlarını okuyabilir. Kullanıcı tarafından istisna olarak seçilen paket adları, cihazdaki SharedPreferences'ta saklanır ve yalnızca bu uygulamaların üzerinde kesin sınır uyarı katmanlarının gösterilmesini önlemek için kullanılır.

## 8. Saklama

Uygulama, bilgileri aşağıdaki standartlar kapsamında tutar:

- Yerel kullanım, hedef, yansıma ve meydan okuma bilgileri: Kullanıcı silene, uygulama verilerini temizleyene veya uygulamayı kaldırana kadar
- SharedPreferences ayarları: kullanıcı uygulama verilerini temizleyene veya uygulamayı kaldırana kadar
- Paylaşılan görseller için geçici dosyalar: paylaşım için gerektiği şekilde veya OS temizleme politikalarına göre
- Reklam ve izinle ilgili veriler: Google'ın ve diğer ilgili üçüncü tarafların politikalarına göre

## 9. İzinler

Uygulama aşağıdaki izinleri kullanabilir:

- `PACKAGE_USAGE_STATS`: uygulama kullanım süresini oku
- `POST_NOTIFICATIONS`: kullanım hatırlatıcılarını ve durum çubuğu bildirimlerini göster
- `SYSTEM_ALERT_WINDOW`: kesin sınır uyarı katmanlarını göster
- `INTERNET`: SDKs reklamıyla iletişim kurun ve yasal bildirim sayfalarını gösterin
- `ACCESS_NETWORK_STATE`: ağ durumunu kontrol et
- `com.google.android.gms.permission.AD_ID`: reklam tanımlayıcılarını kullan

İzinler yalnızca uygulama özellikleri için gerektiğinde kullanılır. Kullanıcılar cihaz ayarlarından izinleri iptal edebilir ancak ilgili özellikler sınırlı olabilir.

## 10. Kullanıcı Hakları ve Seçenekleri

Kullanıcılar şunları yapabilir:

- Uygulama içindeki kayıtları görüntüleyin, düzenleyin veya silin
- Uygulama verilerini temizleyerek veya uygulamayı kaldırarak yerel bilgileri silin
- Cihaz ayarlarında kullanım erişimini, bildirimi ve reklam tanımlayıcı ayarlarını değiştirme
- Yer paylaşımı iznini iptal edin ve yer paylaşımı istisnası uygulama ayarlarını değiştirin
- Reklam gizliliği seçeneklerini değiştirin
- Gizlilikle ilgili sorularınız veya silme talepleriniz için bize ulaşın

İletişim e-postası: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Güvenlik Önlemleri

Uygulama aşağıdaki güvenlik önlemlerini uygular veya uygulayabilir:

- HTTPS/TLS tabanlı harici iletişim
- Yerel öncelikli veri işleme
- Uygulama özellikleri için gereken minimum izin istekleri
- Reklam izin durumunun uygulanması

Rootlama, jailbreak yapma, kötü amaçlı yazılım veya paylaşılan cihaz kullanımı gibi cihaz güvenlik koşulları ek riskler oluşturabilir.

## 12. Çocukların Gizliliği

TimeBack öncelikle çocuklar için tasarlanmamıştır. Reklam ve izin işlemleri sırasında Google Mobile Ads SDK ve UMP'in yaşla ilgili ayarları veya platform politikaları geçerli olabilir.

## 13. Değişiklikler

Bu Politika yasadaki, üçüncü taraf hizmet yapılandırmasındaki veya uygulama özelliklerindeki değişiklikler nedeniyle güncellenebilir. Önemli değişiklikler uygulama içi bildirim yoluyla veya bu sayfanın güncellenmesi yoluyla bildirilecektir.

## 14. İletişim

- Geliştirici: frog-im
- E-posta: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

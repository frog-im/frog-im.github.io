---
title: Uluslararası Veri Aktarımı Bildirimi | FileGuard
description: FileGuard Uluslararası Veri Aktarımı Bildirimi
lang: tr
last_updated: 2026-06-23
---


# Uluslararası Veri Aktarımı Bildirimi

Yürürlük tarihi: 23 Haziran 2026  
Son güncelleme: 23 Haziran 2026

FileGuard kasanızda saklanan dosyaları, dosya içeriklerini, şifreleri, kasa adlarını veya etkinlik geçmişini geliştirici tarafından işletilen bir sunucuya göndermez.

Yine de bazı bilgiler aşağıdaki durumlarda ülkeniz veya bölgeniz dışında işlenebilir: Android reklam veya izin özellikleri kullanıldığında veya yedekleme hedefi olarak doğrudan yurt dışı bir bulut hizmetini seçtiğinizde.

## 1. Google reklamcılığı ve izin hizmetleri

| Öğe | Ayrıntılar |
|---|---|
| **Alıcılar** | Google LLC, Google bağlı kuruluşları, Google tarafından reklamcılık, izin yönetimi, ölçüm, güvenlik ve hizmet operasyonu için kullanılan işleyiciler ve yapılandırılmış reklam teknolojisi sağlayıcıları |
| **İletişim ve politikalar** | [Google Gizlilik Politikası](https://policies.google.com/privacy), [Google reklam teknolojileri bilgileri](https://policies.google.com/technologies/ads) |
| **Ülkeler** | Amerika Birleşik Devletleri ve Google'ın veya işlemcilerinin sunucuları ve altyapıyı işlettiği diğer ülkeler. Gerçek konumlar ağ yönlendirmesine, hizmet yapılandırmasına ve işlemcilere bağlı olarak değişebilir. |
| **Zamanlama** | ne zaman Android uygulama izin bilgilerini günceller, gizlilik seçeneklerini görüntüler veya reklamları görüntüler, görüntüler veya ölçer |
| **Yöntem** | Uygulama veya uygulama arasındaki şifreli internet iletişimi Google SDKs ve harici sunucular |
| **Bilgi** | Reklam, uygulama örneği veya cihaz tanımlayıcıları; IP adresi; yaklaşık konum; cihaz modeli; işletim sistemi; uygulama sürümü; dil; ağ bilgisi; reklam isteği, gösterim, tıklama, etkileşim ve teşhis bilgileri; izin durumu ve gizlilik seçenekleri |
| **Amaçlar** | Reklam yayını, kişiselleştirilmemiş reklamlar, sıklık sınırı, ölçüm, analiz, sahtekarlığın önlenmesi, izin ve gizlilik seçimi yönetimi, hizmet güvenliği ve politikalara ve yasalara uygunluk |
| **Saklama** | Google'ın ve her işleyicinin gizlilik politikaları, sözleşme yükümlülükleri ve geçerli yasaları kapsamında |

Geliştirici, Google reklamcılık hizmetlerine kasa dosyaları, dosya içerikleri, dosya adları, kasa şifreleri, yedekleme şifreleri veya etkinlik geçmişi sağlamaz.

## 2. Sizin tarafınızdan seçilen harici depolama veya bulut hizmetleri

FileGuard yedekleme dosyaları bir şifre ile şifrelenir ve sizin tarafınızdan seçilen bir konuma kaydedilir. Eğer seçerseniz Google Drive, iCloud Drive, OneDrive, Dropboxveya başka bir senkronizasyon veya belge sağlayıcı hizmeti kullanıyorsanız, şifrelenmiş yedekleme dosyası ve bu sağlayıcı tarafından işlenen ilgili bilgiler (dosya adı ve saklama süresi gibi) ülkenizin dışındaki sunuculara aktarılabilir.

| Öğe | Ayrıntılar |
|---|---|
| **Alıcılar** | Sizin tarafınızdan seçilen dosya, belge veya bulut depolama sağlayıcısı ve onun işlemcileri |
| **Ülkeler** | Seçilen sağlayıcının gizlilik politikasında ve altyapı bilgilerinde açıklandığı gibi |
| **Zamanlama ve yöntem** | Hizmeti depolama konumu olarak seçtiğinizde ve işletim sistemi veya sağlayıcı uygulaması aracılığıyla ağ aktarımı yoluyla bir yedekleme oluşturduğunuzda veya güncellediğinizde |
| **Bilgi** | Şifreyle şifrelenmiş yedekleme paketi, tarafınızca seçilen dosya adı, saklama ve değiştirme süreleri ve sağlayıcı tarafından otomatik olarak işlenen hesap, cihaz veya ağ bilgileri |
| **Amaçlar** | Tarafınızca talep edilen yedekleme depolama, senkronizasyon, kurtarma ve cihazlar arası erişim |
| **Saklama** | Siz dosyayı silene kadar veya seçilen sağlayıcının belirttiği süre boyunca |

Harici hizmeti doğrudan seçersiniz. Geliştirici, hizmetin hesabını, sunucularını veya saklama uygulamalarını kontrol etmez. Yedekleme şifresini kaybederseniz geliştirici şifrelenmiş yedeği kurtaramaz.

## 3. Seçimler ve sonuçları

Uluslararası işlemeyi şu şekilde sınırlayabilirsiniz:

- Mümkün olduğu durumlarda Google'ın reklam gizliliği seçenekleri aracılığıyla izni değiştirme
- Mümkün olduğunda kişiselleştirilmemiş reklamları veya kısıtlı veri işlemeyi seçme
- Cihaz ayarlarında reklam tanımlayıcıyı silme veya sıfırlama ya da reklam kişiselleştirmeyi sınırlama
- Ağ bağlantısının kesilmesi, uygulamanın kullanımının durdurulması veya kaldırılması
- Yurtdışı bulut hizmeti yerine cihazın yerel yedekleme hedefini seçme
- Mevcut yedekleme dosyalarını harici bir hizmetten silme ve senkronizasyonu devre dışı bırakma

Reklamla ilgili işlemenin reddedilmesi, kişiselleştirilmiş reklamı sınırlandırabilir, kişiselleştirilmemiş veya sınırlı reklamlarla sonuçlanabilir veya bazı reklam özelliklerinin engellenmesine neden olabilir. Bulut depolamayı seçmeden yerel kasayı kullanabilirsiniz ancak bu sağlayıcı aracılığıyla senkronizasyon ve uzaktan kurtarma mümkün olmayacaktır.

## 4. Korumalar

Google, uluslararası veri aktarımlarında aktarım sırasında şifreleme ve yasal çerçeveler kullandığını ve bilgilerin dünya genelindeki sunucularda işlenebileceğini belirtiyor.

FileGuard yedekleme paketlerini seçilen konuma yazmadan önce yedekleme şifrenizle şifreler. Harici bir sağlayıcı yine de şifrelenmiş dosyanın kendisini, dosya adını ve hesap veya ağla ilgili bilgileri işleyebilir. Güvenilir bir sağlayıcı seçin ve güçlü, benzersiz bir yedekleme şifresi kullanın.

## 5. İletişim

Uluslararası veri aktarımlarıyla ilgili sorularınız için:

- **İletişim:** frog-im
- **E-posta:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

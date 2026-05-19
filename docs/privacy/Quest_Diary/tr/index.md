---
title: Gizlilik Politikası | QDiary
description: QDiary Gizlilik Politikası
---

# Gizlilik Politikası (QDiary)

- Uygulama Adı: QDiary
- Geliştirici: frog-im
- İletişim: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Yürürlük Tarihi: 2026-04-19
- Son Güncelleme: 2026-04-19

Bu Gizlilik Politikası, QDiary uygulamasının mevcut uygulama yapısı esas alınarak hazırlanmıştır. QDiary; günlük yazma, quest oluşturma ve değerlendirme, giriş yapma, manuel bulut kaydetme, reklam ve bildirim özellikleri sunar ve bu süreçte gerekli olduğu ölçüde kişisel verileri veya kişisel veri niteliği taşıyabilecek bilgileri işleyebilir.

## 1. Sunulan Özellikler

QDiary aşağıdaki özellikleri sunar:

- Günlük yazma, düzenleme ve görüntüleme
- Kategori sınıflandırması ve takvim görünümü
- Quest oluşturma, quest değerlendirmesi ve quest tamamlama işlemleri
- Yerel günlük uygulaması kilidi ve yerel şifreleme
- E-posta ile giriş, e-posta doğrulama, anonim (misafir) giriş ve parola sıfırlama
- Kullanıcı tarafından başlatılan bulut kaydetme ve yükleme
- Reklam gösterimi ve reklam gizlilik seçeneklerinin işlenmesi
- Quest hatırlatma bildirimleri

## 2. İşlenen Bilgi Kategorileri

### 2-1. Kullanıcının Doğrudan Girdiği Bilgiler

- E-posta adresi
- Parola
- Günlük başlığı, içeriği, tarihi, kategorisi ve zorluk seviyesi
- Quest yanıtları, değerlendirme içeriği ve seçilen quest bilgileri
- Quest profiliyle ilgili seçilen değerler ve özet metni
- Günlük uygulaması kilidi için parola ifadesi

### 2-2. Uygulamanın Cihazda Sakladığı Bilgiler

- Yerel günlük veritabanı (SQLite)
- Yerel günlükler için quest durum bilgileri
- Katılım, ayarlar, dil, bildirimler ve reklamlarla ilgili durum değerleri
- Uygulama kilidi doğrulama değerleri, salt ve şifreleme meta verileri
- Quest bildirim zamanlama bilgileri

### 2-3. Hesap ve Kimlik Bilgileri

Firebase Authentication aracılığıyla aşağıdaki bilgiler işlenebilir:

- Firebase UID
- E-posta adresi
- E-posta doğrulamasının tamamlanıp tamamlanmadığı
- Anonim giriş kullanılıp kullanılmadığı

### 2-4. Reklam ve Onay İşleme Bilgileri

Google AdMob ve UMP SDK kullanılırken aşağıdaki bilgiler işlenebilir:

- Reklam tanımlayıcıları (Android AD_ID gibi)
- IP adresi ve ağ bilgileri
- Cihaz bilgileri, işletim sistemi sürümü ve uygulama bilgileri
- Reklam gösterimleri, tıklamalar ve ödül işleme bilgileri
- Reklam onay durumu ve gizlilik seçeneği durumu

### 2-5. Bildirimlerle İlgili Bilgiler

- Bildirim izninin verilip verilmediği
- Devam eden quest içeren günlüklerin tanımlayıcı değerleri
- Quest bildirim metni
- Planlanmış bildirim zamanları

## 3. İşleme Amaçları

Uygulama, bilgileri aşağıdaki amaçlarla işler:

- Kayıt olma, giriş yapma, e-posta doğrulama ve parola sıfırlama
- Günlük yazma, kaydetme ve görüntüleme
- Quest oluşturma, değerlendirme ve tamamlanma tespiti
- Uygulama kilidiyle ilişkili yerel şifreleme ve şifre çözme
- Kullanıcının talep ettiği bulut kaydetme ve yükleme işlemleri
- Quest bildirimleri sağlama
- Reklam sağlama, reklam ödüllerini işleme ve reklam onay durumunu yansıtma
- Güvenlik, hata yönetimi ve hizmetin işletilmesi

## 4. Yerel Depolama, Bulut Depolama ve Harici İşleme

### 4-1. Yerel Depolama

Günlük ve quest bilgileri esas olarak cihazın yerel veritabanında saklanır.

- Uygulama kilidi etkin değilse: genel biçimde yerel olarak saklanır
- Uygulama kilidi etkinse: günlük başlığı, içerik ve quest durumu gibi bazı bilgiler yerel olarak şifrelenerek saklanabilir

### 4-2. Bulut Depolama

Uygulama, yalnızca kullanıcı doğrudan `Save` özelliğini çalıştırdığında verileri Firebase Firestore'a kaydeder.

Mevcut proje yapılandırmasına göre:

- Otomatik tam senkronizasyon kullanılmaz
- Veriler yalnızca kullanıcı manuel olarak kaydettiğinde Firestore `savedDiaries` içine kaydedilir
- Kaydetme sırasında günlük başlığı, içerik ve quest durumu, mevcut uygulama kilidi durumuna bağlı olarak şifreli biçimde saklanabilir
- Veriler yalnızca kullanıcı `Load` işlemini gerçekleştirdiğinde yeniden yerel depolamaya yüklenir

### 4-3. Quest Oluşturma ve Değerlendirme için Harici İşleme

Kullanıcı quest oluşturma veya değerlendirme talep ettiğinde, aşağıdaki bilgiler Firebase Functions aracılığıyla harici işleme için kullanılabilir:

- Günlük başlığı
- Günlük içeriği veya değerlendirme içeriği
- Kategori
- Zorluk seviyesi
- Seçilen quest
- Quest profili özet bilgileri

Bu bilgiler, OpenAI API aracılığıyla quest oluşturma ve değerlendirme için kullanılır.

Önemli:

- İlgili günlük içeriği yalnızca quest özelliği kullanıldığında harici işleme için kullanılır.
- Mevcut proje yapılandırmasına göre, quest günlüklerini ayrı bir `questLogs` koleksiyonuna kaydeden bir kod kullanılmamaktadır.

## 5. Üçüncü Taraf Hizmetler ve Dış Kaynak İşleme

### 5-1. Google Firebase

Amaç:

- Kimlik doğrulama (Firebase Authentication)
- Firestore depolama
- Cloud Functions çalıştırma

İşlenebilecek bilgiler:

- UID, e-posta adresi ve kimlik doğrulama durumu
- Kullanıcının manuel olarak kaydettiği günlük verileri
- Quest talep verileri

### 5-2. OpenAI

Amaç:

- Quest oluşturma
- Quest değerlendirmesi ve tamamlanma değerlendirmesi

İşlenebilecek bilgiler:

- Günlük başlığı/içeriği
- Quest metni
- Zorluk seviyesi ve kategori
- Kullanıcının girdiği değerlendirme içeriği
- Quest profili özet bilgileri

### 5-3. Google AdMob / UMP

Amaç:

- Banner, geçiş ve ödüllü reklam sağlama
- Reklam onayı ve gizlilik seçeneklerini işleme

İşlenebilecek bilgiler:

- Reklam tanımlayıcıları
- Cihaz ve ağ bilgileri
- Reklam etkileşim bilgileri
- Onay durumu

## 6. Uluslararası Aktarım Bildirimi

Uygulama, aşağıdaki durumlarda kişisel verileri veya ilgili bilgileri kullanıcının ülkesi dışında işleyebilir:

| Öğe | Ayrıntılar |
|---|---|
| Alıcı | Google LLC, OpenAI ve ilgili altyapı işletmecileri |
| Hedef Ülke | Amerika Birleşik Devletleri vb. |
| Aktarım Zamanı | Giriş sırasında, quest oluşturma/değerlendirme sırasında, reklam taleplerinde ve onay işleme sırasında |
| Aktarım Yöntemi | Şifreli ağ iletişimi |
| Aktarım Amacı | Kimlik doğrulama, veri depolama, sunucusuz işleme, yapay zekâ ile quest oluşturma/değerlendirme ve reklam sunumu |

## 7. Saklama ve Kullanım Süresi

Uygulama, bilgileri aşağıdaki standartlara göre saklar:

- Yerel günlük/ayar bilgileri: kullanıcı silene veya uygulamayı kaldırana kadar
- Firebase hesap bilgileri: kullanıcı hesabı sürdürdüğü sürece
- Firestore'da saklanan veriler: kullanıcı kaydedilmiş öğeleri tuttuğu sürece
- Quest talebi işleme verileri: sunucusuz işleme için gerekli olduğu ölçüde
- Reklam/onay ile ilgili veriler: ilgili her harici sağlayıcının politikasına göre

Buna ek olarak, mevcut proje aşağıdaki otomatik temizleme mantığını içerir:

- Belirli bir süreden sonra anonim kullanıcı hesaplarının ve kullanıcı alt koleksiyonu Firestore verilerinin temizlenmesi
- Uzun süredir etkin olmayan normal kullanıcı hesaplarının ve kullanıcı alt koleksiyonu Firestore verilerinin temizlenmesi

Ancak bunun gerçekten üretim ortamına yansıyıp yansımadığı, dağıtım durumu ve sunucu ayarlarına bağlı olarak değişebilir.

## 8. Uygulama Kilidi ve Yerel Şifreleme Bildirimi

Uygulama ayrı bir `Diary App Lock` özelliği sunar.

- Uygulama kilidi parola ifadesi, hesap parolasından ayrıdır.
- Uygulama kilidi parola ifadesi, yerel günlüğün şifrelenmesi ve şifresinin çözülmesi için kullanılır.
- Yanlış bir parola ifadesi girilse bile, uygulamanın kendisi her zaman tamamen kilitlenmeyebilir; bunun yerine bazı günlük içerikleri okunamaz halde kalabilir.
- Bazı günlükler, yazım anında veya geçici kilit açma anında kullanılan parola ifadesine göre ayrı olarak şifrelenebilir.

Kullanıcılar parola ifadelerini güvenli şekilde saklamalıdır; kaybolması halinde bazı yerel verilerin kurtarılması zor olabilir.

## 9. Quest Bildirim Bildirimi

Kullanıcı quest bildirimlerini etkinleştirdiğinde, devam eden quest içeren her günlük için yerel bildirimler planlanabilir.

- Zamanlama esas olarak cihazın dahili zamanlama sistemi tarafından yönetilir.
- Mevcut proje yapılandırmasına göre, yalnızca bildirim amacıyla günlük ham metninin periyodik olarak merkezi bir sunucuya iletildiği doğrulanmış bir yapı bulunmamaktadır.

## 10. İzin Kullanımı Bildirimi

Uygulama, özelliklerini sağlamak için aşağıdaki izinleri kullanabilir:

- `INTERNET`: Firebase, OpenAI ve reklam SDK'leri ile iletişim
- `com.google.android.gms.permission.AD_ID`: reklam tanımlayıcılarının kullanımı
- `POST_NOTIFICATIONS`: quest bildirimlerini görüntüleme
- `RECEIVE_BOOT_COMPLETED`: cihaz yeniden başlatıldıktan sonra planlanan bildirimleri geri yükleme

İzinler yalnızca ilgili işlevleri yerine getirmek için gerekli olduğu ölçüde kullanılır.

## 11. Veri Sahibinin Hakları ve Bunların Kullanılması

Kullanıcılar aşağıdaki hakları kullanabilir:

- Uygulama içindeki verilere erişme, bunları değiştirme ve silme
- Bulutta saklanan verileri silme veya üzerine yazma
- Çıkış yapma ve hesap silme talebinde bulunma
- Reklam gizlilik seçeneklerini değiştirme
- Bildirim izinlerini devre dışı bırakma

Bu hakların kullanılma yolları:

- Günlükleri doğrudan uygulama içinde silme veya düzenleme
- Uygulamayı silme veya yerel verileri sıfırlama
- Hesaptan çıkış yapma ve ayrıca silme talebinde bulunma
- Bildirimleri, reklam tanımlayıcılarını ve izinleri cihaz ayarlarından değiştirme
- İletişim e-postası: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Güvenlik Önlemleri

Uygulama aşağıdaki koruyucu önlemleri uygular veya uygulayabilir:

- HTTPS tabanlı iletişim
- Yerel günlük uygulaması kilidi ve şifreleme
- Parola ifadesi doğrulama değerlerinin ayrı saklanması
- Firebase Authentication kullanımı
- Asgari düzeyde izin talebi

Ancak kullanıcının cihaz güvenlik durumuna bağlı olarak, örneğin root erişimi, jailbreak, kötü amaçlı yazılım veya paylaşılan cihaz kullanımı gibi nedenlerle riskler ortaya çıkabilir.

## 13. Çocukların Kişisel Verileri

Uygulama, esas olarak çocuklara yönelik bir hizmet olarak tasarlanmamıştır. Ancak reklam/onay işleme sürecinde UMP içindeki yaşla ilgili seçenekler uygulanabilir.

## 14. Bu Politikadaki Değişiklikler

Bu Politika; mevzuat, üçüncü taraf hizmetler veya uygulama özelliklerindeki değişiklikler nedeniyle güncellenebilir.

- Mevcut sürüm için son güncelleme tarihi: **2026-04-19**

## 15. İletişim

- Geliştirici: frog-im
- E-posta: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Hesap silme rehberi: [Silme talimatları](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)


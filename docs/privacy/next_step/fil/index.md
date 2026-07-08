---
title: Patakaran sa Privacy | Next Step
description: Patakaran sa Privacy ng Next Step
lang: fil
last_updated: 2026-07-08
---

# Patakaran sa Privacy (Next Step)

- **Pangalan ng app:** Next Step (다음한걸음)
- **Developer:** frog-im
- **Contact sa privacy:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Petsa ng bisa:** 2026-07-08
- **Huling na-update:** 2026-07-08

> Ang patakarang ito ay ginawa batay sa kasalukuyang implementasyon ng Next Step app. Kung may umiiral na sapilitang batas sa isang bansa o rehiyon, maaaring mauna ang batas na iyon.

---

## 1. Layunin at saklaw

Ang Next Step ay isang local-first na app para sa sariling pagninilay. Tinutulungan nito ang user na ayusin at balikan sa sariling device ang paulit-ulit na problema, sanhi, susunod na aksyon, at tala ng pagpapatupad.

Hindi kailangan ng app ang pag-sign up o pag-login. Walang server na pinapatakbo ng developer na tumatanggap ng nilalaman ng memo, impormasyon ng folder, backup file, PIN, biometric information, o statistical data. Gayunman, maaaring gumamit ang app ng Google AdMob at Google User Messaging Platform (UMP) upang magbigay ng ads at privacy choices para sa ads.

## 2. Impormasyong pinoproseso

### 2-1. Data ng memo na direktang ipinasok o ginawa ng user

Para maibigay ang mga feature, maaaring iproseso ng app ang sumusunod na impormasyon sa device.

- Mga problema, dahilan, susunod na aksyon, at execution notes na isinulat ng user
- Emosyon, kahalagahan, tags, kategorya, at completion status
- Oras ng paggawa, oras ng pagbabago, at status ng completion ng memo
- Mga pangalan, kulay, at parent-folder information na ginawa o binago ng user
- Local calculation results para sa review screens, statistics, macro execution, at retrospectives

Pinoproseso ang impormasyong ito sa device ng user upang maibigay ang mga feature ng app. Hindi ito ina-upload ng developer sa server na pinapatakbo ng developer.

### 2-2. Authentication at security information

Para sa app lock, maaaring iproseso ng app ang sumusunod sa secure storage ng device.

- Kung naka-enable ang app lock
- PIN hash at salt
- Kung naka-enable ang biometric authentication
- Setting information gaya ng lock-related update times

Hindi ini-store o ipinapadala sa developer ang original PIN. Ang biometric authentication ay ginagawa ng operating system; hindi nangongolekta ang app ng fingerprint images, face images, o biometric templates, at tinitingnan lamang kung matagumpay ang authentication.

### 2-3. Local backup, restore, at sharing

Kapag direktang nag-export, nag-restore, o nag-share ang user, maaaring iproseso ng app ang sumusunod.

- JSON backup files na naglalaman ng memos at folders
- Pangalan ng backup file, oras ng paggawa, at impormasyon ng restore result
- Image files na nabubuo kapag nagse-share ng review images
- File paths na pinili ng user o document picker results ng operating system

Ginagawa lamang ang backup files at review images kapag direktang ine-export o sine-share ng user. Hindi natatanggap ng developer ang mga file na ito sa server na pinapatakbo ng developer.

### 2-4. Impormasyong maaaring awtomatikong iproseso sa ads at consent

Sa mga suportadong platform, maaaring gumamit ang app ng Google AdMob at UMP. Maaaring iproseso ng Google at advertising technology providers ang sumusunod.

- Advertising identifiers, app instance identifiers, o device-related identifiers
- IP address at approximate location na hinuha mula sa IP address o katulad na data
- Device model, operating system, app version, wika, at network information
- Ad requests, impressions, clicks, interactions, at diagnostic information
- Ad consent status at regional privacy choices

Maaaring iproseso ang impormasyong ito para sa ad delivery, non-personalized ads, frequency capping, measurement, abuse prevention, consent management, security, at legal compliance. Nakaimplementa ang app na humiling lamang ng ads kapag maaari na ang ad requests pagkatapos ng UMP process.

Makikita ang paraan ng pagproseso ng Google sa [Google Privacy Policy](https://policies.google.com/privacy) at [Google advertising technologies guide](https://policies.google.com/technologies/ads).

## 3. Mga layunin ng pagproseso

Pinoproseso ng Next Step ang impormasyon para sa sumusunod.

- I-save at ipakita ang memos, causes, next actions, emotions, tags, at folders
- Pamahalaan ang completion status at retrospective flows ng memo
- Magbigay ng local analysis results tulad ng reviews, statistics, recurring problems, at remaining actions
- Kontrolin ang access sa pamamagitan ng app lock, PIN, at biometric authentication
- Gumawa at mag-restore ng backup files at mag-share ng review images
- Panatilihin ang app settings tulad ng wika, theme, at ad privacy choices
- Magbigay ng ads, pamahalaan ang ad frequency, at magbigay ng privacy choices
- Pigilan ang abuse, protektahan ang service security, at sumunod sa legal obligations

## 4. Lokasyon ng storage at retention period

| Kategorya | Lokasyon at panahon ng storage | Paraan ng pagbura |
|---|---|---|
| Core data tulad ng memos, folders, at completion status | App-specific local storage hanggang burahin ng user | Burahin sa app, burahin ang app data, o i-uninstall ang app |
| App lock settings, PIN hash, at biometric settings | Secure storage ng operating system hanggang baguhin ang settings o burahin ang app data | I-disable ang related feature, burahin ang app data, o i-uninstall ang app |
| Backup files | Device folder, document provider, o external storage na pinili ng user hanggang burahin | Burahin sa file manager app o storage service |
| Review images | Pansamantalang nililikha bago mag-share at pinoproseso ng OS o app na pinili ng user | Isara ang app, linisin ang cache, o burahin sa sharing app/storage location |
| Google advertising information | Pinapanatili ayon sa policies at legal obligations ng Google at related processors | Baguhin ang app/device ad settings o gamitin ang Google privacy settings |

Maaaring magpanatili ang operating system, device manufacturer, file provider, o cloud storage service ng hiwalay na kopya ng app data o backup files na ginawa ng user. Saklaw ng policies ng provider ang mga kopyang iyon.

## 5. Third-party disclosure, processing entrustment, at sale

Hindi ibinebenta ng developer ang nilalaman ng memo, PIN, o local in-app data, at hindi ito ibinibigay sa third parties sa pamamagitan ng server ng developer.

Kapag gumagana ang ads o consent features, maaaring iproseso ng Google LLC, Google affiliates, advertising technology providers, at related processors ang impormasyon sa Section 2-4. Para sa detalye, tingnan ang [International Data Transfer Notice](policy/).

Kung direktang pipili ang user ng external app o cloud service para mag-save ng backup file, pumili ng file, o mag-share ng review image, maaaring iproseso ng provider na iyon ang file ayon sa instructions ng user. Sa ganitong kaso, ang privacy policy at security settings ng provider ang aangkop, at hindi kontrolado ng developer ang pagproseso ng external service na pinili ng user.

## 6. International data transfers

Hindi inililipat ang memos at core app data sa server ng developer. Gayunman, kapag ginagamit ang ads at consent features, maaaring iproseso ng Google at related processors ang ad at consent information sa United States at iba pang bansang pinapatakbo ang kanilang infrastructure.

Kung pipili ang user ng overseas cloud service o foreign server-based service bilang backup location o sharing destination, maaaring mailipat o ma-sync ang file sa overseas servers ayon sa choice ng user. Para sa detalye, tingnan ang [International Data Transfer Notice](policy/).

## 7. Paggamit ng permissions

Maaaring gamitin ng app ang sumusunod na permissions o system features kapag ginagamit ng user ang kaugnay na feature.

- **File selection and saving:** ginagamit upang pumili o mag-save ng backup files
- **Biometric authentication:** ginagamit upang i-unlock ang app o muling kumpirmahin ang sensitive setting changes
- **Internet at network state:** ginagamit upang humiling ng AdMob ads at UMP consent information
- **Advertising identifier:** ginagamit upang magbigay ng Google advertising features

Kung hindi pinayagan ang permission, ang kaugnay na feature lamang ang maaaring malimitahan. Kapag ginagamit ang system file picker, karaniwang limitado ang access ng app sa mga item na pinili ng user.

## 8. Security measures at limits

Gumagamit ang kasalukuyang implementasyon ng sumusunod.

- Ini-store ang memo at folder data sa local storage ng device
- Ini-store ang PIN hash at salt sa secure storage
- Gumagamit ng OS biometric authentication sa supported devices
- Ini-store ang app lock status at security settings sa secure storage
- Hinahayaan ang user na direktang gumawa, mag-save, at mag-restore ng backup files

Walang security method na ganap na nakaaalis sa lahat ng risk. Maaaring ma-expose ang impormasyon dahil sa pagkawala ng device, malware, OS vulnerabilities, mahinang PIN, files na direktang ibinahagi ng user, o security issues ng external storage services.

Kung ang backup files o review images ay ise-save o ise-share sa external apps o cloud services, maaaring manatili ang hiwalay na copies sa mga lokasyong iyon. Dapat mismong tingnan ng user kung may sensitibong impormasyon.

## 9. Mga karapatan at pagpipilian ng user

Dahil karamihan ng impormasyon ay nasa device lamang ng user, hindi ito malayuang makikita, mababago, o mabubura ng developer. Maaaring pamahalaan ng user ang impormasyon sa mga sumusunod.

- Burahin ang memos, folders, o completion records sa app
- Baguhin ang app lock, PIN, biometric authentication, wika, at theme settings
- Burahin ang app data o i-uninstall ang app
- Burahin mula sa storage location ang backup files at shared files na ginawa ng user
- Kung naaangkop, baguhin ang consent sa Google ad privacy choices screen sa app
- Burahin o i-reset ang advertising identifier, o limitahan ang ad personalization, sa device settings

Ang requests tungkol sa impormasyong direktang ibinigay ng user at hawak ng developer, gaya ng inquiry emails, ay maaaring ipadala sa contact sa ibaba. Kung naaangkop sa ilalim ng batas, maaaring kilalanin ang rights to access, correction, deletion, restriction of processing, withdrawal of consent, at complaint sa supervisory authority.

## 10. Privacy ng mga bata

Hindi pangunahing idinisenyo ang Next Step para sa mga bata at hindi nito hinihingi sa mga bata na maglagay ng personal information. Maaaring gamitin ng guardians ang parental control features ng device o app store.

## 11. Contact

Para sa inquiries tungkol sa personal information processing:

- **Contact person:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Ang requests tungkol sa advertising information na pinoproseso ng Google ay maaaring gawin sa pamamagitan ng privacy controls at inquiry procedures sa [Google Privacy Policy](https://policies.google.com/privacy).

## 12. Pagbabago sa patakaran

Maaaring baguhin ang patakarang ito kung magbago ang batas, app features, permissions, o processing practices ng third-party SDKs. Maaaring ipaalam ang mahahalagang pagbabago sa page na ito, in-app screens, o distribution pages.

Huling na-update: **2026-07-08**

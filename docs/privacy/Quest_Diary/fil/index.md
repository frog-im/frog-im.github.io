---
title: Patakaran sa Privacy | QDiary
description: Patakaran sa Privacy ng QDiary
---

# Patakaran sa Privacy (QDiary)

- Pangalan ng App: QDiary
- Developer: frog-im
- Contact: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Petsa ng Pagkakabisa: 2026-04-19
- Huling Pag-update: 2026-04-19

Ang Patakaran sa Privacy na ito ay ginawa batay sa kasalukuyang implementasyon ng QDiary app. Nagbibigay ang QDiary ng mga tampok para sa pagsusulat ng diary, pagbuo at pagninilay sa quest, pag-log in, manu-manong pag-save sa cloud, advertising, at notifications, at sa prosesong iyon ay maaaring magproseso ng personal na impormasyon o impormasyon na maaaring ituring na personal na impormasyon sa lawak na kinakailangan.

## 1. Mga Tampok na Ibinibigay

Ibinibigay ng QDiary ang mga sumusunod na tampok:

- Pagsusulat, pag-edit, at pagtingin ng mga diary
- Pag-uuri ayon sa kategorya at calendar view
- Pagbuo ng quest, pagninilay sa quest, at paghawak sa pagkumpleto ng quest
- Lokal na app lock para sa diary at lokal na encryption
- Email login, email verification, anonymous (guest) login, at password reset
- Cloud save at load na pinasimulan ng user
- Pagpapakita ng ads at paghawak sa mga privacy option ng ads
- Mga paalala sa quest sa pamamagitan ng notifications

## 2. Mga Kategorya ng Impormasyong Pinoproseso

### 2-1. Impormasyong Direktang Inilalagay ng User

- Email address
- Password
- Pamagat ng diary, nilalaman, petsa, kategorya, at hirap
- Mga sagot sa quest, nilalaman ng pagninilay, at impormasyon ng napiling quest
- Mga piniling halaga na may kaugnayan sa quest profile at buod na teksto
- Passphrase para sa diary app lock

### 2-2. Impormasyong Iniimbak ng App sa Device

- Lokal na diary DB (SQLite)
- Impormasyon ng status ng quest para sa mga lokal na diary
- Mga halaga ng estado kaugnay ng attendance, settings, language, notifications, at ads
- Mga halaga ng pag-verify ng app lock, salt, at metadata ng encryption
- Impormasyon sa pag-iskedyul ng notification para sa quest

### 2-3. Impormasyon ng Account at Pagkakakilanlan

Ang mga sumusunod na impormasyon ay maaaring iproseso sa pamamagitan ng Firebase Authentication:

- Firebase UID
- Email address
- Kung nakumpleto na ang email verification
- Kung ginagamit ang anonymous login

### 2-4. Impormasyon sa Advertising at Consent

Kapag gumagamit ng Google AdMob at UMP SDK, maaaring iproseso ang mga sumusunod na impormasyon:

- Mga advertising identifier (gaya ng Android AD_ID)
- IP address at impormasyon ng network
- Impormasyon ng device, bersyon ng OS, at impormasyon ng app
- Impormasyon tungkol sa ad impressions, clicks, at pagproseso ng rewards
- Katayuan ng ad consent at katayuan ng privacy options

### 2-5. Impormasyong Kaugnay ng Notifications

- Kung naibigay ang pahintulot para sa notifications
- Mga identifier value para sa mga diary na may nagpapatuloy na quest
- Teksto ng quest notification
- Mga nakaiskedyul na oras ng notification

## 3. Mga Layunin ng Pagproseso

Pinoproseso ng app ang impormasyon para sa mga sumusunod na layunin:

- Sign-up, login, email verification, at password reset
- Pagsusulat, pag-save, at pagtingin ng diary
- Pagbuo ng quest, pagninilay, at pagtukoy ng pagkumpleto
- Lokal na encryption at decryption na kaugnay ng app lock
- Cloud save at load na hinihiling ng user
- Pagbibigay ng quest notifications
- Pagbibigay ng ads, pagproseso ng ad rewards, at pagpapakita ng status ng ad consent
- Seguridad, paghawak ng error, at pagpapatakbo ng serbisyo

## 4. Lokal na Imbakan, Cloud Storage, at Panlabas na Pagproseso

### 4-1. Lokal na Imbakan

Ang impormasyon ng diary at quest ay pangunahing iniimbak sa lokal na DB ng device.

- Kung hindi naka-enable ang app lock: lokal itong iniimbak sa pangkalahatang anyo
- Kung naka-enable ang app lock: ang ilang impormasyon, gaya ng pamagat ng diary, nilalaman, at status ng quest, ay maaaring i-encrypt at iimbak nang lokal

### 4-2. Cloud Storage

Nag-iimbak lamang ang app ng data sa Firebase Firestore kapag direktang ginagamit ng user ang tampok na `Save`.

Sa ilalim ng kasalukuyang configuration ng proyekto:

- Hindi ginagamit ang awtomatikong buong synchronization
- Iniimbak ang data sa Firestore `savedDiaries` lamang kapag mano-manong sine-save ito ng user
- Kapag sine-save, ang pamagat ng diary, nilalaman, at status ng quest ay maaaring maimbak sa naka-encrypt na anyo depende sa kasalukuyang status ng app lock
- Nilo-load muli ang data pabalik sa lokal na storage lamang kapag ginagamit ng user ang `Load`

### 4-3. Panlabas na Pagproseso para sa Pagbuo at Pagninilay sa Quest

Kapag humihiling ang user ng pagbuo ng quest o pagninilay, maaaring gamitin ang mga sumusunod na impormasyon para sa panlabas na pagproseso sa pamamagitan ng Firebase Functions:

- Pamagat ng diary
- Nilalaman ng diary o nilalaman ng pagninilay
- Kategorya
- Hirap
- Napiling quest
- Buod ng impormasyon ng quest profile

Ginagamit ang impormasyong ito para sa pagbuo at pagsusuri ng quest sa pamamagitan ng OpenAI API.

Mahalaga:

- Ginagamit lamang ang kaugnay na nilalaman ng diary para sa panlabas na pagproseso kapag ginagamit ang tampok na quest.
- Sa ilalim ng kasalukuyang configuration ng proyekto, hindi ginagamit ang code na nag-iimbak ng mga quest log sa hiwalay na `questLogs` collection.

## 5. Mga Third-Party Service at Outsourced Processing

### 5-1. Google Firebase

Layunin:

- Authentication (Firebase Authentication)
- Firestore storage
- Pagpapatakbo ng Cloud Functions

Impormasyong maaaring iproseso:

- UID, email address, at authentication status
- Data ng diary na mano-manong sine-save ng user
- Data ng kahilingan sa quest

### 5-2. OpenAI

Layunin:

- Pagbuo ng quest
- Pagninilay sa quest at pagsusuri ng pagkumpleto

Impormasyong maaaring iproseso:

- Pamagat/nilalaman ng diary
- Teksto ng quest
- Hirap at kategorya
- Nilalaman ng pagninilay na inilagay ng user
- Buod ng impormasyon ng quest profile

### 5-3. Google AdMob / UMP

Layunin:

- Pagbibigay ng banner, interstitial, at rewarded ads
- Paghawak sa ad consent at privacy options

Impormasyong maaaring iproseso:

- Mga advertising identifier
- Impormasyon ng device at network
- Impormasyon ng pakikipag-ugnayan sa ad
- Katayuan ng consent

## 6. Paunawa sa International Transfer

Maaaring iproseso ng app ang personal na impormasyon o kaugnay na impormasyon sa labas ng bansa ng user sa mga sumusunod na kaso:

| Item | Mga Detalye |
|---|---|
| Tatanggap | Google LLC, OpenAI, at mga kaugnay na operator ng imprastraktura |
| Bansang Patutunguhan | United States, at iba pa |
| Oras ng Paglilipat | Sa panahon ng login, pagbuo/pagninilay sa quest, mga kahilingan sa ad, at pagproseso ng consent |
| Paraan ng Paglilipat | Naka-encrypt na komunikasyon sa network |
| Layunin ng Paglilipat | Authentication, data storage, serverless processing, AI quest generation/evaluation, at advertising |

## 7. Panahon ng Pagtatago at Paggamit

Pinananatili ng app ang impormasyon ayon sa mga sumusunod na pamantayan:

- Lokal na impormasyon ng diary/settings: hanggang burahin ito ng user o i-uninstall ang app
- Impormasyon ng Firebase account: habang pinananatili ng user ang account
- Data na nakaimbak sa Firestore: habang pinananatili ng user ang mga naka-save na item
- Data para sa pagproseso ng kahilingan sa quest: sa lawak na kinakailangan para sa serverless processing
- Data na may kaugnayan sa ads/consent: ayon sa patakaran ng bawat external provider

Bukod dito, kasama sa kasalukuyang proyekto ang sumusunod na awtomatikong logic sa paglilinis:

- Paglilinis ng anonymous user accounts at user subcollection Firestore data makalipas ang isang tiyak na panahon
- Paglilinis ng regular user accounts na matagal nang hindi aktibo at user subcollection Firestore data

Gayunman, kung ito ay talagang naipapatupad sa production environment ay maaaring mag-iba depende sa deployment status at server settings.

## 8. Paunawa sa App Lock at Lokal na Encryption

Nagbibigay ang app ng hiwalay na tampok na `Diary App Lock`.

- Hiwalay ang passphrase ng app lock sa password ng account.
- Ginagamit ang passphrase ng app lock para sa lokal na encryption at decryption ng diary.
- Kahit maling passphrase ang mailagay, maaaring hindi palaging ganap na ma-block ang app; sa halip, maaaring manatiling hindi mabasa ang ilang nilalaman ng diary.
- Maaaring hiwalay na ma-encrypt ang ilang diary batay sa passphrase na ginamit sa oras ng pagsusulat o pansamantalang pag-unlock.

Dapat panatilihing ligtas ng mga user ang kanilang passphrase, at kung ito ay mawala, maaaring maging mahirap ang pagbawi ng ilang lokal na data.

## 9. Paunawa sa Quest Notifications

Kung i-enable ng user ang quest notifications, maaaring mag-iskedyul ng lokal na notifications para sa bawat diary na may nagpapatuloy na quest.

- Ang pag-iskedyul ay pangunahing pinamamahalaan ng internal device scheduling.
- Sa ilalim ng kasalukuyang configuration ng proyekto, walang kumpirmadong istruktura kung saan ang orihinal na teksto ng diary ay pana-panahong ipinapadala sa isang sentral na server para lamang sa layunin ng notification.

## 10. Paunawa sa Paggamit ng Permissions

Maaaring gamitin ng app ang mga sumusunod na permissions upang maibigay ang mga tampok nito:

- `INTERNET`: komunikasyon sa Firebase, OpenAI, at ad SDKs
- `com.google.android.gms.permission.AD_ID`: paggamit ng advertising identifiers
- `POST_NOTIFICATIONS`: pagpapakita ng quest notifications
- `RECEIVE_BOOT_COMPLETED`: pagpapanumbalik ng mga nakaiskedyul na notification pagkatapos mag-reboot ang device

Ginagamit lamang ang permissions sa lawak na kinakailangan upang maisagawa ang mga kaugnay na function.

## 11. Mga Karapatan ng Data Subject at Paano Ito Isasagawa

Maaaring gamitin ng mga user ang mga sumusunod na karapatan:

- Mag-access, magbago, at magbura ng data sa loob ng app
- Magbura o mag-overwrite ng data na nakaimbak sa cloud
- Humiling ng logout at pagbura ng account
- Baguhin ang mga privacy option ng ads
- I-disable ang permissions para sa notifications

Paano gamitin ang mga karapatang ito:

- Direktang burahin o i-edit ang mga diary sa loob ng app
- Burahin ang app o i-reset ang lokal na data
- Mag-log out sa account at hiwalay na humiling ng pagbura
- Baguhin ang notifications, advertising identifiers, at permissions sa settings ng device
- Contact email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Mga Hakbang sa Seguridad

Nagpapatupad o maaaring magpatupad ang app ng mga sumusunod na proteksiyong hakbang:

- HTTPS-based communication
- Lokal na diary app lock at encryption
- Hiwalay na pag-iimbak ng mga halaga ng pag-verify ng passphrase
- Paggamit ng Firebase Authentication
- Minimal na kahilingan para sa permissions

Gayunman, maaaring magkaroon ng mga panganib depende sa estado ng seguridad ng device ng user, tulad ng rooting, jailbreaking, malware, o paggamit ng shared device.

## 13. Personal na Impormasyon ng mga Bata

Ang app ay hindi idinisenyo bilang isang serbisyong pangunahing inilaan para sa mga bata. Gayunman, maaaring mailapat ang mga opsyon na may kaugnayan sa edad sa loob ng UMP sa panahon ng pagproseso ng ads/consent.

## 14. Mga Pagbabago sa Patakarang Ito

Maaaring baguhin ang Patakarang ito dahil sa mga pagbabago sa batas, third-party services, o mga tampok ng app.

- Huling na-update para sa kasalukuyang bersyon: **2026-04-19**

## 15. Contact

- Developer: frog-im
- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Gabay sa pagtanggal ng account: [Mga tagubilin sa pagtanggal](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)


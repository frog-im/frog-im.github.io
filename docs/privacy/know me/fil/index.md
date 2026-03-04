---
title: Patakaran sa Privacy | know_me
description: know_me (PeopleNote, Memory for People) Patakaran sa Privacy (Filipino)
---

# Patakaran sa Privacy (know_me / PeopleNote, Memory for People)

- **Pangalan ng App:** know_me (PeopleNote, Memory for People)
- **Developer:** frog-im
- **Opisyal sa Proteksiyon ng Personal na Impormasyon / Taong Maaaring Kontakin:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Petsa ng Pagkakabisa:** 2026-03-04
- **Huling Na-update:** 2026-03-04

> Inihanda ang Patakarang ito batay sa impormasyong pinoproseso ng app at sa mga kaugnay nitong feature.  
> Kung may anumang sapilitang batas o regulasyon na nalalapat sa isang partikular na bansa o rehiyon, maaaring manaig ang naturang mga batas o regulasyon.

---

## 1. Layunin at Saklaw

Ang `know_me` ay isang app na idinisenyo upang tulungan ang mga user na magtala at mamahala ng impormasyon tungkol sa mga tao, at kung kinakailangan, mag-back up, mag-restore, at magbahagi ng naturang impormasyon bilang mga PDF file.

Kabilang sa mga pangunahing feature nito ang:

- Pag-iimbak ng impormasyong partikular sa tao (tulad ng pangalan, tekstong pangkilala, mga tala, katangian ng personalidad, bansa, kasarian, impormasyon sa pakikipag-ugnayan, atbp.)
- Pag-uuri ng folder, paghahanap, at mga function ng pagsasama
- Pag-attach ng larawan at pamamahala ng paglalarawan
- Pag-export at pag-import ng mga backup (`.knm`)
- Pag-export ng mga PDF
- Pag-lock ng app (password / pattern)
- Pamamahala ng advertising at pahintulot (AdMob / UMP)

Hindi nangangailangan ang app ng hiwalay na pagrerehistro ng account, at ang pangunahing data ng user ng app ay karaniwang iniimbak nang lokal sa device ng user.  
Gayunpaman, ang ilang third-party SDK na kasama para sa pamamahala ng advertising at pahintulot ay maaaring magproseso ng ilang impormasyon.

---

## 2. Mga Kategorya ng Personal na Impormasyong Pinoproseso

### 2-1) Impormasyong Direktang Inilalagay ng User

Ang sumusunod na impormasyon ay iniimbak lamang kapag ito ay direktang inilalagay ng user:

- Pangalan
- Tekstong pangkilala (tulad ng anyo / katangiang ginagamit bilang memo text)
- Mga tala
- Katangian ng personalidad, bansa, kasarian
- Numero ng telepono
- Tekstong may kaugnayan sa oras ng paglitaw / oras ng pagkikita
- Impormasyon ng platform / site
- Pangalan / kulay ng folder
- Paglalarawan ng larawan (caption)

### 2-2) Mga File na Pinili sa Device

- Mga image file na pinili ng user kapag nag-a-attach ng mga larawan
- Mga `.knm` backup file na pinili ng user kapag nag-i-import ng mga backup
- Mga save path at mga na-save na file na pinili ng user kapag nag-e-export ng mga PDF / backup

### 2-3) Data na Lokal na Iniimbak sa Loob ng App

Ang sumusunod na data ay maaaring itago sa device ng user upang maibigay ang mga feature ng app:

- SQLite DB (`people_note.db`): metadata para sa mga tao / folder / platform / site / image
- Mga image file: naka-encrypt at nakaimbak sa loob ng documents folder ng app (`.enc`)
- Mga setting ng app (`SharedPreferences`): theme, sorting, privacy / ad options, PDF masking options, mga patakaran sa app lock, atbp.
- Impormasyon ng app lock: mga hash value at salt para sa mga password / pattern (`SharedPreferences`)
- Mga lokal na encryption key: nakaimbak sa `flutter_secure_storage`
- Mga pansamantalang file: mga preview ng image decryption, import / export cache file, atbp. (temporary folder)

### 2-4) Impormasyong Maaaring Awtomatikong Maproseso sa Panahon ng Advertising at Pamamahala ng Pahintulot

Kapag naka-enable ang mga feature ng advertising o pamamahala ng pahintulot, ang mga SDK ng Google LLC at mga kaugnay na partner (tulad ng AdMob at UMP) ay maaaring awtomatikong magproseso ng sumusunod na impormasyon:

- Mga advertising identifier (AAID / IDFA, atbp.)
- IP address at impormasyon ng network
- Impormasyon ng device (bersyon ng OS, modelo ng device, bersyon ng app, atbp.)
- Impormasyon ng interaksiyon sa ad (impressions, clicks, atbp.)
- Katayuan ng pahintulot at impormasyon sa mga piniling opsyon sa privacy
- Impormasyong may kaugnayan sa diagnostic, performance, at seguridad

Ang pangunahing mga tala ng user sa app ay karaniwang hindi ina-upload sa server ng developer, ngunit ang ilan sa mga impormasyong nasa itaas ay maaaring maipadala sa mga third-party service habang ginagamit ang mga feature ng advertising / pahintulot.

---

## 3. Layunin ng Pagproseso ng Personal na Impormasyon

Pinoproseso ng app ang personal na impormasyon o kaugnay na impormasyon para sa mga sumusunod na layunin:

- Pagtatala at pag-browse ng impormasyong may kaugnayan sa mga tao na nakasentro sa contacts / notes
- Pagbibigay ng mga feature sa pag-aayos tulad ng pag-uuri ng folder, paghahanap, at pagsasama
- Pag-attach at pagpapakita ng mga larawan
- Pagsasagawa ng mga function na hinihiling ng user tulad ng backup / restore at pag-export ng PDF
- Pagbibigay ng mga feature sa seguridad ng app lock
- Pagbibigay ng advertising, pamamahala ng pahintulot, pagpigil sa mapanlinlang na gawain, at pagsunod sa mga legal na obligasyon

---

## 4. Panahon ng Pagpapanatili at Pag-iimbak ng Personal na Impormasyon

- Panloob na data ng app (SQLite, lokal na mga setting, naka-encrypt na mga larawan): nananatili sa device ng user hanggang sa ma-delete ang app, ma-clear ang app data, o direktang ma-delete ng user ang data
- Mga pansamantalang file: dine-delete matapos makumpleto ang kaugnay na gawain o nililinis ayon sa cache policy ng operating system
- Mga file na in-export ng user (mga PDF, backup file): maaaring manatili sa storage location na pinili ng user at kailangang direktang i-delete ng user
- Data na may kaugnayan sa advertising / pahintulot (pinoproseso ng mga third party): nakabatay sa mga patakaran ng bawat service provider at sa mga umiiral na batas

Bilang prinsipyo, hindi iniimbak ng app ang pangunahing mga tala ng user sa server ng developer.  
Gayunpaman, ang mga file na direktang sine-save ng user sa external storage ay pinamamahalaan sa sariling kapaligiran ng user.

---

## 5. Mga Proseso at Paraan ng Pagbura ng Personal na Impormasyon

Kapag natupad na ang layunin ng pagproseso o kapag humiling ang user ng pagbura, buburahin ng app ang kaugnay na impormasyon o ipo-proseso ito upang hindi na ito muling ma-refer, gaya ng sumusunod.

### 5-1) Mga Proseso ng Pagbura

- Kapag direktang binura ng user ang mga indibidwal na tala ng tao, folder, larawan, backup data, atbp., ituturing ang naturang data bilang dapat agad burahin.
- Kapag binura ng user ang app o ni-clear ang app data mula sa settings ng device, ang data na nakaimbak sa internal storage area ng app ay aalisin ayon sa deletion procedures ng operating system.
- Ang mga pansamantalang file ay sasailalim sa paglilinis pagkatapos ng kaugnay na gawain, at ang ilang naka-cache na data ay maaaring manatili hanggang sa isang takdang panahon depende sa patakaran ng operating system.

### 5-2) Mga Paraan ng Pagbura

- SQLite data: pagbura ng mga kaugnay na record
- Mga setting ng app (`SharedPreferences`): pagbura ng kaugnay na key o ng lahat ng settings
- Mga value sa `flutter_secure_storage`: pagbura ng mga kaugnay na secure storage item
- Mga internal na file ng app (mga naka-encrypt na larawan, pansamantalang file, atbp.): pagbura ng mga kaugnay na file
- Mga PDF / backup file na direktang sine-save ng user sa external storage: hindi awtomatikong dine-delete ng app at dapat direktang i-delete ng user

Maliban kung may ibang hinihingi ang mga umiiral na batas, hindi hiwalay na iniimbak ng developer ang pangunahing mga tala ng user sa server ng developer.

---

## 6. Pagbibigay sa Mga Third Party, Outsourcing, at Cross-Border Transfer

Maaaring gumamit ang app ng mga serbisyo ng Google para sa pamamahala ng advertising at pahintulot.

| Item | Detalye |
|---|---|
| **Tatanggap / Pinagkatiwalaang Partido** | Google LLC at mga kaanib nito (mga operator ng AdMob / UMP) |
| **Bansa ng Paglilipatan** | United States at mga rehiyong pinapatakbo ang imprastraktura ng Google |
| **Oras ng Paglilipat** | Patuloy habang may mga ad request, pag-check ng status ng pahintulot, inisyal na pagpapatakbo ng SDK, at operasyon |
| **Paraan ng Paglilipat** | Pagpapadala sa pamamagitan ng network communication sa pagitan ng app at third-party servers |
| **Legal na Batayan para sa Cross-Border Transfer** | Pinoproseso sa saklaw na kinakailangan upang maibigay ang serbisyo alinsunod sa mga umiiral na legal na batayan, o kung kinakailangan, batay sa pahintulot ng data subject |
| **Layunin** | Paghahatid ng ad, pagsukat ng ad, pamamahala ng pahintulot, pag-iwas sa pandaraya, at pagsunod sa mga patakaran / batas |
| **Mga Kategorya ng Data (Mga Halimbawa)** | Mga advertising identifier (AAID / IDFA), impormasyon sa IP / network, impormasyon sa device / app, impormasyon sa interaksiyon sa ad, katayuan ng pahintulot |
| **Panahon ng Pagpapanatili** | Nakabatay sa mga patakaran ng Google at sa mga umiiral na batas |
| **Epekto ng Pagtanggi** | Maaaring malimitahan ang personalized ads, maaaring magpakita ng non-personalized ads, o maaaring malimitahan ang ilang feature na may kaugnayan sa ad |

Hindi kinokolekta o ibinebenta ng developer ang pangunahing data ng talaan ng mga tao sa app sa pamamagitan ng sarili nitong server.

---

## 7. Impormasyon Tungkol sa Mga Pahintulot na Ginagamit

Maaaring gamitin ng app ang mga sumusunod na pahintulot:

- `INTERNET`: komunikasyon para sa mga advertising SDK at kaugnay na network feature
- `com.google.android.gms.permission.AD_ID`: paggamit ng mga advertising identifier (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 at pababa): pag-attach / pagpili ng larawan

Ginagamit lamang ang mga pahintulot sa lawak na kinakailangan upang maibigay ang mga kaugnay na feature.

---

## 8. Pag-install, Operasyon, at Pagtanggi sa Mga Mekanismo ng Awtomatikong Pagkolekta

Ang app na ito ay hindi direktang nagpapatakbo ng karaniwang website cookies.  
Gayunpaman, kaugnay ng mga feature ng advertising at pamamahala ng pahintulot, ang mga third-party SDK ay maaaring awtomatikong magproseso ng mga advertising identifier, impormasyon ng network, impormasyon ng device, at kahalintulad na data.

Maaaring ayusin ng mga user ang mga kaugnay na setting sa mga sumusunod na paraan:

- Baguhin ang mga pinili sa loob ng privacy options ng app o consent management screen (kung mayroon)
- I-reset o i-delete ang advertising ID sa settings ng operating system ng device
- Limitahan ang personalized ads o ayusin ang mga kaugnay na privacy option sa settings ng operating system ng device

Kung lilimitahan ng user ang personalized advertising, maaaring magpakita ng non-personalized ads o maaaring malimitahan ang ilang feature na may kaugnayan sa ad.

---

## 9. Mga Karapatan ng User at Paano Ito Gagamitin

Alinsunod sa mga umiiral na batas, maaaring mayroon ang mga user ng mga sumusunod na karapatan:

- Humiling ng access sa, pagwawasto ng, o pagbura ng personal na impormasyon
- Humiling ng pagsuspinde o paghihigpit sa pagproseso
- Bawiin ang pahintulot para sa pagproseso na nakabatay sa pahintulot
- Baguhin ang mga piniling opsyon sa advertising / pahintulot

Maaaring gamitin ang mga karapatang ito sa mga sumusunod na paraan:

- Direktang baguhin o burahin ang data sa loob ng app
- I-initialize ang lokal na data sa pamamagitan ng pag-delete ng app data o pag-uninstall ng app
- Baguhin ang pahintulot sa advertising sa pamamagitan ng privacy options / consent screen ng app (sa mga rehiyong mayroon nito)
- I-reset / i-delete ang advertising ID o limitahan ang personalized ads sa pamamagitan ng settings ng OS ng device
- Contact: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Mga Panukalang Pangseguridad

Ipinatutupad o sinisikap ipatupad ng developer ang mga sumusunod na hakbang:

- Ang mga tala ng user ay karaniwang lokal na iniimbak sa device
- Ang mga naka-attach na image file ay lokal na iniimbak sa naka-encrypt na anyo (nakabatay sa AES-GCM)
- Ang impormasyon ng app lock ay iniimbak sa hashed form sa halip na plain text
- Ang mga backup file ay iniimbak pagkatapos ma-encrypt batay sa password ng user
- Ang komunikasyon sa mga third-party SDK ay naka-encrypt (HTTPS / TLS)
- Ginagamit ang mga pahintulot nang may pinakamababang saklaw ng access na kinakailangan

Gayunpaman, ang mga panganib na nagmumula sa kalagayan ng seguridad ng device ng user (tulad ng rooting / jailbreaking, mga mapaminsalang app, o exposure ng shared storage) ay hindi ganap na maaalis.

---

## 11. Impormasyon Tungkol sa Sensitibong Impormasyon

Hindi hinihingi ng app na ito ang pag-input ng sensitibong impormasyon.  
Pinapayuhan ang mga user na huwag maglagay ng sensitibong nilalaman tulad ng impormasyong pangkalusugan, mga pananaw pampolitika, relihiyon, biometric na impormasyon, o impormasyong may kaugnayan sa buhay sekswal sa mga tala o free-input field.

Kung boluntaryong maglalagay ang user ng sensitibong nilalaman, maaaring maimbak ang naturang impormasyon bilang lokal na data sa device na direktang pinamamahalaan ng user.

---

## 12. Proteksiyon ng Personal na Impormasyon ng mga Bata

Ang app na ito ay hindi pangunahing idinisenyo para sa mga bata.  
Maaaring pamahalaan ng mga guardian ang paggamit sa pamamagitan ng parental control features na ibinibigay ng device o app store.

---

## 13. Awtomatikong Pagpapasya

Ang app na ito ay hindi nagsasagawa ng awtomatikong pagpapasya batay sa personal na impormasyon na nagdudulot ng legal na epekto o katulad na mahalagang epekto.

---

## 14. Paunawa sa Kaligtasan ng Data (Google Play, atbp.)

Nagsisikap ang developer na panatilihin at i-update ang mga item sa pagsisiwalat ng kaligtasan ng data sa mga app marketplace (tulad ng Google Play) alinsunod sa aktuwal na mga gawain sa pagproseso ng app at sa aktuwal na mga gawain sa pagproseso ng mga third-party SDK.

Gayunpaman, ang impormasyong ipinapakita sa mga app store ay maaaring mag-iba depende sa bersyon ng app, bansang pinamamahagian, configuration ng third-party SDK, at mga pagbabago sa patakaran.

---

## 15. Paunawa sa Open Source

Gumagamit ang app ng ilang open-source library.  
Ang impormasyon tungkol sa mga kaugnay na lisensya ay maaaring makita sa kaugnay na screen sa loob ng app o sa mga paunawang ibinibigay sa pamamagitan ng distribution channel.

---

## 16. Contact

Para sa mga katanungang may kaugnayan sa Patakaran sa Privacy na ito:

- **Opisyal sa Proteksiyon ng Personal na Impormasyon / Taong Maaaring Kontakin:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 17. Mga Pagbabago sa Patakaran sa Privacy na Ito

Maaaring baguhin ang Patakarang ito dahil sa mga pagbabago sa mga batas / patakaran, mga feature ng app, o mga third-party SDK.  
Kung may mahahalagang pagbabago, maaaring magbigay ng paunawa sa pamamagitan ng mga in-app notice, ng distribution page, o ng mga update sa policy page.

Huling Na-update: **2026-03-04**
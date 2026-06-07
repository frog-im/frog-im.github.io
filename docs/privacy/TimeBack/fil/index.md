---
title: Patakaran sa Privacy | TimeBack
description: Patakaran sa Privacy ng TimeBack
lang: fil
last_updated: 2026-06-06
---

# Patakaran sa Privacy (TimeBack)

- **Pangalan ng app:** TimeBack
- **Developer:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Petsa ng bisa:** 2026-06-03
- **Huling na-update:** 2026-06-06

Ang Patakaran sa Privacy na ito ay batay sa kasalukuyang pagpapatupad ng TimeBack app. Nagbibigay ang TimeBack ng pagsusuri sa screen-time, pang-araw-araw na layunin, mga reclaimed-time na tala, pagmumuni-muni, hamon, notification, pagbabahagi, at mga feature sa advertising.

## 1. Mga Tampok

Nagbibigay ang TimeBack ng mga sumusunod na tampok:

- Pagsusuri sa oras ng paggamit ng app sa pamamagitan ng pahintulot sa pag-access sa paggamit ng Android
- Mga layunin sa pang-araw-araw na paggamit, mga paalala, at mga notification sa paggamit ng status-bar
- Hard-limit na mga notification ng babala at overlay na display
- Overlay exception app selection
- Reclaimed-time na mga tala ng aktibidad
- Pang-araw-araw na mga tala ng pagmuni-muni
- Hamunin ang pag-unlad at pamamahala ng checklist
- Pagbabahagi ng larawan sa istatistika ng paggamit
- Mga Google AdMob ad at UMP-based na mga opsyon sa privacy

## 2. Impormasyong Pinoproseso Namin

### 2-1. Pahintulot sa Pag-access sa Paggamit ng Impormasyon

Kung bibigyan ng user ang Android `PACKAGE_USAGE_STATS` ng pahintulot, maaaring basahin ng app ang sumusunod na impormasyon mula sa device:

- Pangalan ng package ng app
- Pangalan ng app
- Oras ng paggamit ng app
- Saklaw ng petsa at oras na ginamit para sa pagsasama-sama ng paggamit

Ginagamit ang impormasyong ito upang magbigay ng mga istatistika ng paggamit at paghambingin ang paggamit laban sa mga layunin ng user.

### 2-2. Impormasyong Inilagay o Na-configure ng User

- Pang-araw-araw na layunin sa paggamit
- Pinagana ang paalala sa paggamit ng estado at pagitan
- Setting ng pagpapakita ng paggamit ng status-bar
- Reclaimed-time na kategorya ng aktibidad, pamagat, oras ng pagsisimula, at tagal
- Pang-araw-araw na repleksyon na teksto
- Hamunin ang pag-unlad at mga entry sa checklist
- Listahan ng app ng pagbubukod ng overlay

### 2-3. Impormasyon na Nakaimbak sa Device

Maaaring iimbak ng app ang sumusunod na impormasyon sa isang lokal na database ng SQLite o SharedPreferences:

- Mga tala sa oras ng paggamit ng app
- Pang-araw-araw na layunin at setting
- Reclaimed-time na mga tala ng aktibidad
- Pang-araw-araw na mga tala ng pagmuni-muni
- Hamunin ang pag-unlad at estado ng checklist
- Katayuan ng pagkumpleto ng onboarding
- Mga setting gaya ng mga paalala sa paggamit, mga hard-limit na babala, display ng status-bar, at mga app ng pagbubukod sa overlay
- Pahintulot ng lokal na ad at estado ng opsyon sa privacy

Batay sa kasalukuyang pagpapatupad, ang mga lokal na tala na ito ay hindi awtomatikong ina-upload sa mga server ng frog-im.

### 2-4. Data ng Advertising at Pahintulot

Kapag ginamit ang Google Mobile Ads SDK (AdMob) at UMP, maaaring iproseso ng Google o ng mga kaakibat nito ang impormasyon gaya ng:

- Mga identifier sa advertising, gaya ng Android AD_ID
- IP address at impormasyon ng network
- Impormasyon ng device, OS na bersyon, at impormasyon ng app
- Mga ad impression, pag-click, data ng pagsukat, at mga signal ng error
- Pahintulot sa ad at estado ng opsyon sa privacy
- Tinatayang lokasyon

## 3. Mga Layunin ng Pagproseso

Pinoproseso ng app ang impormasyon para sa mga sumusunod na layunin:

- Pagbabasa ng oras ng paggamit, pagpapakita ng mga istatistika, at paghahambing ng paggamit laban sa mga layunin
- Pag-iimbak ng reclaimed-time at reflection record na ipinasok ng user
- Pamamahala ng pag-unlad ng hamon
- Nagbibigay ng mga paalala at notification sa status-bar
- Nagbibigay ng hard-limit na mga notification ng babala, overlay display, at overlay exception handling
- Pagbabahagi ng mga larawan sa istatistika ng paggamit kapag hiniling ng user
- Paghahatid ng mga ad, pagsukat ng pagganap ng ad, at paglalapat ng mga pagpipilian sa pagpapahintulot sa ad
- Pagpapanatili ng katatagan ng app at pagtugon sa mga error

## 4. Lokal na Imbakan at Panlabas na Pagproseso

### 4-1. Lokal na Imbakan

Iniimbak ng TimeBack ang data ng user pangunahin sa panloob na storage ng app sa device. Batay sa kasalukuyang pagpapatupad, ang mga talaan ng paggamit, layunin, pagmumuni-muni, at impormasyon ng hamon ay hindi awtomatikong ina-upload sa mga server ng frog-im.

Maaaring kabilang sa lokal na imbakan ang mga sumusunod.

| Imbakan | Mga bagay na nakaimbak | Layunin | Paraan ng pagtanggal |
|---|---|---|---|
| SQLite database | Mga talaan ng paggamit ng app, mga pangalan ng package, mga pangalan ng app, oras ng paggamit, mga pinagsama-samang batay sa petsa | Ipakita ang mga istatistika ng paggamit at ihambing ang paggamit sa mga layunin | Mga feature sa pagtanggal ng in-app, pag-clear ng data ng app, o pag-uninstall ng app |
| SQLite database | Reclaimed-time na mga aktibidad, pagmumuni-muni, pag-unlad ng hamon, mga entry sa checklist | Ipakita ang mga tala at pamahalaan ang pag-unlad | Mga feature sa pagtanggal ng in-app, pag-clear ng data ng app, o pag-uninstall ng app |
| SharedPreferences | Katayuan ng pagkumpleto ng onboarding, mga setting ng paalala, mga setting ng hard-limit na babala, mga setting ng pagpapakita ng status-bar, listahan ng app ng pagbubukod sa overlay, estado ng lokal na pahintulot sa ad | Panatilihin ang mga setting ng app | Pag-clear ng data ng app o pag-uninstall ng app |
| Pansamantalang mga file/cache | Nakabahaging mga larawan sa istatistika ng paggamit at mga katulad na pansamantalang file | Magsagawa ng pagbabahagi na hiniling ng user | Na-delete pagkatapos ibahagi kung posible, o ayon sa OS/mga patakaran sa paglilinis ng app |

Kapag na-clear ng user ang data ng app o na-uninstall ang app, karaniwang tinatanggal ang data na nakaimbak sa internal storage ng app. Gayunpaman, ang backup ng Android, backup ng manufacturer, cloud backup, o mga file na direktang ibinahagi ng user ay maaaring panatilihing hiwalay ayon sa mga patakaran ng mga serbisyong iyon.

Ang mga talaan ng paggamit at teksto ng pagmumuni-muni ay maaaring magbunyag ng mga personal na gawain o interes. Sa mga nakabahaging device, dapat gumamit ang mga user ng mga naaangkop na pananggalang gaya ng lock ng device o hiwalay na OS account.

### 4-2. Mga Pag-upload ng Server

Batay sa kasalukuyang proyekto, ang TimeBack ay hindi awtomatikong nag-a-upload ng mga talaan ng paggamit, pagmumuni-muni, o mga talaan ng hamon sa mga server ng frog-im. Kung ginagamit ng user ang feature sa pagbabahagi, maaaring ilipat ang isang nabuong larawan ng istatistika sa external na app o serbisyong pinili ng user.

### 4-3. Pagproseso ng Advertising

Ginagamit ang Google AdMob at UMP para sa in-app na advertising at pamamahala ng pahintulot. Maaaring iproseso ang impormasyong nauugnay sa advertising sa imprastraktura ng Google.

## 5. Mga Serbisyo at Processor ng Third-party

### 5-1. Google AdMob / UMP

Layunin:

- Paghahatid ng banner ad
- Pahintulot sa ad at paghawak ng opsyon sa privacy
- Pagsusukat sa pagganap ng ad at pag-iwas sa panloloko

Impormasyon na maaaring iproseso:

- Mga pagkakakilanlan sa advertising
- Impormasyon ng device at network
- Impormasyon sa pakikipag-ugnayan ng ad
- Pahintulot at estado ng opsyon sa privacy

### 5-2. Pagbabahagi ng Mga Target na App o Serbisyo

Kung direktang ginagamit ng user ang feature sa pagbabahagi ng larawan sa istatistika ng paggamit, maaaring iproseso ng napiling external na app o serbisyo ang nakabahaging larawan. Ang pagproseso na iyon ay pinamamahalaan ng patakaran sa privacy ng napiling serbisyo.

## 6. Paunawa sa Paglipat ng Cross-Border

Maaaring iproseso ang impormasyon sa labas ng bansa ng gumagamit sa mga sumusunod na kaso.

| item | Mga Detalye |
|---|---|
| tatanggap | Google LLC at mga kaakibat nito |
| Patutunguhan | United States at iba pang mga bansa/rehiyon kung saan matatagpuan ang imprastraktura ng Google |
| Timing | Kapag tumakbo ang app, humiling ng mga ad, nagpapakita o sumusukat ng mga ad, nagpoproseso ng mga pag-click, o humahawak ng pahintulot |
| Pamamaraan | Naka-encrypt na komunikasyon sa network (HTTPS/TLS) |
| Layunin | Paghahatid ng ad, paghawak sa estado ng pag-personalize, pagsukat, analytics, pagpapabuti ng katatagan ng serbisyo, legal na pagsunod |
| Data | Mga identifier sa pag-advertise, impormasyon ng device/app/network, impormasyon sa pakikipag-ugnayan sa ad, estado ng pahintulot, tinatayang lokasyon, atbp. |
| Pagpapanatili | Alinsunod sa mga patakaran at naaangkop na batas ng Google |

Para sa mga detalye, pakitingnan ang [Cross-Border Transfer Notice](./policy/).

## 7. Naka-install na Listahan ng App at Mga Pagbubukod sa Overlay

Sa Android, kung iko-configure ng user ang mga app ng pagbubukod sa overlay, maaaring basahin ng app ang mga pangalan ng package at mga pangalan ng app ng mga mailulunsad na app sa device upang magpakita ng listahan ng pagpili. Ang mga pangalan ng package na pinili ng user bilang mga exception ay naka-store sa SharedPreferences sa device at ginagamit lang ito para maiwasan ang pagpapakita ng mga overlay ng babala na may hard-limit sa ibabaw ng mga app na iyon.

## 8. Pagpapanatili

Ang app ay nagpapanatili ng impormasyon sa ilalim ng mga sumusunod na pamantayan:

- Lokal na paggamit, layunin, pagmuni-muni, at impormasyon ng hamon: hanggang sa i-delete ito ng user, i-clear ang data ng app, o i-uninstall ang app
- Mga setting ng SharedPreferences: hanggang sa i-clear ng user ang data ng app o i-uninstall ang app
- Mga pansamantalang file para sa mga nakabahaging larawan: kung kinakailangan para sa pagbabahagi o ayon sa OS na mga patakaran sa paglilinis
- Data na nauugnay sa advertising at pahintulot: ayon sa mga patakaran ng Google at iba pang nauugnay na third party

## 9. Mga Pahintulot

Maaaring gamitin ng app ang mga sumusunod na pahintulot:

- `PACKAGE_USAGE_STATS`: basahin ang oras ng paggamit ng app
- `POST_NOTIFICATIONS`: ipakita ang mga paalala sa paggamit at mga notification sa status-bar
- `SYSTEM_ALERT_WINDOW`: magpakita ng mga hard-limit na overlay ng babala
- `INTERNET`: makipag-ugnayan sa mga ad SDKs at magpakita ng mga pahina ng legal na notice
- `ACCESS_NETWORK_STATE`: tingnan ang katayuan ng network
- `com.google.android.gms.permission.AD_ID`: gumamit ng mga identifier ng advertising

Ginagamit lang ang mga pahintulot kung kinakailangan para sa mga feature ng app. Maaaring bawiin ng mga user ang mga pahintulot sa mga setting ng device, ngunit maaaring limitado ang mga nauugnay na feature.

## 10. Mga Karapatan at Pagpipilian ng User

Ang mga gumagamit ay maaaring:

- Tingnan, i-edit, o tanggalin ang mga tala sa loob ng app
- Tanggalin ang lokal na impormasyon sa pamamagitan ng pag-clear sa data ng app o pag-uninstall sa app
- Baguhin ang access sa paggamit, notification, at mga setting ng pagkakakilanlan ng advertising sa mga setting ng device
- Bawiin ang pahintulot sa overlay at baguhin ang mga setting ng app ng pagbubukod ng overlay
- Baguhin ang mga opsyon sa privacy ng ad
- Makipag-ugnayan sa amin para sa mga tanong sa privacy o mga kahilingan sa pagtanggal

Email sa pakikipag-ugnayan: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Mga Panukala sa Seguridad

Nalalapat o maaaring ilapat ng app ang mga sumusunod na pananggalang:

- HTTPS/TLS-based na panlabas na komunikasyon
- Lokal-unang pagpoproseso ng data
- Kinakailangan ang mga minimum na kahilingan sa pahintulot para sa mga feature ng app
- Paglalapat ng estado ng pahintulot sa advertising

Ang mga kundisyon sa seguridad ng device gaya ng pag-rooting, pag-jailbreak, malware, o paggamit ng shared-device ay maaaring lumikha ng mga karagdagang panganib.

## 12. Privacy ng mga Bata

Ang TimeBack ay hindi pangunahing idinisenyo para sa mga bata. Ang mga setting na nauugnay sa edad o mga patakaran sa platform ng Google Mobile Ads SDK at UMP ay maaaring malapat sa panahon ng pag-advertise at pagpoproseso ng pahintulot.

## 13. Mga Pagbabago

Maaaring ma-update ang Patakaran na ito dahil sa mga pagbabago sa batas, configuration ng serbisyo ng third-party, o mga feature ng app. Aabisuhan ang mga pagbabago sa materyal sa pamamagitan ng in-app na abiso o sa pamamagitan ng pag-update sa page na ito.

## 14. Makipag-ugnayan

- Nag-develop: frog-im
- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

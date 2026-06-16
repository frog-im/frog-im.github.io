---
title: Patakaran sa Privacy | Lucky Pick Box
description: Lucky Pick Box Patakaran sa Privacy
lang: fil
last_updated: 2026-06-15
---

# Patakaran sa Privacy (Lucky Pick Box / 뽑기박스)

- **Pangalan ng App:** Lucky Pick Box / 뽑기박스
- **Developer:** frog-im
- **Opisyal sa Proteksiyon ng Personal na Impormasyon / Taong Maaaring Kontakin:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Petsa ng Pagkakabisa:** 2026-06-12
- **Huling Na-update:** 2026-06-15

> Inihanda ang Patakarang ito batay sa impormasyong pinoproseso ng app at sa mga kaugnay nitong feature.  
> Kung may anumang sapilitang batas o regulasyon na nalalapat sa isang partikular na bansa o rehiyon, maaaring manaig ang naturang mga batas o regulasyon.

---

## 1. Layunin at Saklaw

Ang Lucky Pick Box ay kaswal na tool para sa random na pagpili, bunutan, pagpili ng pagkakasunod-sunod, paghahati ng team, dice, coin, ladder, wheel, at katulad na pang-araw-araw o panggrupong decision games. Hindi nagbibigay ang app ng real-money gambling, pagtaya, financial transactions, cash prizes, o cash-equivalent rewards.

### A. Mga pangunahing feature

- Quick input: text na tina-type ng user o nabasa mula sa piniling larawan.
- Random choice games: ladder, wheel, plinko, simple draw, dice, coin, random number, team splitter, order picker, card, bomb, at yes/no.
- Result history: maaaring i-save ang game type, title, participants/items, result summary, at creation time.
- Setting slots: maaaring i-save ng ilang laro ang participants, lists, ranges, quantities, teams, weights, at katulad na settings sa hanggang 3 local slots.

Hindi nangangailangan ang app ng sign-up o login. Wala kaming server na tumatanggap mula sa app ng iyong pangalan, numero ng telepono, email address, contacts, game entries, napiling mga larawan, o game results.

Para maibigay ang mga feature, maaaring mag-store ang app sa local storage ng iyong device ng game entries, participant labels, recent results, saved game settings, animation settings, ad privacy choices, at consent-related state. Nililimitahan ng app ang recent result history at hindi ito ipinapadala sa server na pinapatakbo ng developer.

---

## 2. Mga Kategorya ng Personal na Impormasyong Pinoproseso

### 2-1) Impormasyong Direktang Inilalagay ng User

Hindi nangangailangan ang app ng sign-up o login. Wala kaming server na tumatanggap mula sa app ng iyong pangalan, numero ng telepono, email address, contacts, game entries, napiling mga larawan, o game results.

### 2-2) Mga File na Pinili sa Device

Kung pipiliin mong magbasa ng text mula sa larawan, hihilingin ng app na pumili ka ng larawan mula sa photo library. Ginagamit ang napiling larawan para sa on-device text recognition sa pamamagitan ng platform image picker at Google ML Kit text recognition components. Hindi ina-upload ng developer ang larawan sa server na pinapatakbo ng developer at hindi ito iniimbak sa remote account.

### 2-3) Data na Lokal na Iniimbak sa Loob ng App

Para maibigay ang mga feature, maaaring mag-store ang app sa local storage ng iyong device ng game entries, participant labels, recent results, saved game settings, animation settings, ad privacy choices, at consent-related state. Nililimitahan ng app ang recent result history at hindi ito ipinapadala sa server na pinapatakbo ng developer.

### B. Local data sa device

| Lokasyon o key | Data | Layunin | Pag-delete |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, game type, title, participants/items, summary, time; hanggang 50 recent results. | Ipakita ang recent results at history. | In-app history deletion, clear app data, o uninstall |
| `game_settings.<gameId>.slot_<n>` | Game settings, saved time, lists, ranges, quantities, teams, weights; hanggang 3 slots. | I-load muli ang game settings. | Clear slot, clear app data, o uninstall |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Animation at fullscreen settings. | Panatilihin ang display preferences. | Baguhin settings, clear data, o uninstall |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Ad privacy choices at ad frequency count. | Ilapat ang regional choices at kontrolin ang frequency. | Baguhin settings, clear data, o uninstall |
| Image picker at OCR | Maaaring pansamantalang iproseso ang path ng piniling image at recognized text. | Idagdag ang image text sa quick input. | App/OS cache o data deletion |

Hindi ipinapadala ang quick input text sa server ng developer. Maaari lamang itong maging local data kung ginamit sa game result o saved setting.

### 2-4) Impormasyong Maaaring Awtomatikong Maproseso sa Panahon ng Advertising at Pamamahala ng Pahintulot

Sa supported platforms, kasalukuyang Android, gumagamit ang app ng Google AdMob at Google User Messaging Platform (UMP). Maaaring iproseso ng Google at advertising partners ang advertising identifiers, app instance identifiers, IP address, approximate location, device at network information, app version, operating system, language, ad impressions, clicks at interactions, diagnostics, consent status, at regional ad privacy settings para sa ad delivery, frequency capping, fraud prevention, consent management, measurement, analytics, security, at legal compliance.

Inilalarawan ang privacy practices ng Google sa https://policies.google.com/privacy at https://policies.google.com/technologies/ads.

---

## 3. Layunin ng Pagproseso ng Personal na Impormasyon

Ang Lucky Pick Box ay kaswal na tool para sa random na pagpili, bunutan, pagpili ng pagkakasunod-sunod, paghahati ng team, dice, coin, ladder, wheel, at katulad na pang-araw-araw o panggrupong decision games. Hindi nagbibigay ang app ng real-money gambling, pagtaya, financial transactions, cash prizes, o cash-equivalent rewards.

### A. Mga pangunahing feature

- Quick input: text na tina-type ng user o nabasa mula sa piniling larawan.
- Random choice games: ladder, wheel, plinko, simple draw, dice, coin, random number, team splitter, order picker, card, bomb, at yes/no.
- Result history: maaaring i-save ang game type, title, participants/items, result summary, at creation time.
- Setting slots: maaaring i-save ng ilang laro ang participants, lists, ranges, quantities, teams, weights, at katulad na settings sa hanggang 3 local slots.

Sa supported platforms, kasalukuyang Android, gumagamit ang app ng Google AdMob at Google User Messaging Platform (UMP). Maaaring iproseso ng Google at advertising partners ang advertising identifiers, app instance identifiers, IP address, approximate location, device at network information, app version, operating system, language, ad impressions, clicks at interactions, diagnostics, consent status, at regional ad privacy settings para sa ad delivery, frequency capping, fraud prevention, consent management, measurement, analytics, security, at legal compliance.

Inilalarawan ang privacy practices ng Google sa https://policies.google.com/privacy at https://policies.google.com/technologies/ads.

---

## 4. Panahon ng Pagpapanatili at Pag-iimbak ng Personal na Impormasyon

Maaaring manatili ang local history at settings sa iyong device hanggang burahin mo ang history, i-clear ang app data, o i-uninstall ang app. Maaari mong baguhin ang available ad privacy choices sa app settings, buksan ang Google privacy options kung kinakailangan, at i-manage o i-reset ang advertising identifiers sa privacy settings ng device. Ang retention ng impormasyong pinoproseso ng Google ay pinamamahalaan ng policies at legal obligations ng Google.

### B. Local data sa device

| Lokasyon o key | Data | Layunin | Pag-delete |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, game type, title, participants/items, summary, time; hanggang 50 recent results. | Ipakita ang recent results at history. | In-app history deletion, clear app data, o uninstall |
| `game_settings.<gameId>.slot_<n>` | Game settings, saved time, lists, ranges, quantities, teams, weights; hanggang 3 slots. | I-load muli ang game settings. | Clear slot, clear app data, o uninstall |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Animation at fullscreen settings. | Panatilihin ang display preferences. | Baguhin settings, clear data, o uninstall |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Ad privacy choices at ad frequency count. | Ilapat ang regional choices at kontrolin ang frequency. | Baguhin settings, clear data, o uninstall |
| Image picker at OCR | Maaaring pansamantalang iproseso ang path ng piniling image at recognized text. | Idagdag ang image text sa quick input. | App/OS cache o data deletion |

Hindi ipinapadala ang quick input text sa server ng developer. Maaari lamang itong maging local data kung ginamit sa game result o saved setting.

---

## 5. Mga Proseso at Paraan ng Pagbura ng Personal na Impormasyon

Maaaring manatili ang local history at settings sa iyong device hanggang burahin mo ang history, i-clear ang app data, o i-uninstall ang app. Maaari mong baguhin ang available ad privacy choices sa app settings, buksan ang Google privacy options kung kinakailangan, at i-manage o i-reset ang advertising identifiers sa privacy settings ng device. Ang retention ng impormasyong pinoproseso ng Google ay pinamamahalaan ng policies at legal obligations ng Google.

### C. Permissions, SDK, backups, at security

Maaaring gamitin ng app ang `INTERNET`, `ACCESS_NETWORK_STATE`, at `com.google.android.gms.permission.AD_ID` para sa ads at legal notices. Ginagamit lamang ang photo access o image picker kapag pinili ng user na magbasa ng text mula sa image.

Maaaring iproseso ng Google Mobile Ads SDK ang IP address, ad interactions, diagnostics, at device/account identifiers para sa ads, analytics, at fraud prevention. Maaaring iproseso ng UMP ang consent status at privacy choices.

Maaaring burahin ang local data sa pamamagitan ng in-app delete features, OS app-data deletion, o uninstall. Maaaring manatili ang system backups, screenshots, o files na ibinahagi ng user ayon sa policy ng provider. Iwasang maglagay ng sensitive data sa free-text fields.

---

## 6. Pagbibigay sa Mga Third Party, Outsourcing, at Cross-Border Transfer

Hindi namin ibinebenta ang iyong game entries, participant labels, game results, o napiling mga larawan. Kapag humihiling ng ads o consent features, maaaring iproseso ng Google LLC, Google affiliates, at kanilang service providers ang advertising at consent information sa mga bansang nasa labas ng iyong bansa o rehiyon. Tingnan ang "Abiso sa Internasyonal na Paglipat ng Data" sa app para sa karagdagang detalye.

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

---

## 7. Impormasyon Tungkol sa Mga Pahintulot na Ginagamit

### C. Permissions, SDK, backups, at security

Maaaring gamitin ng app ang `INTERNET`, `ACCESS_NETWORK_STATE`, at `com.google.android.gms.permission.AD_ID` para sa ads at legal notices. Ginagamit lamang ang photo access o image picker kapag pinili ng user na magbasa ng text mula sa image.

Maaaring iproseso ng Google Mobile Ads SDK ang IP address, ad interactions, diagnostics, at device/account identifiers para sa ads, analytics, at fraud prevention. Maaaring iproseso ng UMP ang consent status at privacy choices.

Maaaring burahin ang local data sa pamamagitan ng in-app delete features, OS app-data deletion, o uninstall. Maaaring manatili ang system backups, screenshots, o files na ibinahagi ng user ayon sa policy ng provider. Iwasang maglagay ng sensitive data sa free-text fields.

---

## 8. Pag-install, Operasyon, at Pagtanggi sa Mga Mekanismo ng Awtomatikong Pagkolekta

Sa supported platforms, kasalukuyang Android, gumagamit ang app ng Google AdMob at Google User Messaging Platform (UMP). Maaaring iproseso ng Google at advertising partners ang advertising identifiers, app instance identifiers, IP address, approximate location, device at network information, app version, operating system, language, ad impressions, clicks at interactions, diagnostics, consent status, at regional ad privacy settings para sa ad delivery, frequency capping, fraud prevention, consent management, measurement, analytics, security, at legal compliance.

Inilalarawan ang privacy practices ng Google sa https://policies.google.com/privacy at https://policies.google.com/technologies/ads.

Maaaring manatili ang local history at settings sa iyong device hanggang burahin mo ang history, i-clear ang app data, o i-uninstall ang app. Maaari mong baguhin ang available ad privacy choices sa app settings, buksan ang Google privacy options kung kinakailangan, at i-manage o i-reset ang advertising identifiers sa privacy settings ng device. Ang retention ng impormasyong pinoproseso ng Google ay pinamamahalaan ng policies at legal obligations ng Google.

---

## 9. Mga Karapatan ng User at Paano Ito Gagamitin

Maaaring manatili ang local history at settings sa iyong device hanggang burahin mo ang history, i-clear ang app data, o i-uninstall ang app. Maaari mong baguhin ang available ad privacy choices sa app settings, buksan ang Google privacy options kung kinakailangan, at i-manage o i-reset ang advertising identifiers sa privacy settings ng device. Ang retention ng impormasyong pinoproseso ng Google ay pinamamahalaan ng policies at legal obligations ng Google.

---

## 10. Mga Panukalang Pangseguridad

### C. Permissions, SDK, backups, at security

Maaaring gamitin ng app ang `INTERNET`, `ACCESS_NETWORK_STATE`, at `com.google.android.gms.permission.AD_ID` para sa ads at legal notices. Ginagamit lamang ang photo access o image picker kapag pinili ng user na magbasa ng text mula sa image.

Maaaring iproseso ng Google Mobile Ads SDK ang IP address, ad interactions, diagnostics, at device/account identifiers para sa ads, analytics, at fraud prevention. Maaaring iproseso ng UMP ang consent status at privacy choices.

Maaaring burahin ang local data sa pamamagitan ng in-app delete features, OS app-data deletion, o uninstall. Maaaring manatili ang system backups, screenshots, o files na ibinahagi ng user ayon sa policy ng provider. Iwasang maglagay ng sensitive data sa free-text fields.

### C. Permissions, SDK, backups, at security

Maaaring gamitin ng app ang `INTERNET`, `ACCESS_NETWORK_STATE`, at `com.google.android.gms.permission.AD_ID` para sa ads at legal notices. Ginagamit lamang ang photo access o image picker kapag pinili ng user na magbasa ng text mula sa image.

Maaaring iproseso ng Google Mobile Ads SDK ang IP address, ad interactions, diagnostics, at device/account identifiers para sa ads, analytics, at fraud prevention. Maaaring iproseso ng UMP ang consent status at privacy choices.

Maaaring burahin ang local data sa pamamagitan ng in-app delete features, OS app-data deletion, o uninstall. Maaaring manatili ang system backups, screenshots, o files na ibinahagi ng user ayon sa policy ng provider. Iwasang maglagay ng sensitive data sa free-text fields.

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

Huling Na-update: **2026-06-15**

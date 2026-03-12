---
title: Patakaran sa Privacy | Subtitle Tool
description: Patakaran sa Privacy ng Subtitle Tool (Subtitle Player & Editor) - Filipino
lang: fil
last_updated: 2026-03-11
---

# Patakaran sa Privacy (Subtitle Tool / Subtitle Player & Editor)

- **Pangalan ng app:** Subtitle Player & Editor (tinatawag ding **Subtitle Tool** sa Patakarang ito)
- **Developer:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Petsa ng Pagkakabisa:** 2026-03-11

> Ang Patakarang ito ay inihanda bilang pagtukoy sa mga naaangkop na batas, kabilang ang Korean Personal Information Protection Act (PIPA), GDPR / UK GDPR, Swiss FADP, at mga kaugnay na batas sa privacy ng mga estado sa U.S. Kung may umiiral na mga sapilitang lokal na tuntunin, ang mga tuntuning iyon ang mangingibabaw.

---

## 1. Layunin at Saklaw

Nagbibigay ang app na ito ng mga sumusunod:

- Pag-play at pag-edit ng subtitle
- Pag-play ng video + subtitle mula sa mga file na pinili ng user
- Lumulutang na subtitle / lyrics overlay na ipinapakita sa ibabaw ng ibang apps sa Android

Maaaring kabilang sa suportadong paghawak ng subtitle ang mga format tulad ng:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

Ang app ay **hindi** gumagawa ng user account at **hindi** nag-a-upload ng subtitle o media files ng user sa sariling servers ng developer. Ang pag-parse, pag-edit, pag-preview ng subtitle, at karamihan ng processing na may kaugnayan sa playback ay ginagawa **lokal sa device**.

Gayunpaman, para sa advertising, consent management, at legal compliance, ang third-party SDKs tulad ng **Google Mobile Ads SDK (AdMob)** at **Google UMP** ay maaaring magproseso ng ilang impormasyon gaya ng advertising identifiers, device signals, at consent choices.

---

## 2. Mga Kategorya ng Impormasyong Pinoproseso Namin

### 2-1) Mga File na Tahasang Pinili ng User

Nakikipag-ugnayan ang app sa mga file na tahasang pinipili ng user, kabilang ang:

- **Mga subtitle file**
  - Mga halimbawa: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Mga gamit:
    - Pag-play ng subtitle sa loob ng app
    - Pag-edit ng subtitle
    - Pagpapakita ng overlay subtitle
    - Subtitle conversion at export

- **Mga media file**
  - Mga halimbawa: lokal na video o audio files na pinili ng user
  - Mga gamit:
    - Video + subtitle playback
    - Pag-aayos ng overlay timing ayon sa kasalukuyang pinapatugtog na media

Mahahalagang punto:

- Ang mga file na pinili ng user ay pinoproseso nang lokal sa device.
- Hindi ina-upload ng app ang mga file na iyon sa sariling servers ng developer.
- Ang file paths at contents ay ginagamit lamang para sa playback, overlay, editing, saving, at mga aksyong hinihiling ng user.

### 2-2) Mga Lokal na Setting at Nakaimbak na Halaga

Upang magbigay ng persistent settings at maibalik ang dating estado, nag-iimbak ang app ng ilang halaga nang lokal sa device gamit ang `SharedPreferences` o katulad na local storage na ibinibigay ng OS.

Ang mga halagang ito ay hindi ipinapadala sa sariling servers ng developer at karaniwang nabubura kapag na-clear ang app data o na-uninstall ang app.

#### (1) Mga setting ng overlay

Kabilang sa mga halimbawa ang:

- `overlay_box_x`
- `overlay_box_y`
- `overlay_text_font`
- `overlay_text_color`
- `overlay_outline_enabled`
- `overlay_outline_color`
- `overlay_outline_width`
- `overlay_force_landscape`
- `overlay_interstitial_count`

Layunin:

- Ibalik ang posisyon ng overlay
- Ibalik ang estilo ng subtitle para sa overlay at in-app subtitle playback
- Panatilihin ang mga preference sa outline / font / orientation
- Kontrolin ang logic ng dalas ng pagpapakita ng ads sa ilang overlay-related flows

#### (2) Mga kamakailang playback o overlay position

Kabilang sa mga halimbawa ang:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Layunin:

- Ibalik o imungkahi ang mga kamakailang panimulang posisyon ng subtitle/overlay
- Ipagpatuloy ang video + subtitle playback nang mas maginhawa

#### (3) Mga halaga ng preference para sa ads at privacy

Maaaring kabilang sa mga halimbawa ang:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Layunin:

- I-store ang mga pagpili sa ad privacy
- Ilapat ang UMP / AdMob privacy at ad configuration settings

#### (4) Subtitle output na ginawa ng user

Kapag nag-save o nag-export ang user ng subtitle files, maaaring magsulat ang app ng mga bagong subtitle file sa lokasyong pinili ng user, gaya ng:

- Downloads
- Ibang folder na pinili sa pamamagitan ng system picker
- User-managed storage location

Maaaring manatili ang mga user-saved files na ito sa device kahit pagkatapos ma-delete ang app, maliban kung mano-manong burahin ng user ang mga ito.

#### (5) Mga temporary file at cache

Ang app at third-party libraries ay maaaring lumikha ng temporary o cache files para sa normal na operasyon, gaya ng:

- file picker cache data
- temporary subtitle conversion data
- playback-related cache data

Ang mga ito ay para lamang sa lokal na operasyon at hindi ina-upload sa sariling servers ng developer.

#### (6) UMP consent state cache

Sa mga rehiyon kung saan naaangkop ang Google UMP, maaaring i-cache ng SDK ang consent state nang lokal sa device.

Karaniwan itong maaaring i-reset sa pamamagitan ng:

- pag-clear ng app data, o
- pagbabago ng consent choices sa loob ng app kung saan may available na privacy options entry

### 2-3) Android Overlay at Pagproseso na Kaugnay ng Permissions

Sa Android, maaaring gumamit ang lumulutang na subtitle overlay ng:

- `SYSTEM_ALERT_WINDOW` / permission para sa display-over-other-apps
- `POST_NOTIFICATIONS` permission
- foreground service notification na kinakailangan para sa overlay service

Layunin:

- ipakita ang subtitle overlay sa ibabaw ng ibang apps
- panatilihing tumatakbo ang overlay service
- pahintulutan ang Android na ipakita ang mga kinakailangang overlay / service notifications
- basahin ang impormasyon ng media notification kapag kailangan para sa subtitle progression support

Ginagamit lamang ang mga permission na ito para sa mga feature ng app na pinipiling gamitin ng user.

### 2-4) Ads, Consent, at Kaugnay na Data (Third-party SDKs)

Gumagamit ang app ng Google ad / consent SDKs, kabilang ang:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

Maaaring magpakita ang app ng:

- banner ads
- interstitial ads
- rewarded o rewarded-interstitial ads

Maaaring magproseso ang mga SDK na ito ng data gaya ng:

- advertising identifiers (halimbawa, AAID / IDFA kung naaangkop)
- IP-based at network-related information
- metadata ng device at app
- ad interaction signals
- consent choices

Maaaring kabilang sa mga layunin ang:

- ad delivery
- ad measurement at reporting
- frequency capping
- fraud prevention
- legal compliance

Layunin ng developer na i-configure ang mga SDK na ito sa paraang naaayon sa consent choices ng user at sa naaangkop na batas.

---

## 3. Paano Namin Pinoproseso at Pinapanatili ang Data

- **Lokal na settings at recent position data**
  - pinananatili sa device hanggang ma-clear ang app data o maalis ang app

- **Temporary files / cache**
  - pinananatili lamang hangga't kinakailangan para sa operasyon, pagkatapos ay inaalis ng app kung praktikal o nililinis kalaunan ng OS

- **Mga subtitle file na sinave ng user**
  - nananatili sa save location na pinili ng user hanggang burahin ito ng user

- **Ad / consent data na pinangangasiwaan ng third parties**
  - pinananatili ayon sa mga patakaran ng Google at sa naaangkop na batas

---

## 4. Third-party Processing at Cross-Border Transfers

Para sa ads at consent management, maaaring iproseso ng Google at mga kaugnay nitong partner ang ilang impormasyon.

| Item | Mga Detalye |
|---|---|
| Tatanggap | Google LLC at mga kaugnay na affiliates / processors |
| Layunin | Ad delivery, measurement, fraud prevention, consent management, at legal compliance |
| Posibleng data | Advertising identifiers, device/app info, IP-based info, ad interaction data, consent state |
| Destinasyon | United States at iba pang rehiyon kung saan gumagana ang infrastructure ng Google |
| Retention | Ayon sa mga patakaran ng Google at sa naaangkop na batas |

Layunin ng developer na panatilihing naaayon ang mga privacy disclosure sa app store sa aktuwal na asal ng SDK.

---

## 5. Iyong Mga Karapatan at Pagpipilian

Depende sa iyong hurisdiksyon, maaari kang magkaroon ng mga karapatan tulad ng:

- access
- correction
- deletion
- restriction
- portability
- objection
- withdrawal of consent kung ang consent ang legal na batayan

Kabilang sa mga praktikal na kontrol ang:

- pagbabago ng ad / privacy choices sa app kung saan available
- pag-clear ng app data upang alisin ang mga lokal na setting at naka-cache na preferences
- pag-uninstall ng app
- mano-manong pagbura ng mga na-export na subtitle files mula sa user storage
- paggamit ng OS-level controls gaya ng notification settings, ad ID reset, o ad personalization settings

Para sa data na pinoproseso ng Google, dapat ding sumangguni ang mga user sa sariling privacy at account tools ng Google kung naaangkop.

---

## 6. Privacy ng Mga Bata

Ang app na ito ay hindi pangunahing inilaan para sa mga bata.

Ang pangunahing layunin nito ay subtitle playback, editing, overlay display, at mga kaugnay na utility features. Kung naaangkop, maaaring maglapat ang ad SDK configuration ng age-related o child-directed flags na naaayon sa mga kinakailangan ng platform at sa settings ng developer.

---

## 7. Mga Hakbang sa Seguridad

Sa loob ng limitasyon ng architecture ng app, sinisikap ng developer na:

- bawasan ang pangongolekta sa pamamagitan ng pagpapanatili ng karamihan ng subtitle at media processing sa device
- gumamit ng system file pickers at user-initiated file access
- gumamit ng system permissions nang malinaw at transparent
- umasa sa encrypted network transport na ginagamit ng third-party SDKs kung naaangkop

Walang paraan ng storage o transmission ang ganap na ligtas, ngunit ang app ay idinisenyo upang maiwasan ang hindi kinakailangang pangongolekta ng developer.

---

## 8. Open-source Software

Gumagamit ang app ng open-source software, kabilang ang mga library na may kaugnayan sa:

- subtitle parsing at serialization
- file picking
- local preferences
- overlay windows
- video playback
- WebView

Available sa loob ng app ang mga open-source notices. Para sa ilang bahagi, maaaring gumamit ang app ng locally modified copy ng isang open-source package habang pinananatili ang orihinal na license notice.

---

## 9. Contact

Kung mayroon kang mga tanong o privacy-related na kahilingan:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Pakisama ang pangalan ng app na **Subtitle Player & Editor** sa iyong mensahe.

---

## 10. Mga Pagbabago sa Patakarang Ito

Maaaring i-update ang Patakarang ito kung:

- nagbago ang mga feature ng app
- nagbago ang permissions o paggamit ng SDK
- nagbago ang mga legal o platform requirements

Ang mahahalagang pagbabago ay makikita sa updated na policy page at, kung naaangkop, sa app.

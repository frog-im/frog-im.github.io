---
title: Patakaran sa Privacy | Subtitle Tool
description: Patakaran sa Privacy ng Subtitle Tool (Filipino)
lang: fil
last_updated: 2025-12-12
---

# Patakaran sa Privacy (Subtitle Tool / Subtitle Player & Editor)

- **Pangalan ng app:** Subtitle Tool (maaaring lumabas bilang “Subtitle Player & Editor” sa store)  
- **Developer:** frog-im  
- **Contact email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Petsa ng bisa:** 2025-12-12  

> Ang patakarang ito ay inihanda nang may pagsasaalang-alang sa mga naaangkop na batas sa privacy, kabilang ang Korean Personal Information Protection Act (PIPA), GDPR / UK GDPR, Swiss FADP, at ilang batas sa privacy ng mga estado sa U.S. Kapag may mas mahigpit o partikular na tuntunin sa iyong hurisdiksiyon, iyon ang mangingibabaw.

---

## 1. Layunin at saklaw

Ang app na ito ay nagbibigay ng:

- **Pag-edit ng metadata ng audio file** (title, artist, at iba pa) na naka-save sa iyong device;  
- **Lyrics / subtitle overlay** na lumulutang sa ibabaw ng ibang app.

Hindi gumagawa ang app ng **user account** at hindi **nag-u-upload ng user content** sa sariling server ng developer.  
Karaniwang isinasagawa ang pagproseso **lokal sa mismong device** ng user.

Gayunpaman, para sa **ads** at **legal na pagsunod**, gumagamit kami ng mga third-party SDK gaya ng **Google Mobile Ads SDK (AdMob)** at **Google UMP**, na maaaring magproseso ng impormasyon tulad ng **advertising identifiers**.

Ang pagkolekta ng consent at mga privacy option ay sumusunod sa mga patakaran ng **Google UMP (User Messaging Platform)**.

---

## 2. Mga kategorya ng impormasyong pinoproseso

### 2-1) Mga file na pinili mismo ng user

- **Mga path at content ng audio / cover image:**  
  Ginagamit lang sa lokal na pag-read, pag-edit ng metadata, at pag-save.  
- Ang **FFmpegKit** ay tumatakbo lang sa device para sa encoding, editing, at pagkuha ng thumbnail.  
- Hindi **inu-upload** ng app ang mga file na ito sa server ng developer.

### 2-2) Mga lokal na setting at naka-imbak na value

Upang gumana nang maayos at maging mas maginhawa para sa user, ang app ay nag-iimbak ng ilang value **lokal sa device**.  
Ang mga value na ito ay **hindi ipinapadala** sa server ng developer at **nawawala kapag dinelete ang app o app data**.

#### (1) Mga preference (`shared_preferences`)

| Uri | Key / nilalaman | Layunin | Storage | Pag-delete |
|---|---|---|---|---|
| Posisyon / laki ng font ng overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Para ma-restore ang posisyon at laki ng text ng overlay | SharedPreferences sa device | Nabubura kapag dinelete ang app o app data |
| Mga setting para sa ads / privacy | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Pag-set ng non-personalized ads, US RDP flag, child-directed flag, age tag, at max ad rating | SharedPreferences sa device | Ganoon din tulad sa itaas |

#### (2) Temporary files (system temp directory)

- **Halimbawa:** `cover_*.jpg`, `tmp_*.flac`  
- **Gamit:** pagkuha ng cover art, pagsusulat ng FLAC tags, at mga temporary encoding file  
- **Lokasyon:** temporary folder ng operating system (`systemTemp`)  
- **Retention:** sinisikap ng app na burahin ang mga file matapos gamitin; maaari pa rin silang manatili pansamantala sa system cache bago tuluyang linisin ng OS.

#### (3) Custom na lokasyon para sa pag-save (SAF)

- Kapag gumamit ang user ng “Save As” o katulad na feature, ang final audio file ay isi-save sa lokasyong pinili ng user (halimbawa, Downloads folder o cloud storage).  
- Ang mga file na ito ay naka-save sa **external storage** at **hindi awtomatikong nade-delete** kapag in-uninstall ang app. User ang may kontrol sa pag-delete.

#### (4) Consent state (UMP SDK cache)

- Sa EEA / UK / Switzerland, ang UMP SDK ay **nagki-cache nang lokal** ng consent state ng user para sa ads.  
- Maaaring i-reset ang estado na ito sa pamamagitan ng pag-delete ng app data o sa loob ng **Privacy Options** screen ng app (kung available).

---

### 2-3) Datos para sa ads at consent (third-party SDK)

**Google Mobile Ads SDK (AdMob)** at **Google UMP** ay maaaring mangolekta at magproseso ng:

- Advertising IDs (AAID / IDFA);  
- IP address o IP range;  
- Impormasyon tungkol sa device at app;  
- Mga signal ng interaction sa ads (impressions, clicks, atbp.);  
- Consent state at kaugnay na preference.

**Mga layunin ng pagproseso:**

- Paghahatid at pamamahala ng ads;  
- Frequency capping;  
- Pag-iwas sa pandaraya o maling paggamit;  
- Pagsusukat ng performance at pag-uulat;  
- Pagsunod sa mga batas sa privacy at consent.

**Mga rehiyon na nangangailangan ng consent (EEA / UK / Switzerland):**

- Kinokolekta ang consent sa pamamagitan ng UMP dialogs.  
- Mayroong **Privacy Options** screen sa app kung saan puwedeng baguhin ng user ang kanyang mga setting.

**Ibang rehiyon (halimbawa, South Korea):**

- Maaaring **hindi ipakita** ang karagdagang screen na ito kung hindi ito hinihingi ng batas.

---

## 3. Paraan ng pagproseso at retention period

- **Lokal na setting:**  
  Nananatili sa device hanggang i-delete ng user ang app data o i-uninstall ang app.  
- **Temporary files:**  
  Ginagawa sa panahon ng encoding / extraction; sinusubukan naming burahin ang mga ito matapos gamitin, pero maaari pa ring manatili nang ilang sandali sa system cache.  
- **Ad / consent data (third party):**  
  Iniimbak at pinoproseso ng mga third party (halimbawa, Google) alinsunod sa sarili nilang patakaran sa privacy.

---

## 4. Paglipat sa third party at cross-border data flow

Para sa ads at consent management, maaaring maipadala at maproseso ang ilang impormasyon sa loob ng infrastructure ng Google, kabilang ang mga server na nasa labas ng iyong bansa.

| Item | Detalye |
|---|---|
| **Tumatanggap (recipient)** | Google LLC at mga kaugnay nitong kumpanya / subprocessors |
| **Lokasyon** | Estados Unidos at iba pang rehiyon kung saan may data center ang Google |
| **Layunin** | Ad delivery, performance measurement, fraud prevention, legal compliance, consent record management |
| **Uri ng datos** | Advertising IDs, IP data, impormasyon tungkol sa device at app, ad interaction signals, consent state, atbp. |
| **Retention** | Ayon sa internal policies ng Google |
| **Epekto ng pagtanggi** | Maaaring malimitahan ang personalized ads; patuloy pa ring maipapakita ang non-personalized ads |

Sinusunod namin ang mga kinakailangan ng seksyong **“Data safety” ng Google Play**, at pinananatiling tugma ang aming disclosure sa aktwal na pagproseso sa app.

---

## 5. Iyong mga karapatan at paano gamitin ang mga ito

- **Pag-opt-out sa personalized ads / pagbabago ng consent**  
  - Sa EEA / UK / Switzerland: gamitin ang **Settings → Privacy Options** sa loob ng app.  
  - Sa ibang rehiyon: gamitin ang OS settings para i-reset ang advertising ID, limitahan ang tracking, o i-off ang personalized ads.  

- **Pag-reset ng lokal na impormasyon**  
  - Ang pag-delete ng app data o pag-uninstall ng app ay naglilinis ng mga lokal na setting (posisyon ng overlay, laki ng font, atbp.).

Ayon sa **GDPR / UK GDPR / Swiss FADP / ilang US state privacy laws**, maaaring mayroon kang karapatan na mag-access, mag-korek, mag-delete, mag-limit ng processing, humiling ng data portability, at mag-withdraw ng consent.  
Para sa ad-related data na pinoproseso ng Google, gamitin ang **opisyal na mekanismo ng Google**.

---

## 6. Privacy ng mga bata

Ang app na ito ay **hindi pangunahing idinisenyo para sa mga bata**.  
Kung ang user ay mas bata kaysa sa legal minimum age sa kanyang bansa, dapat niyang ihinto ang paggamit ng app, at kasama ang magulang/guardian, gamitin ang OS-level ad-limiting feature.  
Kung kinakailangan, maaari naming gamitin ang mga setting tulad ng **TFUA (child-directed tag)** o katulad na child-protection options.

---

## 7. Mga hakbang sa seguridad

Hangga’t praktikal, sinusubukan naming:

- Ipatupad ang **data minimization** sa koleksiyon at storage;  
- Limitahan ang paggamit ng temporary files at burahin ang mga ito pagkatapos gamitin;  
- Panatilihin ang processing sa loob lamang ng mga permission na ibinigay ng OS;  
- Gumamit ng **encryption (hal. TLS)** kapag nagpapadala ng data sa third parties (ayon sa implementation ng SDK).

---

## 8. Data safety sa Google Play

Tumpak naming pinupunan at ina-update ang seksyong **“Data safety”** sa Play Console sa tuwing may pagbabago sa paraan ng pagproseso ng data sa app.

---

## 9. Mga paunawa tungkol sa open-source

Gumagamit ang app ng open-source software, kabilang ang **FFmpeg**.  
May file sa loob ng app (halimbawa, `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) na nagpapaliwanag kung paano makuha ang source code.  
Kung humiling ang user, ibibigay namin ang source code ayon sa nakasaad sa file na iyon.

---

## 10. Contact

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Pagbabago sa patakarang ito

Maaari naming baguhin ang Patakarang ito kapag kinakailangan dahil sa batas o pagbabago sa serbisyo.  
Ipapaalam ang mga update **sa loob ng app** at sa page na ito.  
Para sa mga mahalagang pagbabago, magsisikap kaming magbigay ng abiso **hindi bababa sa 7 araw bago** maging epektibo ang mga ito.

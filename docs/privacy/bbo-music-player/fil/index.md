---
title: Patakaran sa Pagkapribado | LyriFloat
description: Patakaran sa Pagkapribado ng LyriFloat (Filipino)
lang: fil
last_updated: 2025-10-30
---

# Patakaran sa Pagkapribado (LyriFloat)

- **Pangalan ng app:** LyriFloat  
- **Developer:** frog-im  
- **Kontak:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Petsa ng bisa:** 2025-10-30

> Ang patakarang ito ay ginawa batay sa mga naaangkop na batas kabilang ang Korean Personal Information Protection Act (PIPA), GDPR/UK GDPR, Swiss FADP, at kaugnay na mga batas sa privacy ng mga estado sa U.S. Kapag may mga kinakailangang partikular sa hurisdiksyon, iyon ang masusunod.

---

## 1. Layunin at Saklaw

Ang app na ito ay nagbibigay ng **pag-edit ng metadata ng audio file** (title, artist, atbp.) na naka-save sa device at mga feature ng **lyrics overlay**.  
Hindi gumagawa ang app ng user account at **hindi** nag-a-upload ng content ng user sa anumang server. Ang pagproseso ay karaniwang ginagawa **sa device ng user**.

Gayunpaman, para sa **advertising** at **legal compliance**, maaaring mangolekta at magproseso ang mga third-party partner (hal., Google Mobile Ads SDK (AdMob), UMP) ng impormasyon tulad ng **advertising identifiers**. Ang pangongolekta ng consent at mga pagpipilian sa privacy ay sumusunod sa **Google UMP (User Messaging Platform)**.

---

## 2. Mga Kategorya ng Impormasyong Pinoproseso Namin

### 2-1) Mga File na Sadyang Pinili ng User
- **Mga path at nilalaman ng audio/cover image:** pinoproseso **lokal** sa device para lang sa pag-edit/pag-save.  
- Lokal na ginagamit ang **FFmpegKit** para sa encoding, metadata editing, at thumbnail extraction.  
- **Hindi** ina-upload ng app sa aming server ang mga file na pinili ng user.

### 2-2) Lokal na Settings at Naka-store na Values

Para sa pangunahing functionality at kaginhawaan, ang app ay nag-iimbak ng mga sumusunod **lokal sa device**.  
Hindi ito ipinapadala sa aming server at **nabubura kapag binura ang app o ang data nito**.

#### (1) Preferences (`shared_preferences`)
| Uri | Key/Nilalaman | Layunin | Storage | Pagbura |
|---|---|---|---|---|
| Posisyon/font ng overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Ibalik ang posisyon ng overlay at laki ng font | Device SharedPreferences | Nabubura kapag binura ang app data o ang app |
| Ads/Privacy settings | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Non-personalized ads, U.S. RDP, COPPA tag, age tag, ad content rating limit | Device SharedPreferences | Katulad ng nasa kaliwa |

#### (2) Temporary Files (system temp directory)
- **Halimbawa:** `cover_*.jpg`, `tmp_*.flac`  
- **Gamit:** cover art extraction, FLAC tagging, temporary encoding  
- **Lokasyon:** OS temporary folder (`systemTemp`)  
- **Retention:** tinatanggal ng app pagkatapos kung posible; saklaw din ng OS cleanup

#### (3) User-selected Save (SAF)
- Kapag pinili ng user ang “Save As,” maaaring maisulat ang final audio files sa lokasyong pinili ng user (hal., Downloads, cloud).  
- Nasa **external storage** ang mga file at **mananatili kahit i-uninstall ang app**. Mano-manong mabubura ng user.

#### (4) Consent State (UMP SDK Cache)
- Sa EEA/UK/CH, ang UMP SDK ay **nagka-cache ng consent state lokal**.  
- Maaaring i-reset sa pamamagitan ng pag-delete ng app data o sa in-app na **Privacy Options** screen kung available.

---

### 2-3) Ads at Consent-related Data (Third-party SDKs)
- Maaaring mangolekta/magproseso ang **Google Mobile Ads SDK (AdMob) at UMP** ng: **advertising identifiers (AAID/IDFA)**, **IP ranges**, **device/app info**, **ad interaction signals**, **consent state**, atbp.  
- **Layunin:** ad delivery, frequency capping, fraud prevention, performance measurement, legal compliance  
- **Mga rehiyong nangangailangan ng consent (EEA/UK/CH):** kinokolekta ang consent sa UMP prompts at may **Privacy Options** screen kapag kinakailangan.  
  Sa mga rehiyong walang ganitong requirement (hal., KR), **maaaring hindi ito ipakita**.

---

## 3. Pagproseso at Retention

- **Lokal na settings:** naka-store sa device hanggang burahin ng user ang app data o i-uninstall ang app  
- **Temporary files:** ginagawa habang encoding/extraction, binubura pagkatapos o maaaring pansamantalang manatili sa OS caches  
- **Ads/consent data (third-party):** nire-retain at dini-dispose ayon sa **mga patakaran ng Google**

---

## 4. Third-party Transfers at Cross-Border Data Flows

Para sa advertising at consent management, maaaring maipadala at maproseso ang impormasyon sa Google infrastructure.

| Item | Detalye |
|---|---|
| **Tatanggap** | Google LLC at mga affiliate/sub-processor nito |
| **Destinasyon** | United States (at iba pang rehiyon kung nasaan ang Google infrastructure) |
| **Layunin** | Ad delivery, performance/measurement, legal compliance, consent management |
| **Data** | Advertising identifiers, IP ranges, device/app info, ad interactions, consent state, atbp. |
| **Retention** | Ayon sa patakaran ng Google |
| **Epekto ng Pagtanggi** | Maaaring limitado ang personalized ads; maaaring magpakita ng non-personalized ads |

Sumusunod kami sa mga requirement ng **Google Play Data safety** at tinutugma ang disclosures sa aktuwal na pagproseso.

---

## 5. Mga Karapatan Mo at Paano Ito Gamitin

- **Mag-opt out sa personalized ads / baguhin ang consent**  
  - Sa supported regions (EEA/UK/CH): baguhin sa **Settings → Privacy Options**.  
  - Ibang rehiyon: gamitin ang OS settings para **i-reset ang ad IDs / limitahan ang ad tracking**.
- **I-reset ang lokal na impormasyon:** pag-delete ng app data o pag-uninstall ay magre-reset ng overlay coordinates, font size, at iba pang lokal na settings.
- Ang mga karapatan sa ilalim ng **GDPR/UK GDPR/Swiss FADP/U.S. state privacy laws** (access, rectification, erasure, portability, restriction, withdrawal of consent, atbp.) ay maaaring gamitin ayon sa batas.  
  Para sa ad-related data na pinoproseso ng Google, gamitin ang **mga proseso ng Google**.

---

## 6. Privacy ng mga Bata

Ang app na ito ay **hindi para sa mga bata**. Kung gagamit ang batang mas mababa sa legal na minimum age, dapat huminto at gumamit ng OS-level ad-limiting features kasama ang guardian. Kapag naaangkop, maaari naming i-apply ang **TFUA (child-directed tag)** o katulad na child-protection options.

---

## 7. Mga Hakbang sa Seguridad

- **Data minimization** sa koleksyon at storage  
- **Limitadong paggamit** ng temporary files at pagtatangkang burahin pagkatapos ng proseso  
- Pagproseso nang mahigpit **sa saklaw ng OS permissions**  
- **TLS o katumbas** na encryption in transit para sa third-party transfers (ayon sa SDK standards)

---

## 8. Data Safety (Google Play)

Tumpak naming inihahanda at pinananatili ang seksyong **Data safety** sa Play Console, at ina-update agad kapag may pagbabago.

---

## 9. Open-source Notices

Gumagamit ang app ng open-source software tulad ng **FFmpeg**. May info file (hal., `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) sa loob ng app na nagpapaliwanag kung paano kunin ang source code. Kapag hiniling, ibibigay namin ang source ayon sa nakasaad sa file na iyon.

---

## 10. Kontak

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Mga Pagbabago sa Patakarang Ito

Maaari naming baguhin ang patakarang ito dahil sa legal o service changes. Ipo-post namin ang updates **in-app** at sa **policy page** na ito.  
Para sa material changes, magbibigay kami ng abiso nang hindi bababa sa **7 araw** bago ang effective date.

---

## Appendix: Gabay sa User

- **In-app link:** buksan ang page na ito mula sa **Settings → Privacy**.  
- **Regional behavior:** sa EEA/UK/CH, ipinapakita ang Privacy Options. **Sa KR at ilang ibang rehiyon, maaaring hindi lumabas ang button o dagdag na options** kung hindi legal na kinakailangan.

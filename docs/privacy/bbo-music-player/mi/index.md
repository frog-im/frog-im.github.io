---
title: Kaupapahere Tūmataiti | LyriFloat
description: Kaupapahere Tūmataiti o LyriFloat (Māori)
lang: mi
last_updated: 2025-10-30
---

# Kaupapahere Tūmataiti (LyriFloat)

- **Ingoa taupānga:** LyriFloat  
- **Kaihanga:** frog-im  
- **Whakapā:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Rā whai mana:** 2025-10-30

> I tuhia tēnei kaupapahere mā te aro ki ngā ture e hāngai ana, tae atu ki te Korean Personal Information Protection Act (PIPA), GDPR/UK GDPR, te Swiss FADP, me ngā ture tūmataiti ā-kāwanatanga o te U.S. Mēnā he whakaritenga motuhake ā-rohe, ko aua whakaritenga te mea matua.

---

## 1. Te Kaupapa me te Whānuitanga

Ka whakarato tēnei taupānga i te **whakatika metadata kōnae oro** (taitara, kaitoi, aha atu) kei runga i te pūrere me ngā āhuatanga **lyrics overlay**.  
Kāore te taupānga e hanga pūkete kaiwhakamahi, ā, kāore hoki e **tukuake** i ngā ihirangi a te kaiwhakamahi ki tētahi tūmau. Ka mahia te tukatuka **i runga i te pūrere o te kaiwhakamahi** i te nuinga o te wā.

Heoi anō, mō ngā take **pānuitanga** me te **whai i te ture**, ka taea e ngā hoa tuatoru (hei tauira, Google Mobile Ads SDK (AdMob), UMP) te kohikohi me te tukatuka i ngā mōhiohio pērā i ngā **advertising identifiers**. Ka whai te kohi whakaaetanga me ngā kōwhiringa tūmataiti i ngā whakaritenga a **Google UMP (User Messaging Platform)**.

---

## 2. Ngā Kāwai Mōhiohio Ka Tukatukahia

### 2-1) Ngā Kōnae i Kōwhiria e te Kaiwhakamahi
- **Ngā ara kōnae me ngā ihirangi oro/cover image:** ka tukatukahia **ā-rohe** i runga i te pūrere mō te whakatika/tiaki anake.  
- Ka whakamahia **FFmpegKit** ā-rohe mō te encoding, metadata editing, me te tango thumbnail.  
- Kāore te taupānga e **tukuake** i ngā kōnae i kōwhiria e te kaiwhakamahi ki ā mātou tūmau.

### 2-2) Ngā Tautuhinga ā-Rohe me ngā Uara Ka Penapena

Mō te mahi matua me te ngāwari o te whakamahi, ka penapena te taupānga i ēnei uara **ki te pūrere**.  
Kāore ēnei e tukuna ki ā mātou tūmau, ā, ka **mukua** ina mukua te taupānga, ina mukua rānei ōna raraunga.

#### (1) Ngā Manakohanga (`shared_preferences`)
| Momo | Kī/Ihirangi | Kaupapa | Rokiroki | Mukunga |
|---|---|---|---|---|
| Tūnga/font overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Whakaora anō i te tūnga overlay me te rahi momotuhi | Device SharedPreferences | Ka mukua ina mukua ngā raraunga taupānga, ina mukua rānei te taupānga |
| Ads/Privacy settings | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | NPA, U.S. RDP, COPPA tag, age tag, tepe rating ihirangi pānui | Device SharedPreferences | Ōrite ki te taha mauī |

#### (2) Ngā Kōnae Rangitahi (system temp directory)
- **Tauira:** `cover_*.jpg`, `tmp_*.flac`  
- **Whakamahi:** tango cover art, FLAC tagging, encoding rangitahi  
- **Wāhi:** kōpaki rangitahi OS (`systemTemp`)  
- **Roanga:** ka ngana te taupānga ki te muku ina oti; ka taea hoki te OS te horoi

#### (3) Te Tiaki i Kōwhiria e te Kaiwhakamahi (SAF)
- Ina kōwhiri te kaiwhakamahi i “Save As,” ka taea te tuhi i ngā kōnae oro whakamutunga ki ngā wāhi i tohua (hei tauira, Downloads, cloud).  
- Kei **te rokiroki o waho** ēnei kōnae, ā, ka **noho tonu** ahakoa ka mukua te taupānga. Ka taea e te kaiwhakamahi te muku ā-ringa.

#### (4) Te Āhua Whakaaetanga (UMP SDK Cache)
- I ngā rohe EEA/UK/CH, ka **penapena ā-rohe** te UMP SDK i te āhua whakaaetanga pānui.  
- Ka taea te tautuhi anō mā te muku raraunga taupānga, mā te mata **Privacy Options** i roto i te taupānga (ina wātea).

---

### 2-3) Ngā Raraunga Pānuitanga me te Whakaaetanga (Third-party SDKs)
- Ka taea e **Google Mobile Ads SDK (AdMob) me UMP** te kohi/tukatuka i: **AAID/IDFA**, **IP ranges**, **mōhiohio pūrere/taupānga**, **tohu pāhekoheko pānui**, **āhua whakaaetanga**, aha atu.  
- **Kaupapa:** tuku pānui, frequency capping, ārai tinihanga, ine mahi, whai i te ture  
- **Ngā rohe me tono whakaaetanga (EEA/UK/CH):** ka kohia te whakaaetanga mā ngā UMP prompts, ā, ka whakaratoa he mata **Privacy Options** ina hiahiatia.  
  I ngā rohe kāore e tono pēnei (hei tauira, KR), **tērā pea kāore e whakaaturia** te kōwhiringa.

---

## 3. Tukatuka me te Roanga Penapena

- **Tautuhinga ā-rohe:** ka noho ki te pūrere kia muku rā anō te kaiwhakamahi i ngā raraunga, kia tango rānei i te taupānga  
- **Kōnae rangitahi:** ka hangaia i te wā encoding/extraction, ka mukua i muri, tērā rānei ka noho rangitahi ki ngā cache OS  
- **Raraunga pānui/whakaaetanga (tuatoru):** ka penapenahia ka whakakorea hoki kia rite ki **ngā kaupapa here a Google**

---

## 4. Ngā Whakawhitinga Tuatoru me ngā Rerenga Raraunga ā-Ao

Mō te pānuitanga me te whakahaere whakaaetanga, ka taea te tuku me te tukatuka i ngā mōhiohio ki runga i te hanganga a Google.

| Mea | Taipitopito |
|---|---|
| **Kaiwhiwhi** | Google LLC me ōna hononga/sub-processors |
| **Wāhi** | United States (me ētahi atu rohe e noho ana te hanganga a Google) |
| **Kaupapa** | Tuku pānui, ine mahi, whai i te ture, whakahaere whakaaetanga |
| **Raraunga** | Advertising identifiers, IP ranges, info pūrere/taupānga, pāhekoheko pānui, āhua whakaaetanga, aha atu |
| **Roanga** | E ai ki ngā kaupapa here a Google |
| **Pānga o te whakakore** | Ka iti pea ngā pānui whaiaro; ka whakaaturia pea ngā pānui kāore i te whaiaro |

Ka ū mātou ki ngā whakaritenga **Google Play Data safety** me te whakahāngai i ngā kōrero whakaatu ki te tukatuka tūturu.

---

## 5. Ō Tika me te Āhua Whakatinana

- **Whakakore pānui whaiaro / huri whakaaetanga**  
  - I ngā rohe tautoko (EEA/UK/CH): mā **Settings → Privacy Options**.  
  - I ētahi atu rohe: mā ngā tautuhinga OS hei **tautuhi anō i te ad ID / whakaiti ad tracking**.
- **Tautuhi anō raraunga ā-rohe:** mā te muku raraunga taupānga, mā te tango taupānga rānei ka tautuhi anō i ngā tūnga overlay, rahi momotuhi, me ētahi atu tautuhinga.
- Ka taea ngā tika i raro i **GDPR/UK GDPR/Swiss FADP/U.S. state privacy laws** (access, rectification, erasure, portability, restriction, withdrawal of consent, aha atu) kia rite ki aua ture.  
  Mō ngā raraunga pānui ka tukatukahia e Google, whakamahia ngā **tukanga a Google**.

---

## 6. Tūmataiti o ngā Tamariki

Kāore tēnei taupānga i hanga mō ngā tamariki. Mēnā ka whakamahi tētahi tamaiti i raro i te pakeke iti ā-ture, me whakamutu, ā, me whakamahi ngā āheinga OS hei whakaiti pānui me tētahi kaitiaki. Ina hāngai, ka taea te whakamahi i te **TFUA (child-directed tag)**, me ētahi atu kōwhiringa tiaki tamariki.

---

## 7. Ngā Tikanga Haumarutanga

- **Whakaiti raraunga** i te kohi me te rokiroki  
- **Iti noa** te whakamahi kōnae rangitahi me te ngana ki te muku ina oti  
- Tukatuka **i roto i ngā whakaaetanga OS** anake  
- **TLS, he ōrite rānei** mō te whakamunatanga i te tuku (e ai ki ngā paerewa SDK)

---

## 8. Data Safety (Google Play)

Ka whakarite, ka pupuri mātou i te wāhanga **Data safety** i roto i te Play Console kia tika, ā, ka whakahōu wawe ina rerekē.

---

## 9. Ngā Pānui Open-source

Ka whakamahi te taupānga i ngā pūmanawa open-source pērā i **FFmpeg**. He kōnae pārongo (hei tauira, `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) kei roto i te taupānga e whakamārama ana me pēhea te tiki i te source code. Ina tonoa, ka tukuna e mātou te source kia rite ki taua kōnae.

---

## 10. Whakapā

- Īmēra: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Ngā Panonitanga ki tēnei Kaupapahere

Ka taea te whakahou i tēnei kaupapahere nā ngā panonitanga ture, ratonga rānei. Ka whakaputaina ngā whakahōu **i roto i te taupānga** me tēnei **whārangi kaupapa here**.  
Mō ngā panonitanga nui, ka tukuna he pānui **mō te 7 rā** i mua i te rā whai mana.

---

## Āpitihanga: Aratohu Kaiwhakamahi

- **Hononga i roto i te taupānga:** whakatuwheratia tēnei whārangi i **Settings → Privacy**.  
- **Āhua ā-rohe:** i EEA/UK/CH, ka whakaaturia ngā Privacy Options. **I KR me ētahi atu rohe, tērā pea kāore e puta he kōwhiringa anō** ina kāore e hiahiatia ā-ture.

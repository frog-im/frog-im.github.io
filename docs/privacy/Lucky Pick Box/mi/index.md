---
title: Kaupapahere Tūmataitinga | Lucky Pick Box
description: Lucky Pick Box Kaupapahere Tūmataitinga
lang: mi
last_updated: 2026-06-15
---

# Kaupapahere Tūmataiti (Lucky Pick Box / 뽑기박스)

- **Ingoa Taupānga:** Lucky Pick Box / 뽑기박스
- **Kaiwhakawhanake:** frog-im
- **Āpiha Tiaki Pārongo Whaiaro / Tangata Whakapā:** frog-im
- **Whakapā:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Rā Whai Mana:** 2026-06-12
- **Whakahōu Whakamutunga:** 2026-06-15

> Kua whakaritea tēnei Kaupapahere i runga i ngā pārongo e tukatukahia ana e te taupānga me ōna āhuatanga e hāngai ana.  
> Mēnā ka whai mana ētahi ture, ētahi whakaritenga here rānei i tētahi whenua, i tētahi rohe rānei, ka taea e aua ture, e aua whakaritenga rānei te noho matua.

---

## 1. Te Kaupapa me te Whānuitanga

He taputapu ngahau a Lucky Pick Box mō te kōwhiri matapōkere, te unu, te kōwhiri raupapa, te wehe kapa, te mataono, te moni, te arawhata, te wīra me ngā kēmu whakatau ā-rā, ā-rōpū hoki. Kāore te taupānga e whakarato petipeti moni tūturu, peti, tauwhitinga pūtea, taonga moni, utu taurite ki te moni rānei.

### A. Ngā āhuatanga matua

- Tāuru tere: he kupu ka patohia e te kaiwhakamahi, he kupu rānei ka pānuihia mai i tētahi whakaahua kua tīpakohia.
- Kēmu kōwhiri matapōkere: ladder, wheel, plinko, simple draw, dice, coin, random number, team splitter, order picker, card, bomb me yes/no.
- Hītori hua: ka taea te tiaki i te momo kēmu, taitara, kaitākaro/tūemi, whakarāpopototanga hua me te wā hanga.
- Ngā wāhi tautuhinga: ka taea e ētahi kēmu te tiaki kaitākaro, rārangi, awhe, rahinga, kapa, taumaha me ngā tautuhinga pērā ki te 3 wāhi ā-rohe.

Kāore te taupānga e tono rēhita, takiuru rānei. Kāore mātou e whakahaere tūmau e whiwhi ana i tō ingoa, tau waea, īmēra, hoapā, tāurunga kēmu, whakaahua kua tīpakohia, hua kēmu rānei mai i te taupānga.

Hei tuku āheinga, ka rokiroki pea te taupānga i ngā tāurunga kēmu, tapanga kaitākaro, hua tata, tautuhinga kēmu kua tiakina, tautuhinga nekehanga, kōwhiringa tūmataitinga pānui me te tūnga e pā ana ki te whakaaetanga ki te rokiroki ā-rohe o tō pūrere. Ka herea e te taupānga te hītori hua tata, ā, kāore e tukuna ki tētahi tūmau e whakahaerehia ana e te kaiwhakawhanake.

---

## 2. Ngā Kāwai o te Pārongo Whaiaro e Tukatukahia Ana

### 2-1) Te Pārongo ka Whakaurua Tikatia e te Kaiwhakamahi

Kāore te taupānga e tono rēhita, takiuru rānei. Kāore mātou e whakahaere tūmau e whiwhi ana i tō ingoa, tau waea, īmēra, hoapā, tāurunga kēmu, whakaahua kua tīpakohia, hua kēmu rānei mai i te taupānga.

### 2-2) Ngā Kōnae ka Tīpakohia i runga i te Pūrere

Ki te kōwhiri koe ki te pānui kupu mai i tētahi whakaahua, ka tono te taupānga kia tīpakohia he whakaahua mai i tō whare whakaahua. Ka whakamahia te whakaahua kua tīpakohia mō te mōhio kupu i runga i te pūrere mā te image picker o te pūnaha me ngā wāhanga Google ML Kit. Kāore te kaiwhakawhanake e tukuatu i te whakaahua ki tana tūmau, ā, kāore e pupuri ki tētahi pūkete mamao.

### 2-3) Ngā Raraunga e Penapenahia Ā-Rohe ana i roto i te Taupānga

Hei tuku āheinga, ka rokiroki pea te taupānga i ngā tāurunga kēmu, tapanga kaitākaro, hua tata, tautuhinga kēmu kua tiakina, tautuhinga nekehanga, kōwhiringa tūmataitinga pānui me te tūnga e pā ana ki te whakaaetanga ki te rokiroki ā-rohe o tō pūrere. Ka herea e te taupānga te hītori hua tata, ā, kāore e tukuna ki tētahi tūmau e whakahaerehia ana e te kaiwhakawhanake.

### B. Raraunga ā-rohe i runga i te pūrere

| Wāhi, kī rānei | Raraunga | Kaupapa | Muku |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, momo kēmu, taitara, kaitākaro/tūemi, whakarāpopototanga, wā; tae atu ki te 50 hua tata. | Whakaatu hua tata me te hītori. | Muku i roto i te taupānga, ūkui raraunga taupānga, tango rānei |
| `game_settings.<gameId>.slot_<n>` | Tautuhinga kēmu, wā tiaki, rārangi, awhe, rahinga, kapa, taumaha; tae atu ki te 3 wāhi. | Utaina anō ngā tautuhinga kēmu. | Whakakorea te wāhi, ūkui raraunga, tango rānei |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Tautuhinga nekehanga me te mata katoa. | Pupuri i ngā kōwhiringa whakaatu. | Huri tautuhinga, ūkui raraunga, tango rānei |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Kōwhiringa tūmataitinga pānui me te kaute auau pānui. | Whakamahi kōwhiringa ā-rohe me te whakahaere auau. | Huri tautuhinga, ūkui raraunga, tango rānei |
| Kaitīpako whakaahua me OCR | Ka tukatukahia rangitahi pea te ara whakaahua me te kupu kua mōhiotia. | Tāpiri kupu whakaahua ki te tāuru tere. | Keteroki taupānga/OS, ūkui raraunga rānei |

Kāore te kupu tāuru tere e tukuna ki tētahi tūmau kaiwhakawhanake. Ka noho hei raraunga ā-rohe anake mēnā ka whakamahia ki tētahi hua kēmu, tautuhinga tiaki rānei.

### 2-4) Te Pārongo ka Taea te Tukatuka Aunoa i te Wā e Whakahaerehia ana te Pānuitanga me te Whakaae

I runga i ngā tūāpapa e tautokona ana, arā ko Android i tēnei wā, ka whakamahi te taupānga i a Google AdMob me Google User Messaging Platform (UMP). Ka tukatuka pea a Google me ngā hoa pānui i ngā tautuhi pānui, tautuhi instance taupānga, wāhitau IP, tauwāhi tata, mōhiohio pūrere me te whatunga, putanga taupānga, pūnaha whakahaere, reo, kitenga pānui, pāwhiri me ngā pāhekoheko, tātaritanga, tūnga whakaaetanga me ngā tautuhinga tūmataitinga pānui ā-rohe hei tuku pānui, here auau, aukati tinihanga, whakahaere whakaaetanga, ine, wetewete, haumaru me te ū ki te ture.

Kei https://policies.google.com/privacy me https://policies.google.com/technologies/ads ngā tikanga tūmataitinga a Google.

---

## 3. Te Kaupapa o te Tukatuka Pārongo Whaiaro

He taputapu ngahau a Lucky Pick Box mō te kōwhiri matapōkere, te unu, te kōwhiri raupapa, te wehe kapa, te mataono, te moni, te arawhata, te wīra me ngā kēmu whakatau ā-rā, ā-rōpū hoki. Kāore te taupānga e whakarato petipeti moni tūturu, peti, tauwhitinga pūtea, taonga moni, utu taurite ki te moni rānei.

### A. Ngā āhuatanga matua

- Tāuru tere: he kupu ka patohia e te kaiwhakamahi, he kupu rānei ka pānuihia mai i tētahi whakaahua kua tīpakohia.
- Kēmu kōwhiri matapōkere: ladder, wheel, plinko, simple draw, dice, coin, random number, team splitter, order picker, card, bomb me yes/no.
- Hītori hua: ka taea te tiaki i te momo kēmu, taitara, kaitākaro/tūemi, whakarāpopototanga hua me te wā hanga.
- Ngā wāhi tautuhinga: ka taea e ētahi kēmu te tiaki kaitākaro, rārangi, awhe, rahinga, kapa, taumaha me ngā tautuhinga pērā ki te 3 wāhi ā-rohe.

I runga i ngā tūāpapa e tautokona ana, arā ko Android i tēnei wā, ka whakamahi te taupānga i a Google AdMob me Google User Messaging Platform (UMP). Ka tukatuka pea a Google me ngā hoa pānui i ngā tautuhi pānui, tautuhi instance taupānga, wāhitau IP, tauwāhi tata, mōhiohio pūrere me te whatunga, putanga taupānga, pūnaha whakahaere, reo, kitenga pānui, pāwhiri me ngā pāhekoheko, tātaritanga, tūnga whakaaetanga me ngā tautuhinga tūmataitinga pānui ā-rohe hei tuku pānui, here auau, aukati tinihanga, whakahaere whakaaetanga, ine, wetewete, haumaru me te ū ki te ture.

Kei https://policies.google.com/privacy me https://policies.google.com/technologies/ads ngā tikanga tūmataitinga a Google.

---

## 4. Te Wā Pupuri me te Rokiroki o te Pārongo Whaiaro

Ka noho pea te hītori ā-rohe me ngā tautuhinga ki tō pūrere kia mukua rā anō e koe te hītori, kia whakawāteatia ngā raraunga taupānga, kia tango rānei i te taupānga. Ka taea e koe te huri i ngā kōwhiringa tūmataitinga pānui e wātea ana i ngā tautuhinga taupānga, te whakatuwhera i ngā kōwhiringa tūmataitinga a Google ina hiahiatia, me te whakahaere, tautuhi anō rānei i ngā tautuhi pānui i ngā tautuhinga tūmataitinga o te pūrere. Ko te pupuri o ngā mōhiohio ka tukatukahia e Google e whakahaerehia ana e ngā kaupapa here me ngā herenga ā-ture a Google.

### B. Raraunga ā-rohe i runga i te pūrere

| Wāhi, kī rānei | Raraunga | Kaupapa | Muku |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, momo kēmu, taitara, kaitākaro/tūemi, whakarāpopototanga, wā; tae atu ki te 50 hua tata. | Whakaatu hua tata me te hītori. | Muku i roto i te taupānga, ūkui raraunga taupānga, tango rānei |
| `game_settings.<gameId>.slot_<n>` | Tautuhinga kēmu, wā tiaki, rārangi, awhe, rahinga, kapa, taumaha; tae atu ki te 3 wāhi. | Utaina anō ngā tautuhinga kēmu. | Whakakorea te wāhi, ūkui raraunga, tango rānei |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Tautuhinga nekehanga me te mata katoa. | Pupuri i ngā kōwhiringa whakaatu. | Huri tautuhinga, ūkui raraunga, tango rānei |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Kōwhiringa tūmataitinga pānui me te kaute auau pānui. | Whakamahi kōwhiringa ā-rohe me te whakahaere auau. | Huri tautuhinga, ūkui raraunga, tango rānei |
| Kaitīpako whakaahua me OCR | Ka tukatukahia rangitahi pea te ara whakaahua me te kupu kua mōhiotia. | Tāpiri kupu whakaahua ki te tāuru tere. | Keteroki taupānga/OS, ūkui raraunga rānei |

Kāore te kupu tāuru tere e tukuna ki tētahi tūmau kaiwhakawhanake. Ka noho hei raraunga ā-rohe anake mēnā ka whakamahia ki tētahi hua kēmu, tautuhinga tiaki rānei.

---

## 5. Ngā Tukanga me ngā Tikanga mō te Whakakore i te Pārongo Whaiaro

Ka noho pea te hītori ā-rohe me ngā tautuhinga ki tō pūrere kia mukua rā anō e koe te hītori, kia whakawāteatia ngā raraunga taupānga, kia tango rānei i te taupānga. Ka taea e koe te huri i ngā kōwhiringa tūmataitinga pānui e wātea ana i ngā tautuhinga taupānga, te whakatuwhera i ngā kōwhiringa tūmataitinga a Google ina hiahiatia, me te whakahaere, tautuhi anō rānei i ngā tautuhi pānui i ngā tautuhinga tūmataitinga o te pūrere. Ko te pupuri o ngā mōhiohio ka tukatukahia e Google e whakahaerehia ana e ngā kaupapa here me ngā herenga ā-ture a Google.

### C. Whakaaetanga, SDK, tārua me te haumaru

Ka taea e te taupānga te whakamahi `INTERNET`, `ACCESS_NETWORK_STATE` me `com.google.android.gms.permission.AD_ID` mō ngā pānui me ngā pānui ā-ture. Ka whakamahia te uru whakaahua, kaitīpako whakaahua rānei anake ina kōwhiri te kaiwhakamahi ki te pānui kupu mai i te whakaahua.

Ka tukatuka pea a Google Mobile Ads SDK i te wāhitau IP, ngā pāhekoheko pānui, tātaritanga me ngā tautuhi pūrere/pūkete mō te pānuitanga, wetewete me te aukati tinihanga. Ka tukatuka pea a UMP i te tūnga whakaaetanga me ngā kōwhiringa tūmataitinga.

Ka taea te muku raraunga ā-rohe mā ngā āhuatanga muku o te taupānga, mā te ūkui raraunga taupānga i te OS, mā te tango rānei. Ka noho pea ngā tārua pūnaha, whakaahua mata, kōnae tiritiri rānei i raro i ngā kaupapa here a te kaiwhakarato. Kaua e whakauru raraunga tairongo ki ngā āpure kupu wātea.

---

## 6. Te Tuku ki ngā Rōpū Tuatoru, te Tuku Mahi ki Waho, me te Whakawhiti Raraunga ki Tāwāhi

Kāore mātou e hoko i ō tāurunga kēmu, tapanga kaitākaro, hua kēmu, whakaahua kua tīpakohia rānei. Ina tonoa ngā āheinga pānui, whakaaetanga rānei, ka tukatuka pea a Google LLC, ngā hinonga pātahi o Google me ā rātou kaiwhakarato ratonga i ngā mōhiohio pānui me te whakaaetanga i ngā whenua kei waho i tō whenua, rohe rānei. Tirohia te "Pānui Whakawhiti Raraunga ā-Ao" i roto i te taupānga mō ētahi atu taipitopito.

| Tūemi | Ngā Taipitopito |
|---|---|
| **Kaiwhiwhi / Rōpū Whirinaki** | Google LLC me ōna peka (ngā kaiwhakahaere o AdMob / UMP) |
| **Whenua Whakawhiti** | United States me ngā rohe e whakahaerehia ai te hanganga a Google |
| **Wā Whakawhiti** | Ā-tonu i te wā o ngā tono pānuitanga, te tirohanga tūnga whakaae, te tīmatanga SDK, me te whakahaere |
| **Tikanga Whakawhiti** | Te tuku mā te whakawhiti kōrero whatunga i waenga i te taupānga me ngā tūmau rōpū-tuatoru |
| **Pūtake Ture mō te Whakawhiti ki Tāwāhi** | Ka tukatukahia i roto i te whānuitanga e tika ana hei whakarato i te ratonga i raro i ngā pūtake ture e hāngai ana, ā, mēnā e tika ana, i runga hoki i te whakaae a te tangata nōna ngā raraunga |
| **Kaupapa** | Te tuku pānuitanga, te ine pānuitanga, te whakahaere whakaae, te ārai tinihanga, me te ū ki ngā kaupapa here / ture |
| **Ngā Kāwai Raraunga (Tauira)** | Ngā pūtāutu pānuitanga (AAID / IDFA), pārongo IP / whatunga, pārongo pūrere / taupānga, pārongo pāhekoheko pānuitanga, tūnga whakaae |
| **Wā Pupuri** | Ka whai i ngā kaupapa here a Google me ngā ture e hāngai ana |
| **Pānga o te Whakakāhore** | Tērā pea ka herea ngā pānuitanga kua whakaritea mō te tangata, ka whakaatuhia rānei ngā pānuitanga kāore i whakaritea mō te tangata, ka herea rānei ētahi āhuatanga e pā ana ki te pānuitanga |

---

## 7. Pārongo mō ngā Whakaaetanga e Whakamahia Ana

### C. Whakaaetanga, SDK, tārua me te haumaru

Ka taea e te taupānga te whakamahi `INTERNET`, `ACCESS_NETWORK_STATE` me `com.google.android.gms.permission.AD_ID` mō ngā pānui me ngā pānui ā-ture. Ka whakamahia te uru whakaahua, kaitīpako whakaahua rānei anake ina kōwhiri te kaiwhakamahi ki te pānui kupu mai i te whakaahua.

Ka tukatuka pea a Google Mobile Ads SDK i te wāhitau IP, ngā pāhekoheko pānui, tātaritanga me ngā tautuhi pūrere/pūkete mō te pānuitanga, wetewete me te aukati tinihanga. Ka tukatuka pea a UMP i te tūnga whakaaetanga me ngā kōwhiringa tūmataitinga.

Ka taea te muku raraunga ā-rohe mā ngā āhuatanga muku o te taupānga, mā te ūkui raraunga taupānga i te OS, mā te tango rānei. Ka noho pea ngā tārua pūnaha, whakaahua mata, kōnae tiritiri rānei i raro i ngā kaupapa here a te kaiwhakarato. Kaua e whakauru raraunga tairongo ki ngā āpure kupu wātea.

---

## 8. Te Tāutanga, te Whakahaere, me te Whakakore i ngā Tikanga Kohikohi Aunoa

I runga i ngā tūāpapa e tautokona ana, arā ko Android i tēnei wā, ka whakamahi te taupānga i a Google AdMob me Google User Messaging Platform (UMP). Ka tukatuka pea a Google me ngā hoa pānui i ngā tautuhi pānui, tautuhi instance taupānga, wāhitau IP, tauwāhi tata, mōhiohio pūrere me te whatunga, putanga taupānga, pūnaha whakahaere, reo, kitenga pānui, pāwhiri me ngā pāhekoheko, tātaritanga, tūnga whakaaetanga me ngā tautuhinga tūmataitinga pānui ā-rohe hei tuku pānui, here auau, aukati tinihanga, whakahaere whakaaetanga, ine, wetewete, haumaru me te ū ki te ture.

Kei https://policies.google.com/privacy me https://policies.google.com/technologies/ads ngā tikanga tūmataitinga a Google.

Ka noho pea te hītori ā-rohe me ngā tautuhinga ki tō pūrere kia mukua rā anō e koe te hītori, kia whakawāteatia ngā raraunga taupānga, kia tango rānei i te taupānga. Ka taea e koe te huri i ngā kōwhiringa tūmataitinga pānui e wātea ana i ngā tautuhinga taupānga, te whakatuwhera i ngā kōwhiringa tūmataitinga a Google ina hiahiatia, me te whakahaere, tautuhi anō rānei i ngā tautuhi pānui i ngā tautuhinga tūmataitinga o te pūrere. Ko te pupuri o ngā mōhiohio ka tukatukahia e Google e whakahaerehia ana e ngā kaupapa here me ngā herenga ā-ture a Google.

---

## 9. Ngā Motika a te Kaiwhakamahi me te Āhua o te Whakatinana

Ka noho pea te hītori ā-rohe me ngā tautuhinga ki tō pūrere kia mukua rā anō e koe te hītori, kia whakawāteatia ngā raraunga taupānga, kia tango rānei i te taupānga. Ka taea e koe te huri i ngā kōwhiringa tūmataitinga pānui e wātea ana i ngā tautuhinga taupānga, te whakatuwhera i ngā kōwhiringa tūmataitinga a Google ina hiahiatia, me te whakahaere, tautuhi anō rānei i ngā tautuhi pānui i ngā tautuhinga tūmataitinga o te pūrere. Ko te pupuri o ngā mōhiohio ka tukatukahia e Google e whakahaerehia ana e ngā kaupapa here me ngā herenga ā-ture a Google.

---

## 10. Ngā Tikanga Haumarutanga

### C. Whakaaetanga, SDK, tārua me te haumaru

Ka taea e te taupānga te whakamahi `INTERNET`, `ACCESS_NETWORK_STATE` me `com.google.android.gms.permission.AD_ID` mō ngā pānui me ngā pānui ā-ture. Ka whakamahia te uru whakaahua, kaitīpako whakaahua rānei anake ina kōwhiri te kaiwhakamahi ki te pānui kupu mai i te whakaahua.

Ka tukatuka pea a Google Mobile Ads SDK i te wāhitau IP, ngā pāhekoheko pānui, tātaritanga me ngā tautuhi pūrere/pūkete mō te pānuitanga, wetewete me te aukati tinihanga. Ka tukatuka pea a UMP i te tūnga whakaaetanga me ngā kōwhiringa tūmataitinga.

Ka taea te muku raraunga ā-rohe mā ngā āhuatanga muku o te taupānga, mā te ūkui raraunga taupānga i te OS, mā te tango rānei. Ka noho pea ngā tārua pūnaha, whakaahua mata, kōnae tiritiri rānei i raro i ngā kaupapa here a te kaiwhakarato. Kaua e whakauru raraunga tairongo ki ngā āpure kupu wātea.

### C. Whakaaetanga, SDK, tārua me te haumaru

Ka taea e te taupānga te whakamahi `INTERNET`, `ACCESS_NETWORK_STATE` me `com.google.android.gms.permission.AD_ID` mō ngā pānui me ngā pānui ā-ture. Ka whakamahia te uru whakaahua, kaitīpako whakaahua rānei anake ina kōwhiri te kaiwhakamahi ki te pānui kupu mai i te whakaahua.

Ka tukatuka pea a Google Mobile Ads SDK i te wāhitau IP, ngā pāhekoheko pānui, tātaritanga me ngā tautuhi pūrere/pūkete mō te pānuitanga, wetewete me te aukati tinihanga. Ka tukatuka pea a UMP i te tūnga whakaaetanga me ngā kōwhiringa tūmataitinga.

Ka taea te muku raraunga ā-rohe mā ngā āhuatanga muku o te taupānga, mā te ūkui raraunga taupānga i te OS, mā te tango rānei. Ka noho pea ngā tārua pūnaha, whakaahua mata, kōnae tiritiri rānei i raro i ngā kaupapa here a te kaiwhakarato. Kaua e whakauru raraunga tairongo ki ngā āpure kupu wātea.

---

## 11. Pārongo mō te Pārongo Tairongo

Kāore tēnei taupānga e tono kia whakaurua he pārongo tairongo.  
Ka tohutohungia ngā kaiwhakamahi kia kaua e whakauru i ngā ihirangi tairongo pērā i ngā pārongo hauora, ngā whakaaro tōrangapū, te whakapono, ngā pārongo koiora (biometric), ngā pārongo rānei e pā ana ki te ao taikaha ki roto i ngā tuhipoka, i ngā wāhanga whakauru mārire rānei.

Mēnā ka whakauru noa te kaiwhakamahi i ngā ihirangi tairongo, tērā pea ka penapenahia aua pārongo hei raraunga ā-rohe ki te pūrere e whakahaeretia tikatia ana e te kaiwhakamahi.

---


## 12. Te Tiaki i te Pārongo Whaiaro o ngā Tamariki

Kāore tēnei taupānga i hangaia mō ngā tamariki i te tuatahi.  
Ka taea e ngā kaitiaki te whakahaere i te whakamahinga mā ngā āhuatanga whakahaere mātua e whakaratohia ana e te pūrere, e te toa taupānga rānei.

---


## 13. Te Whakatau Aunoa

Kāore tēnei taupānga e whakahaere whakatau aunoa i runga i ngā pārongo whaiaro e hua ai ngā pānga ā-ture, ētahi pānga nui ōrite rānei.

---


## 14. Pānui Haumarutanga Raraunga (Google Play, me ērā atu)

Ka whakapau kaha te kaiwhakawhanake ki te pupuri me te whakahōu i ngā tūemi whakaaturanga haumarutanga raraunga i ngā mākete taupānga (pērā i a Google Play) kia hāngai ki ngā tikanga tukatuka tūturu a te taupānga me ngā tikanga tukatuka tūturu a ngā SDK rōpū-tuatoru.

Heoi anō, tērā pea ka rerekē ngā pārongo e whakaaturia ana i ngā toa taupānga i runga i te putanga taupānga, te whenua tohatoha, te whirihoranga SDK rōpū-tuatoru, me ngā panonitanga kaupapa here.

---


## 15. Pānui Pūtake Tuwhera

Ka whakamahi te taupānga i ētahi whare pukapuka pūtake tuwhera.  
Ka kitea ngā pārongo mō ngā raihana e hāngai ana i te mata e hāngai ana i roto i te taupānga, i ngā pānui rānei ka tukuna mā te hongere tohatoha.

---


## 16. Whakapā

Mō ngā pātai e pā ana ki tēnei Kaupapahere Tūmataiti:

- **Āpiha Tiaki Pārongo Whaiaro / Tangata Whakapā:** frog-im
- **Īmēra:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---


## 17. Ngā Panonitanga ki Tēnei Kaupapahere Tūmataiti

Ka taea te whakahou i tēnei Kaupapahere nā runga i ngā panonitanga o ngā ture / kaupapa here, ngā āhuatanga o te taupānga, ngā SDK rōpū-tuatoru rānei.  
Mēnā he panonitanga hira, ka taea te tuku pānui mā ngā pānui ā-roto o te taupānga, te whārangi tohatoha, ngā whakahōutanga rānei o te whārangi kaupapa here.

Whakahōu Whakamutunga: **2026-06-15**

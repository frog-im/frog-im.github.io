---
title: Kaupapahere Tūmataiti | know_me
description: know_me (PeopleNote, Memory for People) Kaupapahere Tūmataiti (Māori)
---

# Kaupapahere Tūmataiti (know_me / PeopleNote, Memory for People)

- **Ingoa Taupānga:** know_me (PeopleNote, Memory for People)
- **Kaiwhakawhanake:** frog-im
- **Āpiha Tiaki Pārongo Whaiaro / Tangata Whakapā:** frog-im
- **Whakapā:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Rā Whai Mana:** 2026-03-04
- **Whakahōu Whakamutunga:** 2026-03-04

> Kua whakaritea tēnei Kaupapahere i runga i ngā pārongo e tukatukahia ana e te taupānga me ōna āhuatanga e hāngai ana.  
> Mēnā ka whai mana ētahi ture, ētahi whakaritenga here rānei i tētahi whenua, i tētahi rohe rānei, ka taea e aua ture, e aua whakaritenga rānei te noho matua.

---

## 1. Te Kaupapa me te Whānuitanga

He taupānga a `know_me` i hangaia hei āwhina i ngā kaiwhakamahi ki te tuhi me te whakahaere pārongo mō ngā tāngata, ā, mēnā e hiahiatia ana, ki te pūrua, ki te whakahoki mai, ā, ki te tiritiri i aua pārongo hei kōnae PDF.

Kei roto i āna āhuatanga matua ēnei:

- Te penapena pārongo e hāngai ana ki tētahi tangata (pērā i te ingoa, te kuputuhi tautohu, ngā tuhipoka, ngā āhuatanga tangata, te whenua, te ira tangata, ngā pārongo whakapā, me ērā atu)
- Te whakarōpū kōpaki, te rapu, me ngā mahi whakakotahi
- Te tāpiri whakaahua me te whakahaere whakamārama
- Te kaweake me te kawemai i ngā pūrua (`.knm`)
- Te kaweake PDF
- Te raka taupānga (kupuhipa / tauira)
- Te whakahaere pānuitanga me te whakaae (AdMob / UMP)

Kāore te taupānga e tono kia rēhita motuhake he pūkete, ā, ka penapenahia ngā raraunga matua o te kaiwhakamahi o te taupānga ki te pūrere o te kaiwhakamahi i te nuinga o te wā.  
Heoi anō, tērā pea ka tukatukahia ētahi pārongo e ētahi SDK rōpū-tuatoru kua whakaurua mō te whakahaere pānuitanga me te whakaae.

---

## 2. Ngā Kāwai o te Pārongo Whaiaro e Tukatukahia Ana

### 2-1) Te Pārongo ka Whakaurua Tikatia e te Kaiwhakamahi

Ko ngā pārongo e whai ake nei ka penapenahia anake ina whakaurua tikatia e te kaiwhakamahi:

- Ingoa
- Kuputuhi tautohu (pērā i te āhua / ngā āhuatanga e whakamahia ana hei kuputuhi tuhipoka)
- Tuhipoka
- Ngā āhuatanga tangata, te whenua, te ira tangata
- Tau waea
- Kuputuhi e pā ana ki te wā i puta mai ai / te wā i tūtaki ai
- Pārongo tūāpapa / pae tukutuku
- Ingoa / tae kōpaki
- Whakamārama whakaahua (caption)

### 2-2) Ngā Kōnae ka Tīpakohia i runga i te Pūrere

- Ngā kōnae whakaahua ka tīpakohia e te kaiwhakamahi i te wā e tāpiri ana i ngā whakaahua
- Ngā kōnae pūrua `.knm` ka tīpakohia e te kaiwhakamahi i te wā e kawemai ana i ngā pūrua
- Ngā ara penapena me ngā kōnae kua penapenatia ka tīpakohia e te kaiwhakamahi i te wā e kaweake ana i ngā PDF / pūrua

### 2-3) Ngā Raraunga e Penapenahia Ā-Rohe ana i roto i te Taupānga

Ka taea te penapena i ngā raraunga e whai ake nei ki te pūrere o te kaiwhakamahi hei whakarato i ngā āhuatanga o te taupānga:

- SQLite DB (`people_note.db`): metadata mō ngā tāngata / kōpaki / tūāpapa / pae tukutuku / whakaahua
- Ngā kōnae whakaahua: kua whakamunatia, ā, ka penapenahia ki roto i te kōpaki tuhinga o te taupānga (`.enc`)
- Ngā tautuhinga taupānga (`SharedPreferences`): kaupapa, whakaraupapa, kōwhiringa tūmataiti / pānuitanga, kōwhiringa huna PDF, kaupapa here raka taupānga, me ērā atu
- Pārongo raka taupānga: ngā uara hash me ngā salt mō ngā kupuhipa / tauira (`SharedPreferences`)
- Ngā kī whakamuna ā-rohe: ka penapenahia ki `flutter_secure_storage`
- Ngā kōnae rangitahi: ngā arokite wetemunatanga whakaahua, ngā kōnae keteroki kawemai / kaweake, me ērā atu (kōpaki rangitahi)

### 2-4) Te Pārongo ka Taea te Tukatuka Aunoa i te Wā e Whakahaerehia ana te Pānuitanga me te Whakaae

Ina whakahohea ngā āhuatanga pānuitanga, whakahaere whakaae rānei, ka taea e ngā SDK a Google LLC me ōna hoa pānga (pērā i a AdMob me UMP) te tukatuka aunoa i ngā pārongo e whai ake nei:

- Ngā pūtāutu pānuitanga (AAID / IDFA, me ērā atu)
- Te wāhitau IP me ngā pārongo whatunga
- Ngā pārongo pūrere (putanga OS, tauira pūrere, putanga taupānga, me ērā atu)
- Ngā pārongo pāhekoheko pānuitanga (whakaaturanga, pāwhiri, me ērā atu)
- Te tūnga whakaae me ngā pārongo kōwhiringa tūmataiti
- Ngā pārongo e pā ana ki te tātari, te mahinga, me te haumarutanga

I te nuinga o te wā kāore ngā rekoata matua a te kaiwhakamahi o te taupānga e tukuna ake ki te tūmau a te kaiwhakawhanake, engari tērā pea ka tukuna ētahi o ngā pārongo kua whakahuatia ake nei ki ngā ratonga rōpū-tuatoru i te wā e whakamahia ana ngā āhuatanga pānuitanga / whakaae.

---

## 3. Te Kaupapa o te Tukatuka Pārongo Whaiaro

Ka tukatukahia e te taupānga ngā pārongo whaiaro, ngā pārongo e pā ana rānei mō ngā kaupapa e whai ake nei:

- Te tuhi me te tirotiro pārongo e pā ana ki ngā tāngata, e aro ana ki ngā hoapā / tuhipoka
- Te whakarato āhuatanga whakahaere pērā i te whakarōpū kōpaki, te rapu, me te whakakotahi
- Te tāpiri me te whakaatu whakaahua
- Te whakatutuki i ngā mahi e tonoa ana e te kaiwhakamahi pērā i te pūrua / whakahokinga mai me te kaweake PDF
- Te whakarato āhuatanga haumarutanga raka taupānga
- Te whakarato pānuitanga, te whakahaere whakaae, te ārai mahi tinihanga, me te whakatutuki herenga ā-ture

---

## 4. Te Wā Pupuri me te Rokiroki o te Pārongo Whaiaro

- Ngā raraunga ā-roto o te taupānga (SQLite, tautuhinga ā-rohe, whakaahua kua whakamunatia): ka pupuritia ki te pūrere o te kaiwhakamahi kia mukua rā anō te taupānga, kia whakawāteatia rānei ngā raraunga taupānga, kia mukua rānei e te kaiwhakamahi ngā raraunga
- Ngā kōnae rangitahi: ka mukua i muri i te otinga o te mahi e hāngai ana, ka whakawāteatia rānei i raro i te kaupapa here keteroki a te pūnaha whakahaere
- Ngā kōnae kua kaweakehia e te kaiwhakamahi (PDF, kōnae pūrua): tērā pea ka noho tonu ki te wāhi rokiroki i tīpakohia e te kaiwhakamahi, ā, me muku tikatia e te kaiwhakamahi
- Ngā raraunga e pā ana ki te pānuitanga / whakaae (e tukatukahia ana e ngā rōpū tuatoru): ka ārahina e ngā kaupapa here a ia kaiwhakarato ratonga me ngā ture e hāngai ana

Hei tikanga matua, kāore te taupānga e penapena i ngā rekoata matua a te kaiwhakamahi ki te tūmau a te kaiwhakawhanake.  
Heoi, ko ngā kōnae ka penapenahia tikatia e te kaiwhakamahi ki te rokiroki o waho ka whakahaerehia i roto i te taiao ake o te kaiwhakamahi.

---

## 5. Ngā Tukanga me ngā Tikanga mō te Whakakore i te Pārongo Whaiaro

Ina oti te kaupapa o te tukatuka, ina tono rānei te kaiwhakamahi kia mukua, ka whakakorehia e te taupānga ngā pārongo e hāngai ana, ka tukatukahia rānei kia kore e tohua anō, e whai ake nei.

### 5-1) Ngā Tukanga Whakakore

- Ina muku tika te kaiwhakamahi i ngā rekoata tangata takitahi, ngā kōpaki, ngā whakaahua, ngā raraunga pūrua, me ērā atu, ka whakaarohia aua raraunga hei raraunga me whakakore tonu.
- Ina muku te kaiwhakamahi i te taupānga, ka whakawātea rānei i ngā raraunga taupānga i ngā tautuhinga pūrere, ka tangohia ngā raraunga i penapenahia ki te wāhi rokiroki ā-roto o te taupānga i raro i ngā tukanga muku a te pūnaha whakahaere.
- Ka uru ngā kōnae rangitahi ki te tukanga whakawātea i muri i te mutunga o te mahi e hāngai ana, ā, tērā pea ka noho ētahi raraunga keteroki mō tētahi wā i raro i te kaupapa here a te pūnaha whakahaere.

### 5-2) Ngā Tikanga Whakakore

- Raraunga SQLite: te muku i ngā rekoata e hāngai ana
- Ngā tautuhinga taupānga (`SharedPreferences`): te muku i te kī e hāngai ana, i ngā tautuhinga katoa rānei
- Ngā uara `flutter_secure_storage`: te muku i ngā tūemi rokiroki haumaru e hāngai ana
- Ngā kōnae ā-roto o te taupānga (ngā whakaahua kua whakamunatia, ngā kōnae rangitahi, me ērā atu): te muku i ngā kōnae e hāngai ana
- Ngā PDF / kōnae pūrua ka penapenahia tikatia e te kaiwhakamahi ki te rokiroki o waho: kāore e mukua aunoa e te taupānga, ā, me muku tikatia e te kaiwhakamahi

Ki te kore e hiahiatia e ngā ture e hāngai ana te kē, kāore te kaiwhakawhanake e penapena wehe i ngā rekoata matua a te kaiwhakamahi ki te tūmau a te kaiwhakawhanake.

---

## 6. Te Tuku ki ngā Rōpū Tuatoru, te Tuku Mahi ki Waho, me te Whakawhiti Raraunga ki Tāwāhi

Ka taea e te taupānga te whakamahi i ngā ratonga a Google mō te whakahaere pānuitanga me te whakaae.

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

Kāore te kaiwhakawhanake e kohikohi, e hoko rānei i ngā raraunga matua o ngā rekoata tāngata o te taupānga mā tana ake tūmau.

---

## 7. Pārongo mō ngā Whakaaetanga e Whakamahia Ana

Ka taea e te taupānga te whakamahi i ngā whakaaetanga e whai ake nei:

- `INTERNET`: mō te whakawhiti kōrero a ngā SDK pānuitanga me ngā āhuatanga whatunga e hāngai ana
- `com.google.android.gms.permission.AD_ID`: mō te whakamahi i ngā pūtāutu pānuitanga (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 me raro iho): mō te tāpiri / tīpako whakaahua

Ka whakamahia ngā whakaaetanga i roto anake i te whānuitanga e tika ana hei whakarato i ngā āhuatanga e hāngai ana.

---

## 8. Te Tāutanga, te Whakahaere, me te Whakakore i ngā Tikanga Kohikohi Aunoa

Kāore tēnei taupānga e whakahaere tika i ngā pihikete paetukutuku whānui.  
Heoi anō, e pā ana ki ngā āhuatanga pānuitanga me te whakahaere whakaae, ka taea e ngā SDK rōpū-tuatoru te tukatuka aunoa i ngā pūtāutu pānuitanga, ngā pārongo whatunga, ngā pārongo pūrere, me ētahi raraunga ōrite.

Ka taea e ngā kaiwhakamahi te whakatika i ngā tautuhinga e hāngai ana mā ēnei ara:

- Te huri i ngā kōwhiringa i roto i ngā kōwhiringa tūmataiti o te taupānga, i te mata whakahaere whakaae rānei (ina wātea)
- Te tautuhi anō, te muku rānei i te ID pānuitanga i ngā tautuhinga pūnaha whakahaere o te pūrere
- Te whakaiti i ngā pānuitanga kua whakaritea mō te tangata, te whakatika rānei i ngā kōwhiringa tūmataiti e hāngai ana i ngā tautuhinga pūnaha whakahaere o te pūrere

Mēnā ka whakaiti te kaiwhakamahi i ngā pānuitanga kua whakaritea mō te tangata, tērā pea ka whakaatuhia ngā pānuitanga kāore i whakaritea mō te tangata, ka herea rānei ētahi āhuatanga e pā ana ki te pānuitanga.

---

## 9. Ngā Motika a te Kaiwhakamahi me te Āhua o te Whakatinana

I raro i ngā ture e hāngai ana, tērā pea kei ngā kaiwhakamahi ēnei motika:

- Te tono kia whai wāhi ki ngā pārongo whaiaro, kia whakatikahia, kia mukua rānei
- Te tono kia whakatārewatia, kia herea rānei te tukatuka
- Te whakahoki i te whakaae mō te tukatuka i runga anō i te whakaae
- Te huri i ngā kōwhiringa pānuitanga / whakaae

Ka taea te whakamahi i ēnei motika mā ēnei ara:

- Te whakatika, te muku rānei i ngā raraunga i roto tonu i te taupānga
- Te tīmata anō i ngā raraunga ā-rohe mā te muku i ngā raraunga taupānga, mā te tango rānei i te taupānga
- Te huri i te whakaae pānuitanga mā ngā kōwhiringa tūmataiti / mata whakaae o te taupānga (i ngā rohe e wātea ana)
- Te tautuhi anō / te muku i te ID pānuitanga, te whakaiti rānei i ngā pānuitanga kua whakaritea mō te tangata mā ngā tautuhinga OS o te pūrere
- **Whakapā:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Ngā Tikanga Haumarutanga

Ka whakatinanahia e te kaiwhakawhanake, ka whai rānei kia whakatinanahia, ngā tikanga e whai ake nei:

- Ka penapenahia ngā rekoata kaiwhakamahi ki te pūrere ā-rohe i te nuinga o te wā
- Ka penapenahia ngā kōnae whakaahua kua tāpirihia ki te āhua whakamuna ā-rohe (i runga i te AES-GCM)
- Ka penapenahia ngā pārongo raka taupānga ki te āhua hash, kaua ki te kuputuhi māori
- Ka penapenahia ngā kōnae pūrua i muri i te whakamunatanga i runga i te kupuhipa a te kaiwhakamahi
- Ka whakamunatia te whakawhiti kōrero ki ngā SDK rōpū-tuatoru (HTTPS / TLS)
- Ka whakamahia ngā whakaaetanga i raro i te whānuitanga iti rawa o te uru e tika ana

Heoi anō, kāore e taea te whakakore katoatia ngā tūraru ka puta mai i te āhua haumarutanga o te pūrere o te kaiwhakamahi (pērā i te rooting / jailbreaking, ngā taupānga kino, te whakakitea rānei o te rokiroki tiritahi).

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

Whakahōu Whakamutunga: **2026-03-04**
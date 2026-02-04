---
title: Beartas Príobháideachais | LyriFloat
description: Beartas Príobháideachais LyriFloat (Gaeilge)
lang: ga
last_updated: 2025-10-30
---

# Beartas Príobháideachais (LyriFloat)

- **Ainm na haipe:** LyriFloat  
- **Forbróir:** frog-im  
- **Teagmháil:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Dáta éifeachtach:** 2025-10-30

> Dréachtaíodh an beartas seo le tagairt do dhlíthe infheidhme, lena n-áirítear Acht Cosanta Faisnéise Pearsanta na Cóiré (PIPA), GDPR/UK GDPR, FADP na hEilvéise, agus dlíthe príobháideachais ábhartha i stáit SAM. Má tá ceanglais shonracha dlínse ann, bíonn tosaíocht acu sin.

---

## 1. Cuspóir agus Scóip

Cuireann an aip seo **eagarthóireacht ar mheiteashonraí comhaid fuaime** (teideal, ealaíontóir, srl.) atá stóráilte ar an ngléas agus gnéithe **forleagain liricí (lyrics overlay)** ar fáil.  
Ní chruthaíonn an aip cuntas úsáideora agus ní **uaslódálann** sí ábhar úsáideora chuig aon fhreastalaí. Déantar an phróiseáil **ar ghléas an úsáideora** de réir réamhshocraithe.

Mar sin féin, chun críocha **fógraíochta** agus **comhlíonta dlí**, féadfaidh comhpháirtithe tríú páirtí (m.sh., Google Mobile Ads SDK (AdMob), UMP) faisnéis ar nós **aitheantóirí fógraíochta** a bhailiú agus a phróiseáil. Leanann bailiú toiliú agus roghanna príobháideachais sonraíochtaí **Google UMP (User Messaging Platform)**.

---

## 2. Catagóirí Faisnéise a Phróiseálaimid

### 2-1) Comhaid a Roghnaíonn an tÚsáideoir go Sonrach
- **Conairí agus ábhar fuaime/íomhá chlúdaigh:** próiseáilte **go háitiúil** ar an ngléas chun eagarthóireacht/sábháil amháin.  
- Úsáidtear **FFmpegKit** go háitiúil le haghaidh ionchódaithe, eagarthóireachta meiteashonraí, agus eastóscadh mionsamhlacha.  
- Ní **uaslódálann** an aip comhaid roghnaithe an úsáideora chuig ár bhfreastalaithe.

### 2-2) Socruithe Áitiúla agus Luachanna Stóráilte

Chun feidhmiúlacht chroí agus áisiúlacht, stórálann an aip na luachanna seo a leanas **go háitiúil ar an ngléas**.  
Ní sheoltar iad chuig ár bhfreastalaithe agus baintear iad nuair a scriostar an aip nó a sonraí.

#### (1) Roghanna (`shared_preferences`)
| Cineál | Eochair/Ábhar | Cuspóir | Stóráil | Scriosadh |
|---|---|---|---|---|
| Suíomh/cló forleagain | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Suíomh forleagain agus méid cló a athchóiriú | SharedPreferences an ghléis | Baintear nuair a scriostar sonraí na haipe nó an aip |
| Socruithe Fógraí/Príobháideachais | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Fógraí neamhphearsantaithe, RDP SAM, clib COPPA, clib aoise, teorainn rátála ábhair fógraí | SharedPreferences an ghléis | Mar an gcéanna leis an gcolún ar chlé |

#### (2) Comhaid Sealadacha (fillteán temp an chórais)
- **Samplaí:** `cover_*.jpg`, `tmp_*.flac`  
- **Úsáid:** eastóscadh clúdaigh, clibeáil FLAC, ionchódú sealadach  
- **Suíomh:** fillteán sealadach OS (`systemTemp`)  
- **Coinneáil:** baintear ag an aip nuair is féidir tar éis críochnaithe; faoi réir glantacháin OS freisin

#### (3) Sábháil Roghnaithe ag an Úsáideoir (SAF)
- Nuair a roghnaíonn an t-úsáideoir “Save As,” féadfar comhaid fuaime deiridh a scríobh chuig suíomhanna roghnaithe (m.sh., Íoslódálacha, scamall).  
- Fanann na comhaid seo i **stóráil sheachtrach** agus **fanann siad tar éis díshuiteála**. Is féidir leis an úsáideoir iad a scriosadh de láimh.

#### (4) Stádas Toiliú (Taisce SDK UMP)
- I réigiúin EEA/UK/CH, **taisceann** SDK UMP stádas toiliú fógraí an úsáideora go háitiúil.  
- Is féidir é a athshocrú trí shonraí na haipe a scriosadh nó tríd an scáileán **Privacy Options** san aip nuair atá sé ar fáil.

---

### 2-3) Sonraí a Bhaineann le Fógraí agus Toiliú (SDKanna Tríú Páirtí)
- Féadfaidh **Google Mobile Ads SDK (AdMob) agus UMP** a bhailiú/próiseáil, mar shampla: **AAID/IDFA**, **raonta IP**, **faisnéis ghléis/aipe**, **comharthaí idirghníomhaíochta fógraí**, **stádas toiliú**, srl.  
- **Cuspóirí:** seachadadh fógraí, teorannú minicíochta, cosc calaoise, tomhas feidhmíochta, comhlíonadh dlí  
- **Réigiúin a éilíonn toiliú (EEA/UK/CH):** bailítear toiliú trí UMP agus cuirtear scáileán **Privacy Options** ar fáil nuair is gá.  
  I réigiúin nach bhfuil gá dlíthiúil leis (m.sh., KR), **b’fhéidir nach dtaispeánfar** an rogha.

---

## 3. Próiseáil agus Coinneáil

- **Socruithe áitiúla:** stóráilte ar an ngléas go dtí go scriosann an t-úsáideoir sonraí na haipe nó go ndíshuiteálann sé/sí an aip  
- **Comhaid sealadacha:** cruthaítear le linn ionchódaithe/eastóscadh, scriostar tar éis próiseála nó féadfaidh siad fanacht go sealadach i gcatheanna OS  
- **Sonraí fógraí/toiliú (tríú páirtí):** coinneáil agus diúscairt de réir **bheartais Google**

---

## 4. Aistrithe Tríú Páirtí agus Sreafaí Sonraí Tras-Teorann

Chun fógraíocht agus bainistíocht toiliú, féadfar faisnéis úsáideora a tharchur chuig agus a phróiseáil ar bhonneagar Google.

| Mír | Sonraí |
|---|---|
| **Faighteoir** | Google LLC agus a chuid cleamhnaithe/fos-phróiseálaithe |
| **Ceann scríbe** | Stáit Aontaithe Mheiriceá (agus réigiúin eile ina bhfuil bonneagar Google) |
| **Cuspóir** | Seachadadh fógraí, feidhmíocht/tomhas, comhlíonadh dlí, bainistíocht toiliú |
| **Sonraí** | Aitheantóirí fógraí, raonta IP, faisnéis ghléis/aipe, idirghníomhaíochtaí fógraí, stádas toiliú, srl. |
| **Coinneáil** | De réir bheartais Google |
| **Éifeacht diúltaithe** | D’fhéadfadh fógraí pearsantaithe a bheith teoranta; d’fhéadfaí fógraí neamhphearsantaithe a thaispeáint |

Comhlíonann muid ceanglais nochta **Google Play Data safety** agus coimeádaimid na nochtaí ailínithe leis an bpróiseáil iarbhír.

---

## 5. Do Chearta agus Conas Iad a Fheidhmiú

- **Diúltú do fhógraí pearsantaithe / toiliú a athrú**  
  - I réigiúin tacaithe (EEA/UK/CH): athraigh i **Settings → Privacy Options**.  
  - I réigiúin eile: úsáid socruithe an OS chun **aitheantóirí fógraí a athshocrú / rianú fógraí a theorannú**.
- **Athshocrú faisnéise áitiúla:** scriosadh sonraí na haipe nó díshuiteáil athshocraíonn comhordanáidí forleagain, méid cló, agus socruithe áitiúla eile.
- Is féidir cearta faoi **GDPR/UK GDPR/Swiss FADP/dlíthe príobháideachais stáit SAM** (rochtain, ceartú, scriosadh, inaistritheacht, srian, tarraingt siar toiliú, srl.) a fheidhmiú de réir na ndlíthe sin.  
  Maidir le sonraí fógraíochta a phróiseálann Google, bain úsáid as **próisis Google**.

---

## 6. Príobháideachas Leanaí

Níl an aip seo dírithe ar leanaí. Má úsáideann leanbh faoi bhun aoise íosta dlíthiúla í, ba cheart stopadh agus gnéithe teorannaithe fógraí ar leibhéal OS a úsáid le caomhnóir. Nuair is cuí, féadfaimid **TFUA (clib seirbhís dírithe ar leanaí)** nó roghanna cosanta leanaí dá samhail a chur i bhfeidhm.

---

## 7. Bearta Slándála

- **Íoslaghdú sonraí** i mbailiú agus i stóráil  
- Úsáid **theoranta** comhad sealadach agus iarrachtaí scriosadh tar éis próiseála  
- Próiseáil go docht **laistigh de raon ceadanna OS**  
- Criptiú **TLS nó a chomhionann** le linn aistrithe tríú páirtí (de réir chaighdeáin SDK)

---

## 8. Data Safety (Google Play)

Ullmhaímid agus coinnímid an rannán **Data safety** sa Play Console go cruinn, agus nuashonraímid go pras é nuair a athraíonn rudaí.

---

## 9. Fógraí Open-source

Úsáideann an aip bogearraí open-source ar nós **FFmpeg**. Míníonn comhad faisnéise (m.sh., `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) laistigh den aip conas an cód foinse a fháil. Ar iarratas, cuirfimid an fhoinse ar fáil mar a ordaítear sa chomhad sin.

---

## 10. Teagmháil

- Ríomhphost: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Athruithe ar an mBeartas Seo

Féadfaimid an beartas seo a leasú de bharr athruithe dlí nó seirbhíse. Postálfaimid nuashonruithe **san aip** agus ar an **leathanach beartais** seo.  
Le haghaidh athruithe ábhartha, tabharfaimid fógra **7 lá ar a laghad** roimh an dáta éifeachtach.

---

## Aguisín: Treoir don Úsáideoir

- **Nasc san aip:** oscail an leathanach seo ó **Settings → Privacy**.  
- **Iompar réigiúnach:** in EEA/UK/CH, taispeántar Privacy Options. **In KR agus i roinnt réigiún eile, b’fhéidir nach dtaispeánfaidh an cnaipe roghanna breise** nuair nach bhfuil sé riachtanach go dlíthiúil.

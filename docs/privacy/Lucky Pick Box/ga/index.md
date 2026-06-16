---
title: Polasaí Príobháideachais | Lucky Pick Box
description: Lucky Pick Box Polasaí Príobháideachais
lang: ga
last_updated: 2026-06-15
---

# Polasaí Príobháideachais (Lucky Pick Box / 뽑기박스)

- **Ainm an Aip:** Lucky Pick Box / 뽑기박스
- **Forbróir:** frog-im
- **Oifigeach Cosanta Faisnéise Pearsanta / Duine Teagmhála:** frog-im
- **Teagmháil:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Dáta Teacht i bhFeidhm:** 2026-06-12
- **Nuashonraithe go Deireanach:** 2026-06-15

> Ullmhaíodh an Beartas seo bunaithe ar an bhfaisnéis a phróiseálann an aip agus ar na gnéithe gaolmhara atá aici.  
> Má bhaineann aon dlíthe nó rialacháin éigeantacha le tír nó réigiún ar leith, féadfaidh na dlíthe nó na rialacháin sin tosaíocht a bheith acu.

---

## 1. Cuspóir agus Raon Feidhme

Is uirlis ócáideach é Lucky Pick Box le haghaidh roghanna randamacha, crannchuir, roghnú ord, roinnt foirne, dísle, boinn, dréimirí, rothaí agus cluichí cinnteoireachta laethúla nó grúpa dá samhail. Ní sholáthraíonn an aip cearrbhachas fíor-airgid, gealltóireacht, idirbhearta airgeadais, duaiseanna airgid ná luaíochtaí atá comhionann le hairgead.

### A. Príomhghnéithe

- Ionchur tapa: téacs a chlóscríobhann an t-úsáideoir nó téacs a léitear ó íomhá roghnaithe.
- Cluichí rogha randamaí: ladder, wheel, plinko, simple draw, dice, coin, random number, team splitter, order picker, card, bomb agus yes/no.
- Stair torthaí: cineál cluiche, teideal, rannpháirtithe/ítimí, achoimre toraidh agus am cruthaithe a shábháil.
- Sliotáin socruithe: is féidir le roinnt cluichí rannpháirtithe, liostaí, raonta, cainníochtaí, foirne, meáchain agus socruithe dá leithéid a shábháil i suas le 3 sliotán áitiúla.

Ní éilíonn an aip clárú ná logáil isteach. Ní oibrímid freastalaí a fhaigheann ón aip d'ainm, d'uimhir ghutháin, do sheoladh ríomhphoist, do theagmhálaithe, iontrálacha cluiche, íomhánna roghnaithe nó torthaí cluiche.

Chun gnéithe a sholáthar, féadfaidh an aip iontrálacha cluiche, lipéid rannpháirtithe, torthaí le déanaí, socruithe cluiche sábháilte, socruithe beochana, roghanna príobháideachais fógraí agus stádas a bhaineann le toiliú a stóráil i stóráil áitiúil do ghléis. Tá stair na dtorthaí le déanaí teoranta ag an aip agus ní sheoltar í chuig freastalaí a oibríonn an forbróir.

---

## 2. Catagóirí na Faisnéise Pearsanta a Phróiseáiltear

### 2-1) Faisnéis a Iontrálann an tÚsáideoir go Díreach

Ní éilíonn an aip clárú ná logáil isteach. Ní oibrímid freastalaí a fhaigheann ón aip d'ainm, d'uimhir ghutháin, do sheoladh ríomhphoist, do theagmhálaithe, iontrálacha cluiche, íomhánna roghnaithe nó torthaí cluiche.

### 2-2) Comhaid a Roghnaítear ar an nGléas

Má roghnaíonn tú téacs a léamh ó íomhá, iarrann an aip ort íomhá a roghnú ó do leabharlann grianghraf. Úsáidtear an íomhá roghnaithe le haghaidh aithint téacs ar an ngléas trí roghnóir íomhánna an ardáin agus comhpháirteanna Google ML Kit. Ní uaslódálann an forbróir an íomhá chuig freastalaí dá chuid agus ní choinníonn sé í i gcuntas cianda.

### 2-3) Sonraí a Stóráiltear go hÁitiúil Laistigh den Aip

Chun gnéithe a sholáthar, féadfaidh an aip iontrálacha cluiche, lipéid rannpháirtithe, torthaí le déanaí, socruithe cluiche sábháilte, socruithe beochana, roghanna príobháideachais fógraí agus stádas a bhaineann le toiliú a stóráil i stóráil áitiúil do ghléis. Tá stair na dtorthaí le déanaí teoranta ag an aip agus ní sheoltar í chuig freastalaí a oibríonn an forbróir.

### B. Sonraí áitiúla ar an ngléas

| Suíomh nó eochair | Sonraí | Cuspóir | Scriosadh |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, cineál cluiche, teideal, rannpháirtithe/ítimí, achoimre, am; suas le 50 toradh le déanaí. | Torthaí le déanaí agus stair a thaispeáint. | Scriosadh san aip, sonraí aip a ghlanadh nó díshuiteáil |
| `game_settings.<gameId>.slot_<n>` | Socruithe cluiche, am sábháilte, liostaí, raonta, cainníochtaí, foirne, meáchain; suas le 3 sliotán. | Socruithe cluiche a luchtú arís. | Sliotán a ghlanadh, sonraí a ghlanadh nó díshuiteáil |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Socruithe beochana agus lánscáileáin. | Roghanna taispeána a choinneáil. | Socruithe a athrú, sonraí a ghlanadh nó díshuiteáil |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Roghanna príobháideachais fógraí agus comhaireamh minicíochta fógraí. | Roghanna réigiúnacha a chur i bhfeidhm agus minicíocht a rialú. | Socruithe a athrú, sonraí a ghlanadh nó díshuiteáil |
| Roghnóir íomhá agus OCR | D'fhéadfadh cosán na híomhá roghnaithe agus an téacs aitheanta a phróiseáil go sealadach. | Téacs íomhá a chur leis an ionchur tapa. | Taisce aip/OS nó glanadh sonraí |

Ní sheoltar téacs ionchuir thapa chuig freastalaí an fhorbróra. Ní éiríonn sé ina shonraí áitiúla ach má úsáidtear é i dtoradh nó i socrú sábháilte.

### 2-4) Faisnéis a D’fhéadfadh a Bheith Próiseáilte go hUathoibríoch le linn Láimhseála Fógraíochta agus Toilithe

Ar ardáin a dtacaítear leo, Android faoi láthair, úsáideann an aip Google AdMob agus Google User Messaging Platform (UMP). Féadfaidh Google agus comhpháirtithe fógraíochta aitheantóirí fógraíochta, aitheantóirí sampla aip, seoladh IP, suíomh garbh, faisnéis gléis agus líonra, leagan aip, córas oibriúcháin, teanga, taispeántais fógraí, cliceálacha agus idirghníomhaíochtaí, diagnóisic, stádas toilithe agus socruithe réigiúnacha príobháideachais fógraí a phróiseáil chun fógraí a sheachadadh, minicíocht a theorannú, calaois a chosc, toiliú a bhainistiú, tomhas, anailís, slándáil agus comhlíonadh dlíthiúil a dhéanamh.

Déantar cur síos ar chleachtais phríobháideachais Google ag https://policies.google.com/privacy agus https://policies.google.com/technologies/ads.

---

## 3. Cuspóir Phróiseáil na Faisnéise Pearsanta

Is uirlis ócáideach é Lucky Pick Box le haghaidh roghanna randamacha, crannchuir, roghnú ord, roinnt foirne, dísle, boinn, dréimirí, rothaí agus cluichí cinnteoireachta laethúla nó grúpa dá samhail. Ní sholáthraíonn an aip cearrbhachas fíor-airgid, gealltóireacht, idirbhearta airgeadais, duaiseanna airgid ná luaíochtaí atá comhionann le hairgead.

### A. Príomhghnéithe

- Ionchur tapa: téacs a chlóscríobhann an t-úsáideoir nó téacs a léitear ó íomhá roghnaithe.
- Cluichí rogha randamaí: ladder, wheel, plinko, simple draw, dice, coin, random number, team splitter, order picker, card, bomb agus yes/no.
- Stair torthaí: cineál cluiche, teideal, rannpháirtithe/ítimí, achoimre toraidh agus am cruthaithe a shábháil.
- Sliotáin socruithe: is féidir le roinnt cluichí rannpháirtithe, liostaí, raonta, cainníochtaí, foirne, meáchain agus socruithe dá leithéid a shábháil i suas le 3 sliotán áitiúla.

Ar ardáin a dtacaítear leo, Android faoi láthair, úsáideann an aip Google AdMob agus Google User Messaging Platform (UMP). Féadfaidh Google agus comhpháirtithe fógraíochta aitheantóirí fógraíochta, aitheantóirí sampla aip, seoladh IP, suíomh garbh, faisnéis gléis agus líonra, leagan aip, córas oibriúcháin, teanga, taispeántais fógraí, cliceálacha agus idirghníomhaíochtaí, diagnóisic, stádas toilithe agus socruithe réigiúnacha príobháideachais fógraí a phróiseáil chun fógraí a sheachadadh, minicíocht a theorannú, calaois a chosc, toiliú a bhainistiú, tomhas, anailís, slándáil agus comhlíonadh dlíthiúil a dhéanamh.

Déantar cur síos ar chleachtais phríobháideachais Google ag https://policies.google.com/privacy agus https://policies.google.com/technologies/ads.

---

## 4. Tréimhse Choinneála agus Stórála na Faisnéise Pearsanta

Féadfaidh stair áitiúil agus socruithe fanacht ar do ghléas go dtí go scriosann tú an stair, go nglanann tú sonraí na haipe nó go ndíshuiteálann tú an aip. Is féidir leat roghanna príobháideachais fógraí atá ar fáil a athrú i socruithe na haipe, roghanna príobháideachais Google a oscailt nuair is gá, agus aitheantóirí fógraíochta a bhainistiú nó a athshocrú i socruithe príobháideachais an ghléis. Rialaítear coinneáil faisnéise a phróiseálann Google ag polasaithe agus oibleagáidí dlíthiúla Google.

### B. Sonraí áitiúla ar an ngléas

| Suíomh nó eochair | Sonraí | Cuspóir | Scriosadh |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, cineál cluiche, teideal, rannpháirtithe/ítimí, achoimre, am; suas le 50 toradh le déanaí. | Torthaí le déanaí agus stair a thaispeáint. | Scriosadh san aip, sonraí aip a ghlanadh nó díshuiteáil |
| `game_settings.<gameId>.slot_<n>` | Socruithe cluiche, am sábháilte, liostaí, raonta, cainníochtaí, foirne, meáchain; suas le 3 sliotán. | Socruithe cluiche a luchtú arís. | Sliotán a ghlanadh, sonraí a ghlanadh nó díshuiteáil |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Socruithe beochana agus lánscáileáin. | Roghanna taispeána a choinneáil. | Socruithe a athrú, sonraí a ghlanadh nó díshuiteáil |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Roghanna príobháideachais fógraí agus comhaireamh minicíochta fógraí. | Roghanna réigiúnacha a chur i bhfeidhm agus minicíocht a rialú. | Socruithe a athrú, sonraí a ghlanadh nó díshuiteáil |
| Roghnóir íomhá agus OCR | D'fhéadfadh cosán na híomhá roghnaithe agus an téacs aitheanta a phróiseáil go sealadach. | Téacs íomhá a chur leis an ionchur tapa. | Taisce aip/OS nó glanadh sonraí |

Ní sheoltar téacs ionchuir thapa chuig freastalaí an fhorbróra. Ní éiríonn sé ina shonraí áitiúla ach má úsáidtear é i dtoradh nó i socrú sábháilte.

---

## 5. Nósanna Imeachta agus Modhanna chun Faisnéis Phearsanta a Scriosadh

Féadfaidh stair áitiúil agus socruithe fanacht ar do ghléas go dtí go scriosann tú an stair, go nglanann tú sonraí na haipe nó go ndíshuiteálann tú an aip. Is féidir leat roghanna príobháideachais fógraí atá ar fáil a athrú i socruithe na haipe, roghanna príobháideachais Google a oscailt nuair is gá, agus aitheantóirí fógraíochta a bhainistiú nó a athshocrú i socruithe príobháideachais an ghléis. Rialaítear coinneáil faisnéise a phróiseálann Google ag polasaithe agus oibleagáidí dlíthiúla Google.

### C. Ceadanna, SDKanna, cúltacaí agus slándáil

D'fhéadfadh an aip `INTERNET`, `ACCESS_NETWORK_STATE` agus `com.google.android.gms.permission.AD_ID` a úsáid le haghaidh fógraí agus fógraí dlí. Ní úsáidtear rochtain grianghraf nó roghnóir íomhá ach nuair a roghnaíonn an t-úsáideoir téacs a léamh ó íomhá.

D'fhéadfadh Google Mobile Ads SDK seoladh IP, idirghníomhaíochtaí fógraí, diagnóisic agus aitheantóirí gléis/cuntais a phróiseáil le haghaidh fógraíochta, anailíse agus cosc calaoise. D'fhéadfadh UMP stádas toilithe agus roghanna príobháideachais a phróiseáil.

Is féidir sonraí áitiúla a scriosadh trí ghnéithe scriosta san aip, scriosadh sonraí aip san OS nó díshuiteáil. D'fhéadfadh cúltacaí córais, screenshots nó comhaid roinnte fanacht de réir bheartais an tsoláthraí. Seachain sonraí íogaire i réimsí téacs saor.

---

## 6. Soláthar do Thríú Páirtithe, Foinsiú Seachtrach, agus Aistriú Trasteorann

Ní dhíolaimid d'iontrálacha cluiche, lipéid rannpháirtithe, torthaí cluiche ná íomhánna roghnaithe. Nuair a iarrtar gnéithe fógraí nó toilithe, féadfaidh Google LLC, cleamhnaithe Google agus a soláthraithe seirbhíse faisnéis fógraíochta agus toilithe a phróiseáil i dtíortha lasmuigh de do thír nó réigiún. Féach "Fógra um Aistriú Idirnáisiúnta Sonraí" san aip le haghaidh tuilleadh sonraí.

| Mír | Sonraí |
|---|---|
| **Faighteoir / Páirtí Iontaofa** | Google LLC agus a chleamhnaithe (oibreoirí AdMob / UMP) |
| **Tír an Aistrithe** | Stáit Aontaithe Mheiriceá agus réigiúin ina n-oibrítear bonneagar Google |
| **Am an Aistrithe** | Ar bhonn leanúnach le linn iarrataí fógraí, seiceálacha stádais toilithe, túsú SDK, agus oibriú |
| **Modh an Aistrithe** | Tarchur trí chumarsáid líonra idir an aip agus freastalaithe tríú páirtí |
| **Bunús Dlí don Aistriú Trasteorann** | Próiseáiltear laistigh den raon atá riachtanach chun an tseirbhís a sholáthar faoi bhunúis dlí is infheidhme, nó, nuair is gá, bunaithe ar thoiliú ábhar na sonraí |
| **Cuspóir** | Freastal fógraí, tomhas fógraí, bainistiú toilithe, cosc calaoise, agus comhlíonadh le beartais / dlíthe |
| **Catagóirí Sonraí (Samplaí)** | Aitheantóirí fógraíochta (AAID / IDFA), faisnéis IP / líonra, faisnéis gléis / aip, faisnéis idirghníomhaíochta fógra, stádas toilithe |
| **Tréimhse Choinneála** | Faoi réir bheartais Google agus na ndlíthe is infheidhme |
| **Éifeacht an Diúltaithe** | Féadfar fógraí pearsantaithe a theorannú, féadfar fógraí neamhphearsantaithe a sholáthar, nó féadfar roinnt gnéithe a bhaineann le fógraí a shrianadh |

---

## 7. Faisnéis faoi na Ceadanna a Úsáidtear

### C. Ceadanna, SDKanna, cúltacaí agus slándáil

D'fhéadfadh an aip `INTERNET`, `ACCESS_NETWORK_STATE` agus `com.google.android.gms.permission.AD_ID` a úsáid le haghaidh fógraí agus fógraí dlí. Ní úsáidtear rochtain grianghraf nó roghnóir íomhá ach nuair a roghnaíonn an t-úsáideoir téacs a léamh ó íomhá.

D'fhéadfadh Google Mobile Ads SDK seoladh IP, idirghníomhaíochtaí fógraí, diagnóisic agus aitheantóirí gléis/cuntais a phróiseáil le haghaidh fógraíochta, anailíse agus cosc calaoise. D'fhéadfadh UMP stádas toilithe agus roghanna príobháideachais a phróiseáil.

Is féidir sonraí áitiúla a scriosadh trí ghnéithe scriosta san aip, scriosadh sonraí aip san OS nó díshuiteáil. D'fhéadfadh cúltacaí córais, screenshots nó comhaid roinnte fanacht de réir bheartais an tsoláthraí. Seachain sonraí íogaire i réimsí téacs saor.

---

## 8. Suiteáil, Oibriú, agus Diúltú do Mheicníochtaí Bailithe Uathoibríche

Ar ardáin a dtacaítear leo, Android faoi láthair, úsáideann an aip Google AdMob agus Google User Messaging Platform (UMP). Féadfaidh Google agus comhpháirtithe fógraíochta aitheantóirí fógraíochta, aitheantóirí sampla aip, seoladh IP, suíomh garbh, faisnéis gléis agus líonra, leagan aip, córas oibriúcháin, teanga, taispeántais fógraí, cliceálacha agus idirghníomhaíochtaí, diagnóisic, stádas toilithe agus socruithe réigiúnacha príobháideachais fógraí a phróiseáil chun fógraí a sheachadadh, minicíocht a theorannú, calaois a chosc, toiliú a bhainistiú, tomhas, anailís, slándáil agus comhlíonadh dlíthiúil a dhéanamh.

Déantar cur síos ar chleachtais phríobháideachais Google ag https://policies.google.com/privacy agus https://policies.google.com/technologies/ads.

Féadfaidh stair áitiúil agus socruithe fanacht ar do ghléas go dtí go scriosann tú an stair, go nglanann tú sonraí na haipe nó go ndíshuiteálann tú an aip. Is féidir leat roghanna príobháideachais fógraí atá ar fáil a athrú i socruithe na haipe, roghanna príobháideachais Google a oscailt nuair is gá, agus aitheantóirí fógraíochta a bhainistiú nó a athshocrú i socruithe príobháideachais an ghléis. Rialaítear coinneáil faisnéise a phróiseálann Google ag polasaithe agus oibleagáidí dlíthiúla Google.

---

## 9. Cearta Úsáideora agus Conas Iad a Fheidhmiú

Féadfaidh stair áitiúil agus socruithe fanacht ar do ghléas go dtí go scriosann tú an stair, go nglanann tú sonraí na haipe nó go ndíshuiteálann tú an aip. Is féidir leat roghanna príobháideachais fógraí atá ar fáil a athrú i socruithe na haipe, roghanna príobháideachais Google a oscailt nuair is gá, agus aitheantóirí fógraíochta a bhainistiú nó a athshocrú i socruithe príobháideachais an ghléis. Rialaítear coinneáil faisnéise a phróiseálann Google ag polasaithe agus oibleagáidí dlíthiúla Google.

---

## 10. Bearta Slándála

### C. Ceadanna, SDKanna, cúltacaí agus slándáil

D'fhéadfadh an aip `INTERNET`, `ACCESS_NETWORK_STATE` agus `com.google.android.gms.permission.AD_ID` a úsáid le haghaidh fógraí agus fógraí dlí. Ní úsáidtear rochtain grianghraf nó roghnóir íomhá ach nuair a roghnaíonn an t-úsáideoir téacs a léamh ó íomhá.

D'fhéadfadh Google Mobile Ads SDK seoladh IP, idirghníomhaíochtaí fógraí, diagnóisic agus aitheantóirí gléis/cuntais a phróiseáil le haghaidh fógraíochta, anailíse agus cosc calaoise. D'fhéadfadh UMP stádas toilithe agus roghanna príobháideachais a phróiseáil.

Is féidir sonraí áitiúla a scriosadh trí ghnéithe scriosta san aip, scriosadh sonraí aip san OS nó díshuiteáil. D'fhéadfadh cúltacaí córais, screenshots nó comhaid roinnte fanacht de réir bheartais an tsoláthraí. Seachain sonraí íogaire i réimsí téacs saor.

### C. Ceadanna, SDKanna, cúltacaí agus slándáil

D'fhéadfadh an aip `INTERNET`, `ACCESS_NETWORK_STATE` agus `com.google.android.gms.permission.AD_ID` a úsáid le haghaidh fógraí agus fógraí dlí. Ní úsáidtear rochtain grianghraf nó roghnóir íomhá ach nuair a roghnaíonn an t-úsáideoir téacs a léamh ó íomhá.

D'fhéadfadh Google Mobile Ads SDK seoladh IP, idirghníomhaíochtaí fógraí, diagnóisic agus aitheantóirí gléis/cuntais a phróiseáil le haghaidh fógraíochta, anailíse agus cosc calaoise. D'fhéadfadh UMP stádas toilithe agus roghanna príobháideachais a phróiseáil.

Is féidir sonraí áitiúla a scriosadh trí ghnéithe scriosta san aip, scriosadh sonraí aip san OS nó díshuiteáil. D'fhéadfadh cúltacaí córais, screenshots nó comhaid roinnte fanacht de réir bheartais an tsoláthraí. Seachain sonraí íogaire i réimsí téacs saor.

---

## 11. Faisnéis maidir le Faisnéis Íogair

Ní éilíonn an aip seo ionchur faisnéise íogaire.  
Moltar d’úsáideoirí gan ábhar íogair amhail faisnéis sláinte, tuairimí polaitiúla, reiligiún, faisnéis bhithmhéadrach, nó faisnéis a bhaineann leis an saol gnéasach a iontráil i nótaí nó i réimsí ionchuir saorscríofa.

Má iontrálann úsáideoir ábhar íogair go deonach, féadfar an fhaisnéis sin a stóráil mar shonraí áitiúla ar an ngléas a bhainistíonn an t-úsáideoir go díreach.

---


## 12. Cosaint Faisnéise Pearsanta Leanaí

Níor dearadh an aip seo go príomha do leanaí.  
Féadfaidh caomhnóirí úsáid a bhainistiú trí ghnéithe rialaithe tuismitheoirí a sholáthraíonn an gléas nó an siopa aip.

---


## 13. Cinnteoireacht Uathoibríoch

Ní dhéanann an aip seo cinnteoireacht uathoibríoch bunaithe ar fhaisnéis phearsanta a tháirgeann éifeachtaí dlíthiúla nó tionchair shuntasacha chomhchosúla.

---


## 14. Fógra um Shábháilteacht Sonraí (Google Play, etc.)

Déanann an forbróir iarracht na míreanna nochta sábháilteachta sonraí i margadh aipeanna (amhail Google Play) a chothabháil agus a nuashonrú i gcomhréir le cleachtais iarbhír phróiseála na haipe agus cleachtais iarbhír phróiseála SDKanna tríú páirtí.

Mar sin féin, féadfaidh an fhaisnéis a thaispeántar i siopaí aipeanna a bheith éagsúil ag brath ar leagan na haipe, tír an dáileacháin, cumraíocht SDK tríú páirtí, agus athruithe beartais.

---


## 15. Fógra Foinse Oscailte

Úsáideann an aip roinnt leabharlann foinse oscailte.  
Is féidir faisnéis faoi na ceadúnais ábhartha a fháil ar an scáileán gaolmhar laistigh den aip nó sna fógraí a chuirtear ar fáil tríd an gcainéal dáileacháin.

---


## 16. Teagmháil

Le haghaidh fiosrúchán maidir leis an bPolasaí Príobháideachais seo:

- **Oifigeach Cosanta Faisnéise Pearsanta / Duine Teagmhála:** frog-im
- **Ríomhphost:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---


## 17. Athruithe ar an bPolasaí Príobháideachais seo

Féadfar an Beartas seo a athbhreithniú mar gheall ar athruithe i ndlíthe / beartais, gnéithe na haipe, nó SDKanna tríú páirtí.  
Má tá athruithe ábhartha ann, féadfar fógra a thabhairt trí fhógraí laistigh den aip, an leathanach dáileacháin, nó nuashonruithe ar leathanach an bheartais.

Nuashonraithe go Deireanach: **2026-06-15**

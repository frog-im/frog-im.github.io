---
title: Polasaí Príobháideachais | Power lucky lotto
description: Polasaí Príobháideachais Power lucky lotto (Gaeilge)
lang: ga
last_updated: 2026-01-29
---

# Polasaí Príobháideachais (Power lucky lotto)

- **Ainm na haipe:** Power lucky lotto  
- **Forbróir:** frog-im  
- **Teagmháil:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Dáta éifeachtach:** 2026-01-29  

> Scríobhadh an polasaí seo ag tagairt do dhlíthe príobháideachais is infheidhme amhail PIPA na Cóiré, GDPR/UK GDPR, FADP na hEilvéise, agus dlíthe príobháideachais stáit ábhartha sna S.A.  
> Má tá ceanglais éigeantacha shonracha i do réigiún, tá tús áite acu.

---

## 1. Cuspóir agus raon feidhme

Is aip í Power lucky lotto chun cluichí crannchuir a bhainistiú agus taifid a fheiceáil. I measc na bpríomhghnéithe tá:

- Roghnú tíre/cluiche agus socrú (m.sh., KR 6/45, US Powerball)  
- Giniúint/sábháil uimhreacha agus amharc ar logaí (stair)  
- Amharc agus scrios táblaí logaí (liosta táblaí/sonraí)  
- Eagarthóireacht/bainistíocht sonraí torthaí trí JSON (do staitisticí/amléiriú)  
- Fógraí (lena n-áirítear fógraí luaíochta) agus bainistíocht toilithe (nuair is gá)

**Ní éilíonn** an aip **cuntas**, agus de réir réamhshocraithe **ní uaslódálann sí do shonraí chuig freastalaithe an fhorbróra.**  
Déantar formhór na próiseála **ar do ghléas**.

Mar sin féin, le haghaidh **fógraíochta**, **bainistíocht toilithe**, agus **comhlíonadh dlíthiúil**, féadfaidh SDKanna tríú páirtí amhail  
**Google Mobile Ads SDK (AdMob)** agus **Google UMP (User Messaging Platform)** sonraí áirithe a bhailiú agus a phróiseáil (m.sh., aitheantóirí fógraíochta).

---

## 2. Cineálacha sonraí a phróiseáiltear

### 2-1) Sonraí a stóráiltear ar do ghléas (stóráil áitiúil)

Stórálann an aip roinnt sonraí **go háitiúil ar do ghléas** chun gnéithe a sholáthar agus inúsáidteacht a fheabhsú.  
De ghnáth **ní sheoltar** na sonraí seo chuig freastalaithe an fhorbróra agus baintear iad nuair a ghlanann tú sonraí na haipe nó nuair a dhíshuiteálann tú í (seachas comhaid a onnmhairíonn tú in áit eile).

#### (1) Socruithe (SharedPreferences)

| Catagóir | Eochair (sampla) | Cuspóir | Stóráil | Scriosadh |
|---|---|---|---|---|
| Socrú críochnaithe | `setup_done` | Staid an tsocraithe tosaigh a stóráil | SharedPreferences | Bainte ar ghlanadh sonraí/díshuiteáil |
| Stair tíortha | `selected_countries` | Tíortha a roghnaíodh le déanaí a choinneáil | Mar an gcéanna | Mar an gcéanna |
| Tír ghníomhach | `active_country` | An tír roghnaithe reatha a stóráil | Mar an gcéanna | Mar an gcéanna |
| Cluichí roghnaithe | `selected_lotto_ids` | IDanna cluichí ticáilte a stóráil | Mar an gcéanna | Mar an gcéanna |
| Cluiche gníomhach | `active_lotto_id` | ID an chluiche ghníomhaigh a stóráil | Mar an gcéanna | Mar an gcéanna |
| **Roghnú ama síl (roghnach)** | `birth_datetime_iso` | Am tagartha síl roghnaithe ag an úsáideoir a stóráil (d’fhéadfadh sé a bheith in úsáid le haghaidh seed/personalization) | Mar an gcéanna | Mar an gcéanna |

> **Nóta:** Ní bhailítear “Roghnú ama síl (roghnach)” ach má roghnaíonn an t-úsáideoir é, agus b’fhéidir nach mbeidh sé riachtanach don phríomhúsáid.

#### (2) Sonraí loga (SQLite)

Féadfaidh an aip taifid ghinte/sábháilte a stóráil i mbunachar sonraí SQLite áitiúil.

- Sampla táblaí: `log_...`  
- Sampla réimsí:  
  - `id`, `date_id` nó `date_text` (stamp ama), `choice1..choiceN` (uimhreacha roghnaithe), `isFinger` (bratach a bhaineann le méarlorg, srl.)

Is féidir leat na logaí a fheiceáil sna scáileáin liosta/sonraí, agus iad a scriosadh (de réir tábla nó de réir ró) más mian leat.

#### (3) Comhaid JSON (de réir cluiche)

Féadfaidh an aip sonraí JSON in aghaidh an chluiche a stóráil i ndoiciméid na haipe.

- Sampla: `game_json/<gameId>.json`  
- Cuspóir: sonraí tarraingthe/torthaí in-eagarthóireachta ag an úsáideoir (m.sh., staitisticí/amléiriú)

Stóráiltear na comhaid seo ar an ngléas agus baintear iad go minic ar dhíshuiteáil, ag brath ar iompar OS/cúltaca.

---

### 2-2) Fógraí, toiliú agus sonraí gaolmhara (SDK tríú páirtí)

Úsáideann an aip **Google Mobile Ads SDK (AdMob)** agus **Google UMP** chun:

- Fógraí a thaispeáint (lena n-áirítear **fógraí luaíochta**)  
- Toiliú dlíthiúil riachtanach do fhógraíocht a bhainistiú

Féadfaidh na SDKanna seo, mar shampla, na sonraí seo a leanas a bhailiú/próiseáil:

- **Advertising ID** (m.sh., AAID, IDFA)  
- Eolas bunaithe ar IP, suíomh garbh, eolas líonra  
- Eolas gléis/aipe (leagan OS, leagan aipe, teanga, eolas diagnóiseach)  
- Idirghníomhaíochtaí fógraí (impressions, clicks, críochnú luaíochta)  
- Roghanna toilithe a thaifeadann UMP

I roinnt réigiún (m.sh., EEA/UK/CH), d’fhéadfadh foirm toilithe UMP a bheith le feiceáil agus d’fhéadfadh iontráil **Privacy Options** a bheith ar fáil nuair is gá.

---

## 3. Coinneáil (Retention)

- **Socruithe áitiúla (SharedPreferences):** coinnithe go dtí glanadh sonraí nó díshuiteáil  
- **Sonraí loga (SQLite):** coinnithe go dtí go scriosann tú iad nó go nglanann tú sonraí/díshuiteáil  
- **Comhaid JSON:** stóráilte i ndoiciméid na haipe; bainte go minic ar dhíshuiteáil, ach tá comhaid onnmhairithe/cúltaca faoi bhainistíocht an úsáideora  
- **Sonraí fógraí/toilithe (tríú páirtí):** de réir bheartais Google agus dlíthe is infheidhme

---

## 4. Roinnt tríú páirtí agus aistrithe idirnáisiúnta

Le haghaidh fógraí agus bainistíocht toilithe, féadfaidh roinnt sonraí a bheith próiseáilte ag **Google agus a chomhpháirtithe**.

| Mír | Sonraí |
|---|---|
| **Faighteoirí** | Google LLC, cleamhnaithe, agus fo-phróiseálaithe |
| **Ceann scríbe aistrithe** | Stáit Aontaithe agus réigiúin eile ina bhfuil bonneagar Google |
| **Cuspóir** | Seachadadh fógraí, tomhas, cosc calaoise, bainistíocht toilithe, comhlíonadh |
| **Sonraí** | Advertising ID, eolas bunaithe ar IP, eolas gléis/aipe, sonraí idirghníomhaíochta fógraí, stádas toilithe |
| **Coinneáil** | De réir bheartais Google agus dlí |
| **Tionchar má dhiúltaíonn tú** | D’fhéadfadh fógraí pearsantaithe a bheith teoranta; fógraí neamhphearsantaithe nó níos lú fógraí a bheith le feiceáil |

---

## 5. Do chearta agus conas iad a fheidhmiú

Ag brath ar an dlí is infheidhme, d’fhéadfadh cearta a bheith agat amhail rochtain, ceartú, scriosadh, srianadh, agóid, inaistritheacht, agus tarraingt siar toilithe (nuair is é an toiliú an bonn dlí).

Samplaí:

- **Roghanna fógraí/toilithe a choigeartú:** trí Privacy Options san aip (más ann) nó trí shocruithe fógraí an OS (Advertising ID a athshocrú, pearsantú a theorannú).  
- **Sonraí áitiúla a athshocrú:** glan sonraí na haipe nó díshuiteáil an aip.

---

## 6. Príobháideachas leanaí

**Ní dheartar** an aip seo **do leanaí**. Má úsáideann leanbh í, ba chóir do chaomhnóir rialuithe tuismitheora ar leibhéal OS agus roghanna teorannaithe fógraí a mheas.

---

## 7. Bearta slándála

Laistigh de raon na haipe, déanaimid ár ndícheall:

- Gan ach an t-íosmhéid riachtanach sonraí a stóráil go háitiúil  
- Próiseáil ar an ngléas a choinneáil nuair is féidir  
- TLS/iompar slán a úsáid do chumarsáid SDK (laistigh de chumais SDK)

---

## 8. Google Play Data safety

Má dháiltear ar Google Play, déanaimid iarracht nochtadh Data safety a choinneáil cruinn agus cothrom le dáta, go háirithe nuair a athraíonn SDKanna nó cleachtais phróiseála.

---

## 9. Fógraí open-source

Féadfaidh an aip leabharlanna open-source a úsáid do bhratacha tíre, stóráil, fógraí/toiliú, agus UI.  
Tá fógraí ceadúnais ar fáil i scáileán “Open-source licenses” na haipe (nó a chomhionann).

---

## 10. Teagmháil

Le haghaidh fiosruithe príobháideachais:

- **Ríomhphost:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Luaigh **“Power lucky lotto”** i do theachtaireacht.

---

## 11. Athruithe ar an bpolasaí seo

Féadfaidh an polasaí seo athrú mar gheall ar nuashonruithe dlí, athruithe gnéithe (m.sh., SDK nua), nó coigeartuithe beartais inmheánaigh.  
Foilseofar athruithe beaga san aip nó ar an leathanach seo; fógrófar athruithe ábhartha roimh ré mar a cheanglaítear.

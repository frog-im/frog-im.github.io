---
title: Politica da protecziun da datas | Lucky Pick Box
description: Lucky Pick Box Politica da protecziun da datas
lang: rm
last_updated: 2026-06-15
---

# Politica da confidenzialitad (Lucky Pick Box / 뽑기박스)

- **Num da l'app:** Lucky Pick Box / 뽑기박스
- **Sviluppader:** frog-im
- **Persuna responsabla per la protecziun da datas:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data d'entrada en vigur:** 2026-06-12
- **Ultima actualisaziun:** 2026-06-15

> Questa politica descriva co l'app tracta datas.  
> Sche i dat reglas obligatoricas en in pajais u regiun specifica, vegnan quellas applitgadas cun prioritad.

---

## 1. Intent e champ d'applicaziun

Lucky Pick Box è in utensil casual per elecziuns casualas, tratgas, elecziun da successiun, repartiziun d'equips, dats, munaidas, stgalas, rodas e gieus sumegliants per decisiuns dal mintgadi u da gruppa. L'app na porscha nagin gieu da fortuna cun daner real, naginas scumessas, transacziuns finanzialas, premis en daner u remuneraziuns equivalenta a daner.

### A. Funcziuns principalas

- Endataziun rapida: text scrit da l'utilisader u text legì d'in maletg tschernì.
- Gieus da tscherna casuala: ladder, wheel, plinko, simple draw, dice, coin, random number, team splitter, order picker, card, bomb e yes/no.
- Istorgia da resultats: tip da gieu, titel, participants/items, resumaziun dal resultat ed uras da creaziun pon vegnir memorisads.
- Slots da parameters: tscherts gieus pon memorisar participants, glistas, intervalls, quantitads, teams, pais e parameters sumegliants en fin 3 slots locals.

L'app na pretenda nagina registraziun u annunzia. Nus na manain nagin server che survegn da l'app tes num, numer da telefon, adressa dad e-mail, contacts, endataziuns da gieu, maletgs tschernids u resultats da gieu.

Per porscher las funcziuns po l'app memorisar endataziuns da gieu, etichettas da participants, resultats recents, parameters da gieu memorisads, parameters d'animaziun, tschernas da protecziun da datas per reclama e stadi collià cun consentiment en la memoria locala da tes apparat. L'istorgia dals resultats recents è limitada da l'app e na vegn betg tramessa ad in server dal sviluppader.

---

## 2. Tge datas vegnan tractadas

### 2-1) Datas endatadas da l'utilisader

L'app na pretenda nagina registraziun u annunzia. Nus na manain nagin server che survegn da l'app tes num, numer da telefon, adressa dad e-mail, contacts, endataziuns da gieu, maletgs tschernids u resultats da gieu.

### 2-2) Datotecas tschernidas sin il dispositiv

Sche ti tschernas da leger text ord in maletg, dumonda l'app da tscherner in maletg ord tia biblioteca da fotos. Il maletg tschernì vegn duvrà per renconuschientscha da text sin l'apparat tras il selectur da maletgs da la plattafurma e cumpunents Google ML Kit. Il sviluppader na chargia betg il maletg sin in agen server e na lochescha betg el en in conto lontan.

### 2-3) Datas localas da l'app

Per porscher las funcziuns po l'app memorisar endataziuns da gieu, etichettas da participants, resultats recents, parameters da gieu memorisads, parameters d'animaziun, tschernas da protecziun da datas per reclama e stadi collià cun consentiment en la memoria locala da tes apparat. L'istorgia dals resultats recents è limitada da l'app e na vegn betg tramessa ad in server dal sviluppader.

### B. Datas localas sin l'apparat

| Lieu u clav | Datas | Intent | Stizzar |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, tip da gieu, titel, participants/items, resumaziun, temp; fin 50 resultats recents. | Mussar resultats recents ed istorgia. | Stizzar en l'app, stizzar datas da l'app u deinstallar |
| `game_settings.<gameId>.slot_<n>` | Parameters da gieu, temp da memorisaziun, glistas, intervalls, quantitads, teams, pais; fin 3 slots. | Rechargiar parameters da gieu. | Svidar slot, stizzar datas u deinstallar |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Parameters d'animaziun e fullscreen. | Tegnair preferenzas da visualisaziun. | Midar parameters, stizzar datas u deinstallar |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Tschernas da privacy da reclama e dumber per frequenza da reclama. | Applitgar tschernas regiunalas e controllar frequenza. | Midar parameters, stizzar datas u deinstallar |
| Selectur da maletgs ed OCR | Via dal maletg tschernì e text renconuschì pon vegnir tractads temporarmain. | Agiuntar text da maletg a l'endataziun rapida. | Cache da l'app/OS u stizzar datas |

Text d'endataziun rapida na vegn betg tramess ad in server dal sviluppader. El po daventar data locala mo sch'el vegn duvrà en in resultat u parameter memorisà.

### 2-4) Datas automaticas per reclama/consentiment

Sin plattafurmas sustegnidas, actualmain Android, dovra l'app Google AdMob e Google User Messaging Platform (UMP). Google e partenaris da reclama pon tractar identificaturs da reclama, identificaturs d'instanza d'app, adressa IP, lieu approximativ, infurmaziuns d'apparat e rait, versiun da l'app, sistem operativ, lingua, impressiuns da reclama, clics ed interacziuns, diagnostica, stadi da consentiment e parameters regiunals da protecziun da datas da reclama per furnir reclama, limitar frequenza, impedir fraud, gestir consentiment, mesirar, analisar, segirar il servetsch e cumplir obligaziuns legalas.

Las praticas da protecziun da datas da Google èn descrittas a https://policies.google.com/privacy e https://policies.google.com/technologies/ads.

---

## 3. Intent da la tractaziun

Lucky Pick Box è in utensil casual per elecziuns casualas, tratgas, elecziun da successiun, repartiziun d'equips, dats, munaidas, stgalas, rodas e gieus sumegliants per decisiuns dal mintgadi u da gruppa. L'app na porscha nagin gieu da fortuna cun daner real, naginas scumessas, transacziuns finanzialas, premis en daner u remuneraziuns equivalenta a daner.

### A. Funcziuns principalas

- Endataziun rapida: text scrit da l'utilisader u text legì d'in maletg tschernì.
- Gieus da tscherna casuala: ladder, wheel, plinko, simple draw, dice, coin, random number, team splitter, order picker, card, bomb e yes/no.
- Istorgia da resultats: tip da gieu, titel, participants/items, resumaziun dal resultat ed uras da creaziun pon vegnir memorisads.
- Slots da parameters: tscherts gieus pon memorisar participants, glistas, intervalls, quantitads, teams, pais e parameters sumegliants en fin 3 slots locals.

Sin plattafurmas sustegnidas, actualmain Android, dovra l'app Google AdMob e Google User Messaging Platform (UMP). Google e partenaris da reclama pon tractar identificaturs da reclama, identificaturs d'instanza d'app, adressa IP, lieu approximativ, infurmaziuns d'apparat e rait, versiun da l'app, sistem operativ, lingua, impressiuns da reclama, clics ed interacziuns, diagnostica, stadi da consentiment e parameters regiunals da protecziun da datas da reclama per furnir reclama, limitar frequenza, impedir fraud, gestir consentiment, mesirar, analisar, segirar il servetsch e cumplir obligaziuns legalas.

Las praticas da protecziun da datas da Google èn descrittas a https://policies.google.com/privacy e https://policies.google.com/technologies/ads.

---

## 4. Durada da conservaziun

L'istorgia locala e parameters pon restar sin tes apparat fin che ti stizzas l'istorgia, stizzas las datas da l'app u deinstalleschas l'app. Ti pos midar las tschernas disponiblas da protecziun da datas da reclama en ils parameters da l'app, avrir las opziuns da privacy da Google sche necessari, e gestir u resetar identificaturs da reclama en ils parameters da privacy da l'apparat. La retenziun d'infurmaziuns tractadas da Google vegn reglada da las politicas e obligaziuns legalas da Google.

### B. Datas localas sin l'apparat

| Lieu u clav | Datas | Intent | Stizzar |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, tip da gieu, titel, participants/items, resumaziun, temp; fin 50 resultats recents. | Mussar resultats recents ed istorgia. | Stizzar en l'app, stizzar datas da l'app u deinstallar |
| `game_settings.<gameId>.slot_<n>` | Parameters da gieu, temp da memorisaziun, glistas, intervalls, quantitads, teams, pais; fin 3 slots. | Rechargiar parameters da gieu. | Svidar slot, stizzar datas u deinstallar |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Parameters d'animaziun e fullscreen. | Tegnair preferenzas da visualisaziun. | Midar parameters, stizzar datas u deinstallar |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Tschernas da privacy da reclama e dumber per frequenza da reclama. | Applitgar tschernas regiunalas e controllar frequenza. | Midar parameters, stizzar datas u deinstallar |
| Selectur da maletgs ed OCR | Via dal maletg tschernì e text renconuschì pon vegnir tractads temporarmain. | Agiuntar text da maletg a l'endataziun rapida. | Cache da l'app/OS u stizzar datas |

Text d'endataziun rapida na vegn betg tramess ad in server dal sviluppader. El po daventar data locala mo sch'el vegn duvrà en in resultat u parameter memorisà.

---

## 5. Stizzada da datas

L'istorgia locala e parameters pon restar sin tes apparat fin che ti stizzas l'istorgia, stizzas las datas da l'app u deinstalleschas l'app. Ti pos midar las tschernas disponiblas da protecziun da datas da reclama en ils parameters da l'app, avrir las opziuns da privacy da Google sche necessari, e gestir u resetar identificaturs da reclama en ils parameters da privacy da l'apparat. La retenziun d'infurmaziuns tractadas da Google vegn reglada da las politicas e obligaziuns legalas da Google.

### C. Permissiuns, SDKs, backups e segirezza

L'app po duvrar `INTERNET`, `ACCESS_NETWORK_STATE` e `com.google.android.gms.permission.AD_ID` per reclama ed avis legals. Access a fotos u selectur da maletgs vegn duvrà mo cura che l'utilisader tscherna da leger text d'in maletg.

Google Mobile Ads SDK po tractar adressa IP, interacziuns da reclama, diagnostica ed identificaturs d'apparat/conto per reclama, analitica e prevenziun da fraud. UMP po tractar stadi da consentiment e tschernas da privacy.

Datas localas pon vegnir stizzadas tras funcziuns da l'app, stizzar datas da l'app en l'OS u deinstallaziun. Backups dal sistem, screenshots u datotecas partagidas pon restar tenor politicas dal furnitur. Evitai datas sensiblas en champs da text liber.

---

## 6. Terzas partidas e transferiment transfrontalier

Nus na vendain betg tias endataziuns da gieu, etichettas da participants, resultats da gieu u maletgs tschernids. Cura che funcziuns da reclama u consentiment vegnan dumandadas, pon Google LLC, affiliads da Google e lur furniturs da servetschs tractar infurmaziuns da reclama e consentiment en pajais ordaifer tes pajais u tia regiun. Guarda "Infurmaziun davart la transmissiun internaziunala da datas" en l'app per dapli detagls.

| Element | Detagls |
|---|---|
| **Destinatari** | Google LLC e sias affiliadas |
| **Pajais da transferiment** | Stadis Unids e regiuns cun infrastructura Google |
| **Intent** | reclama, mesiraziun, consentiment, prevenziun d'abus, conformitad |
| **Datas (exempels)** | AAID/IDFA, IP/rait, datas dal dispositiv/app, interacziun cun reclama, status da consentiment |
| **Durada** | tenor politica da Google e reglas legalas |
| **Effect en cas da refusa** | reclama persunalisada limitada; reclama betg persunalisada u restricziuns da funcziuns da reclama |

---

## 7. Permissiuns duvradas

### C. Permissiuns, SDKs, backups e segirezza

L'app po duvrar `INTERNET`, `ACCESS_NETWORK_STATE` e `com.google.android.gms.permission.AD_ID` per reclama ed avis legals. Access a fotos u selectur da maletgs vegn duvrà mo cura che l'utilisader tscherna da leger text d'in maletg.

Google Mobile Ads SDK po tractar adressa IP, interacziuns da reclama, diagnostica ed identificaturs d'apparat/conto per reclama, analitica e prevenziun da fraud. UMP po tractar stadi da consentiment e tschernas da privacy.

Datas localas pon vegnir stizzadas tras funcziuns da l'app, stizzar datas da l'app en l'OS u deinstallaziun. Backups dal sistem, screenshots u datotecas partagidas pon restar tenor politicas dal furnitur. Evitai datas sensiblas en champs da text liber.

---

## 8. Installaziun, funcziunament e refus dals mecanissems da rimnada automatica

Sin plattafurmas sustegnidas, actualmain Android, dovra l'app Google AdMob e Google User Messaging Platform (UMP). Google e partenaris da reclama pon tractar identificaturs da reclama, identificaturs d'instanza d'app, adressa IP, lieu approximativ, infurmaziuns d'apparat e rait, versiun da l'app, sistem operativ, lingua, impressiuns da reclama, clics ed interacziuns, diagnostica, stadi da consentiment e parameters regiunals da protecziun da datas da reclama per furnir reclama, limitar frequenza, impedir fraud, gestir consentiment, mesirar, analisar, segirar il servetsch e cumplir obligaziuns legalas.

Las praticas da protecziun da datas da Google èn descrittas a https://policies.google.com/privacy e https://policies.google.com/technologies/ads.

L'istorgia locala e parameters pon restar sin tes apparat fin che ti stizzas l'istorgia, stizzas las datas da l'app u deinstalleschas l'app. Ti pos midar las tschernas disponiblas da protecziun da datas da reclama en ils parameters da l'app, avrir las opziuns da privacy da Google sche necessari, e gestir u resetar identificaturs da reclama en ils parameters da privacy da l'apparat. La retenziun d'infurmaziuns tractadas da Google vegn reglada da las politicas e obligaziuns legalas da Google.

---

## 9. Dretgs da l'utilisader

L'istorgia locala e parameters pon restar sin tes apparat fin che ti stizzas l'istorgia, stizzas las datas da l'app u deinstalleschas l'app. Ti pos midar las tschernas disponiblas da protecziun da datas da reclama en ils parameters da l'app, avrir las opziuns da privacy da Google sche necessari, e gestir u resetar identificaturs da reclama en ils parameters da privacy da l'apparat. La retenziun d'infurmaziuns tractadas da Google vegn reglada da las politicas e obligaziuns legalas da Google.

---

## 10. Mesiras da segirezza

### C. Permissiuns, SDKs, backups e segirezza

L'app po duvrar `INTERNET`, `ACCESS_NETWORK_STATE` e `com.google.android.gms.permission.AD_ID` per reclama ed avis legals. Access a fotos u selectur da maletgs vegn duvrà mo cura che l'utilisader tscherna da leger text d'in maletg.

Google Mobile Ads SDK po tractar adressa IP, interacziuns da reclama, diagnostica ed identificaturs d'apparat/conto per reclama, analitica e prevenziun da fraud. UMP po tractar stadi da consentiment e tschernas da privacy.

Datas localas pon vegnir stizzadas tras funcziuns da l'app, stizzar datas da l'app en l'OS u deinstallaziun. Backups dal sistem, screenshots u datotecas partagidas pon restar tenor politicas dal furnitur. Evitai datas sensiblas en champs da text liber.

### C. Permissiuns, SDKs, backups e segirezza

L'app po duvrar `INTERNET`, `ACCESS_NETWORK_STATE` e `com.google.android.gms.permission.AD_ID` per reclama ed avis legals. Access a fotos u selectur da maletgs vegn duvrà mo cura che l'utilisader tscherna da leger text d'in maletg.

Google Mobile Ads SDK po tractar adressa IP, interacziuns da reclama, diagnostica ed identificaturs d'apparat/conto per reclama, analitica e prevenziun da fraud. UMP po tractar stadi da consentiment e tschernas da privacy.

Datas localas pon vegnir stizzadas tras funcziuns da l'app, stizzar datas da l'app en l'OS u deinstallaziun. Backups dal sistem, screenshots u datotecas partagidas pon restar tenor politicas dal furnitur. Evitai datas sensiblas en champs da text liber.

---

## 11. Datas sensiblas

L'app na pretenda betg datas sensiblas. Ils utilisaders duain evitar d'endatar infurmaziuns fitg sensiblas en champs libers.

---


## 12. Protecziun d'uffants

L'app n'è betg concepida principalmain per uffants.

---


## 13. Decisiuns automatisadas

L'app na fa naginas decisiuns automatisadas cun effect legal u equivalent.

---


## 14. Avis da Data Safety (stores)

Il sviluppader emprova da mantegnair actualisads ils avis da "Data safety" en stores (p.ex. Google Play) tenor il cumportament real da l'app e dals SDKs.

---


## 15. Open source

L'app po duvrar bibliotecas open source. Licenzas vegnan publitgadas en la zona da licenzas da l'app u en ils meds da distribuziun.

---


## 16. Contact

- **Persuna responsabla:** frog-im
- **E-mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---


## 17. Midadas da la politica

Questa politica po vegnir midada per motivs legals, tecnics u da servetsch. Midada impurtanta vegn communitgada tras l'app u la pagina da politica.

Ultima actualisaziun: **2026-06-15**

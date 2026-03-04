---
title: Politica da confidenzialitad | know_me
description: know_me (PeopleNote, Memory for People) Politica da confidenzialitad (Rumantsch)
lang: rm
last_updated: 2026-03-04
---

# Politica da confidenzialitad (know_me / PeopleNote, Memory for People)

- **Num da l'app:** know_me (PeopleNote, Memory for People)
- **Sviluppader:** frog-im
- **Persuna responsabla per la protecziun da datas:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data d'entrada en vigur:** 2026-03-04
- **Ultima actualisaziun:** 2026-03-04

> Questa politica descriva co l'app tracta datas.  
> Sche i dat reglas obligatoricas en in pajais u regiun specifica, vegnan quellas applitgadas cun prioritad.

---

## 1. Intent e champ d'applicaziun

`know_me` gida persunas a registrar e manischar infurmaziuns davart persunas, incl. backup/restauraziun e export PDF.

Funcziuns principalas:

- registrar infurmaziuns da persunas (num, text d'identificaziun, notas, tendenza, pajais, schlattaina, contact)
- urdenar en dossiers, tschertgar e fusiunar
- agiuntar fotos e descriziuns
- exportar/importar backup (`.knm`)
- exportar PDF
- serrar l'app (pled-clav / pattern)
- administraziun da reclama e consentiment (AdMob/UMP)

L'app na pretenda nagin conto separat. Las datas principalas vegnan memorisadas localmain sin il dispositiv.

---

## 2. Tge datas vegnan tractadas

### 2-1) Datas endatadas da l'utilisader

- num
- text d'identificaziun
- notas
- tendenza, pajais, schlattaina
- numer da telefon
- temp da cumparsa / sentupada
- infurmaziuns da plattafurmas/sites
- num e colur da dossier
- descriziun da fotografia (caption)

### 2-2) Datotecas tschernidas sin il dispositiv

- fotografias tschernidas da l'utilisader
- datotecas backup `.knm` tschernidas per import
- lieu da memorisaziun tschernì per export PDF/backup

### 2-3) Datas localas da l'app

- SQLite DB (`people_note.db`): persunas/dossiers/plattafurmas/sites/metadata da fotos
- fotografias criptadas (`.enc`) en il dossier intern da documents da l'app
- parameters (`SharedPreferences`): tema, urden, opziuns da privacy/reclama, opziuns PDF, politica da serrada
- datas da serrada: hash + salt per pled-clav/pattern
- clav da criptaziun locala en `flutter_secure_storage`
- datotecas temporaras per previsualisaziun e process d'import/export

### 2-4) Datas automaticas per reclama/consentiment

Cur che reclama u consentiment èn activads, SDKs da Google/partenaris pon tractar:

- identifitgaders da reclama (AAID/IDFA)
- IP e datas da rait
- datas dal dispositiv/app (versiun OS, model, versiun app)
- interacziun cun reclama (visualisaziuns, clics)
- status da consentiment e tschernas da privacy

Las datas principalas da persunas na vegnan generalmain betg chargiadas sin in server dal sviluppader.

---

## 3. Intent da la tractaziun

- registrar e tschertgar infurmaziuns da persunas
- urdenar cun dossiers/tschertga/fusiun
- mussar e manischar fotos
- exequir backup/restauraziun/export PDF
- furnir funcziun da serrada
- reclama, administraziun da consentiment, prevenziun d'abus e conformitad legala

---

## 4. Durada da conservaziun

- datas localas internas: fin a stizzada da l'app u da las datas da l'app
- datotecas temporaras: stizzadas suenter l'operaziun u tenor politica da cache dal sistem
- PDFs/backup exportads: restan en il lieu tschernì da l'utilisader fin che l'utilisader stizza quellas
- datas da reclama/consentiment (terzas partidas): tenor politica da Google e reglas legalas

---

## 5. Stizzada da datas

- stizzada directa en l'app (persunas, dossiers, fotos, etc.)
- stizzada da datas da l'app tras il sistem operativ
- stizzada da valurs en `SharedPreferences` e `flutter_secure_storage`
- stizzada da datotecas internas (inclus temp)
- datotecas externas exportadas ston vegnir stizzadas da l'utilisader

---

## 6. Terzas partidas e transferiment transfrontalier

Per reclama/consentiment po l'app duvrar Google (AdMob/UMP).

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

- `INTERNET`: communicaziun da rait (incl. SDKs da reclama)
- `com.google.android.gms.permission.AD_ID`: identifitgader da reclama
- `READ_MEDIA_IMAGES` (Android 13+) / `READ_EXTERNAL_STORAGE` (Android 12 e pli vegl): tscherna da fotos

Permissiuns vegnan duvradas mo en il rom necessari.

---

## 8. Dretgs da l'utilisader

Tenor leschas applitgablas:

- dretg d'access, correctura e stizzada
- dretg da limitar tractaziun
- dretg da retrair consentiment

Co exercitar:

- midar/stizzar datas directamain en l'app
- stizzar datas da l'app u disinstallar l'app
- midar tschernas da consentiment/privacy en l'app (sche disponibel)
- midar settings da reclama en il sistem operativ
- contact: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 9. Mesiras da segirezza

- memorisaziun locala da datas
- criptaziun da fotografias (AES-GCM)
- hash da datas da serrada (nagin text plain)
- backup criptà cun pled-clav da l'utilisader
- transmissiun criptada (HTTPS/TLS) per communicaziun cun terzas partidas

---

## 10. Datas sensiblas

L'app na pretenda betg datas sensiblas. Ils utilisaders duain evitar d'endatar infurmaziuns fitg sensiblas en champs libers.

---

## 11. Protecziun d'uffants

L'app n'è betg concepida principalmain per uffants.

---

## 12. Decisiuns automatisadas

L'app na fa naginas decisiuns automatisadas cun effect legal u equivalent.

---

## 13. Avis da Data Safety (stores)

Il sviluppader emprova da mantegnair actualisads ils avis da "Data safety" en stores (p.ex. Google Play) tenor il cumportament real da l'app e dals SDKs.

---

## 14. Open source

L'app po duvrar bibliotecas open source. Licenzas vegnan publitgadas en la zona da licenzas da l'app u en ils meds da distribuziun.

---

## 15. Contact

- **Persuna responsabla:** frog-im
- **E-mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 16. Midadas da la politica

Questa politica po vegnir midada per motivs legals, tecnics u da servetsch. Midada impurtanta vegn communitgada tras l'app u la pagina da politica.

Ultima actualisaziun: **2026-03-04**

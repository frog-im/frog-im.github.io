---
title: Politica da protecziun da datas | LyriFloat
description: Politica da protecziun da datas da LyriFloat (Rumantsch)
lang: rm
last_updated: 2025-10-30
---

# Politica da protecziun da datas (LyriFloat)

- **Num da l’app:** LyriFloat  
- **Sviluppader:** frog-im  
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data d’entrada en vigur:** 2025-10-30

> Questa politica è redigida cun referenza a las novitadsaziuns giuridicas applicablas, tranter auter la Korean Personal Information Protection Act (PIPA), il GDPR/UK GDPR, la Swiss FADP edaziunsaziuns relevantas dals stadis dals Stadis Unids. Sche i dat pretensiuns specificas d’ina giurisdicziun, han quellas prioritad.

---

## 1. Intent e champ d’applicaziun

Questa app porscha **l’ediziun da metadata da files audio** (titgel, artist, etc.) ch’èn memorisads sin il dispositiv e funcziuns da **lyrics overlay**.  
L’app **na crea nagin** conto d’utilisader e **na chargia nagut si** dal cuntegn da l’utilisader sin in server. Il tractament succeda **sin il dispositiv da l’utilisader** sco standard.

Tuttina, per motivs da **publicitad** e da **confurmitad legala**, pon partenaris da terza vart (p.ex. Google Mobile Ads SDK (AdMob), UMP) rimnar e tractar infurmaziuns sco **identificaders da reclama**. La rimnada da consentiment e las tschernas da privacy suondan las specificaziuns da **Google UMP (User Messaging Platform)**.

---

## 2. Categorias d’infurmaziuns che nus tractain

### 2-1) Files tschernids explicitamain da l’utilisader
- **Percurs e cuntegn da files audio/immaginas da cover:** tractads **localmain** sin il dispositiv mo per editar e salvar.  
- **FFmpegKit** vegn utilisà localmain per encoding, ediziun da metadata e l’extracziun da thumbnails.  
- L’app **na chargia betg si** ils files tschernids da l’utilisader sin noss servers.

### 2-2) Parameters locals e valurs memorisadas

Per la funcziunalitad fundamentala e la cumadaivladad, memorisescha l’app las valurs suandantas **localmain sin il dispositiv**.  
Questas valurs na vegnan betg tramessas a noss servers e vegnan **allontanadas** cura che l’app u ses datas vegnan stizzadas.

#### (1) Preferenzas (`shared_preferences`)
| Tip | Clav/Cuntegn | Intent | Memorisaziun | Stizzar |
|---|---|---|---|---|
| Posiziun/font da l’overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restaurar la posiziun da l’overlay e la grondezza dal font | Device SharedPreferences | Stizzà cura che datas da l’app u l’app vegnan stizzadas |
| Settings Ads/Privacy | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Reclama betg persunalisada, RDP US, tag COPPA, tag da vegliadetgna, limita da rating da reclama | Device SharedPreferences | Sco a sanestra |

#### (2) Files temporars (directori temp dal sistem)
- **Exempels:** `cover_*.jpg`, `tmp_*.flac`  
- **Utilisaziun:** extrar cover art, tagging FLAC, encoding temporar  
- **Lieu:** dossier temporar dal OS (`systemTemp`)  
- **Durada:** l’app emprova da stizzar suenter la terminaziun, sche pussaivel; er sutmettà a la pulizia automatica dal OS

#### (3) Salvament tschernì da l’utilisader (SAF)
- Cura che l’utilisader tscherna “Save As”, pon ils files audio finals vegnir scrits en lieus tschernids (p.ex. Downloads, cloud).  
- Quests files stattan en **stoccadi extern** e **restan** er suenter che l’app è stizzada. L’utilisader po els stizzar manualmain.

#### (4) Stadi da consentiment (UMP SDK Cache)
- En regiuns EEA/UK/CH **memorischa (cache)** la UMP SDK il stadi da consentiment da reclama localmain.  
- Quel po vegnir resettà cun stizzar las datas da l’app u via il scherm **Privacy Options** en l’app (sche disponibel).

---

### 2-3) Datas da reclama e consentiment (SDKs da terza vart)
- **Google Mobile Ads SDK (AdMob) e UMP** pon rimnar/tratar, per exempel: **identificaders da reclama (AAID/IDFA)**, **IP ranges**, **infos dal dispositiv e da l’app**, **signals d’interacziun cun reclama**, **stadi da consentiment**, etc.  
- **Intents:** furniziun da reclama, frequency capping, prevenziun da fraud, mesiraziun da prestaziun, confurmitad legala  
- **Regiuns che pretendan consentiment (EEA/UK/CH):** consentiment vegn rimnà via UMP prompts, e vegnir mess a disposiziun in scherm **Privacy Options** cura ch’i è necessari.  
  En regiuns senza tala obligaziun (p.ex. KR), la funcziun **po betg vegnir mussada**.

---

## 3. Tractament e durada da conservaziun

- **Settings locals:** memorisads sin il dispositiv fin che l’utilisader stizza las datas da l’app u deinstallescha l’app  
- **Files temporars:** creats durant encoding/extracziun, stizzads suenter il tractament u eventualmain temporarmain en caches dal OS  
- **Datas Ads/consentiment (terza vart):** conservadas e stizzadas tenor **politicas da Google**

---

## 4. Transfers a terzas varts e transfers transfruntaliers

Per reclama e consent management pon infurmaziuns da l’utilisader vegnir tramessas e tractadas sin l’infrastructura da Google.

| Element | Detagls |
|---|---|
| **Recipient** | Google LLC e ses affiliates/sub-processors |
| **Destinaziun** | Stadis Unids (e autras regiuns nua che l’infrastructura da Google è situada) |
| **Intent** | Furniziun da reclama, prestaziun/mesiraziun, confurmitad legala, consent management |
| **Datas** | Identificaders da reclama, IP ranges, infos dal dispositiv e da l’app, interacziuns cun reclama, stadi da consentiment, etc. |
| **Conservaziun** | Tenor politicas da Google |
| **Effect da refusa** | Reclama persunalisada po vegnir limitada; reclama betg persunalisada po vegnir mussada |

Nus respechain las pretensiuns da publicaziun da **Google Play Data safety** e tegnain las decleraziuns en accord cun il tractament real.

---

## 5. Voss dretgs e co els exercitar

- **Opt-out da reclama persunalisada / midar consentiment**  
  - En regiuns sustegnidas (EEA/UK/CH): midar las preferenzas en **Settings → Privacy Options**.  
  - En autras regiuns: duvrar las settings dal OS per **resettar ad IDs / limitar ad tracking**.
- **Reset da datas localas:** stizzar las datas da l’app u deinstallar l’app resetta las coordinatas da l’overlay, la grondezza dal font e settings locals.
- Dretgs sut **GDPR/UK GDPR/Swiss FADP/leschas da privacy dals stadis US** (access, rectificaziun, stizzar, portability, restricziun, retratga dal consentiment, etc.) pon vegnir exercitads tenor las leschas respectivas.  
  Per datas da reclama tractadas da Google, duvrar per plaschair **las proceduras da Google**.

---

## 6. Protecziun da persunas minorennas

Questa app **na sa drizza betg** a persunas minorennas. Sche in uffant sut la vegliadetgna minima legala utilisescha l’app, duai el chalar e duvrar funcziuns dal OS per limitar reclama cun l’agid d’in guardian. Cura ch’i è adattà, pudain nus applitgar **TFUA (child-directed tag)** u opziuns sumegliantas da protecziun.

---

## 7. Mesiras da segirezza

- **Minimizaziun da datas** tar rimnada e memorisaziun  
- Utilisaziun **limitada** da files temporars e tentativas da stizzar suenter il tractament  
- Tractament strictamain **en il champ da permissiun dal OS**  
- **TLS u equivalent** per criptaziun durant la transmissiun tar transfers a terzas varts (tenor standards da SDK)

---

## 8. Data Safety (Google Play)

Nus preparain e mantegnin la secziun **Data safety** en il Play Console correctamain e l’actualisain svelt cura che i dat midadas.

---

## 9. Avisas open-source

L’app utilisescha software open-source sco **FFmpeg**. In file d’infurmaziun (p.ex. `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) en l’app declera co obtegnair il source code. Sin dumonda furnin nus la funtauna sco inditgà en quel file.

---

## 10. Contact

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Midadas da questa politica

Nus pudain reveder questa politica per motivs legals u da midadas dal servetsch. Nus publitgain novitadsaziunsaziuns **en l’app** ed sin questa **pagina da politica**.  
Per midadas materialas dain nus in avis d’almain **7 dis** avant la data d’entrada en vigur.

---

## Appendix: Guidanza per l’utilisader

- **Link en l’app:** avrir questa pagina via **Settings → Privacy**.  
- **Cumportament regiunal:** en EEA/UK/CH vegnan mussadas Privacy Options. **En KR e tschertas autras regiuns, il buttun po betg mussar ulteriuras opziuns** sch’i na vegnan betg pretendidas legalmain.

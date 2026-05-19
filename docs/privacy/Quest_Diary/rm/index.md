---
title: Decleraziun davart la protecziun da datas | QDiary
description: Decleraziun davart la protecziun da datas da QDiary
---

# Decleraziun davart la protecziun da datas (QDiary)

- Num da l'app: QDiary
- Sviluppader: frog-im
- Contact: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Data d'entrada en vigur: 2026-04-19
- Ultima actualisaziun: 2026-04-19

Questa decleraziun davart la protecziun da datas è redigida sin basa da l'implementaziun actuala da l'app QDiary. QDiary porscha novitadsziuns per scriver in diari, generar e reflectar quests, s'annunziar, memorisar manualmain en il cloud, mussar novitadsziuns publicitaras ed novitadsziuns. En quest connex po l'app elavurar datas persunalas u novitadsziuns che pudessan vegnir consideradas sco datas persunalas, uschè lunsch sco quai è necessari.

## 1. Funcziuns purschidas

QDiary porscha las suandantas funcziuns:

- scriver, modifitgar e consultar diaris
- classificaziun tenor categorias e vista da chalender
- generaziun da quests, reflexiun davart quests e tractament da la terminaziun da quests
- blocada locala da l'app da diari e criptaziun locala
- annunzia cun e-mail, verificaziun da l'e-mail, annunzia anonima (giast) e redefiniziun dal pled-clav
- memorisaziun e chargiada en il cloud iniziadas da l'utilisader
- visualisaziun da novitadsziuns publicitaras e tractament da las opziuns da privacy da novitadsziuns publicitaras
- novitadsziuns da regurdientscha per quests

## 2. Categorias da novitadsziuns elavuradas

### 2-1. Novitadsziuns endatadas directamain da l'utilisader

- adressa dad e-mail
- pled-clav
- titel dal diari, cuntegn, data, categoria e grad da difficultad
- novitadsziuns da risposta als quests, cuntegn da reflexiun e novitadsziuns davart il quest tschernì
- selecziuns che pertutgan il profil dal quest e text da resumaziun
- frasa da pass per blocar l'app da diari

### 2-2. Novitadsziuns memorisadas da l'app sin il device

- banca da datas locala dal diari (SQLite)
- novitadsziuns davart il status dals quests per diaris locals
- novitadsziuns da status areguard preschientscha, parameters, lingua, novitadsziuns e novitadsziuns publicitaras
- novitadsziuns da verificaziun da la blocada da l'app, salt e metadatas da criptaziun
- novitadsziuns davart la planisaziun da novitadsziuns da quests

### 2-3. Novitadsziuns davart il conto e l'identificaziun

Las suandantas novitadsziuns pon vegnir elavuradas tras Firebase Authentication:

- Firebase UID
- adressa dad e-mail
- sche la verificaziun da l'e-mail è vegnida terminada
- sche l'annunzia anonima vegn duvrada

### 2-4. Novitadsziuns davart novitadsziuns publicitaras e consentiment

Cura che Google AdMob ed il UMP SDK vegnan duvrads, pon vegnir elavuradas las suandantas novitadsziuns:

- identificaturs publicitaris (sco Android AD_ID)
- adressa IP e novitadsziuns da rait
- novitadsziuns dal device, versiun dal sistem operativ e novitadsziuns da l'app
- novitadsziuns davart impressiuns publicitaras, clics e tractament da recumpensas
- status dal consentiment publicitar e status da las opziuns da privacy

### 2-5. Novitadsziuns colliadas cun novitadsziuns

- sche la permissiun per novitadsziuns è vegnida dada
- novitadsziuns d'identificaziun per diaris che cuntegnan quests actuals
- text da novitadsziuns da quests
- uras planisadas da novitadsziuns

## 3. Finamiras da l'elavuraziun

L'app elavura novitadsziuns per las suandantas finamiras:

- registraziun, annunzia, verificaziun da l'e-mail e redefiniziun dal pled-clav
- scriver, memorisar e consultar diaris
- generaziun da quests, reflexiun e determinaziun da terminaziun
- criptaziun e decriptaziun locala colliadas cun la blocada da l'app
- memorisaziun e chargiada en il cloud pretendidas da l'utilisader
- furniziun da novitadsziuns da quests
- furniziun da novitadsziuns publicitaras, tractament da recumpensas publicitaras e resguardar il status dal consentiment publicitar
- segirezza, tractament d'errurs e funcziunament dal servetsch

## 4. Arcunaziun locala, arcunaziun en il cloud ed elavuraziun externa

### 4-1. Arcunaziun locala

Las novitadsziuns davart diaris e quests vegnan principalmain arcunadas en la banca da datas locala dal device.

- sche la blocada da l'app n'è betg activa: novitadsziuns vegnan arcunadas localmain en furma generala
- sche la blocada da l'app è activa: tschertas novitadsziuns, sco il titel dal diari, il cuntegn ed il status dal quest, pon vegnir criptadas ed arcunadas localmain

### 4-2. Arcunaziun en il cloud

L'app arcunescha novitadsziuns en Firebase Firestore mo cura che l'utilisader exequescha directamain la funcziun `Save`.

Tenor la configuraziun actuala dal project:

- i na vegn betg duvrà in sync cumplet automatic
- novitadsziuns vegnan arcunadas en Firestore `savedDiaries` mo cura che l'utilisader las memorisescha manualmain
- cura che novitadsziuns vegnan memorisadas, pon il titel dal diari, il cuntegn ed il status dal quest vegnir arcunads en furma criptada, tenor il status actual da la blocada da l'app
- novitadsziuns vegnan chargiadas enavos en la memoria locala mo cura che l'utilisader exequescha `Load`

### 4-3. Elavuraziun externa per generaziun e reflexiun da quests

Cura che l'utilisader pretenda la generaziun d'in quest u ina reflexiun, pon las suandantas novitadsziuns vegnir duvradas per elavuraziun externa tras Firebase Functions:

- titel dal diari
- cuntegn dal diari u cuntegn da la reflexiun
- categoria
- difficultad
- quest tschernì
- novitadsziuns resumadas dal profil dal quest

Questas novitadsziuns vegnan duvradas per generar e valitar quests tras l'API d'OpenAI.

Impurtant:

- il cuntegn relevant dal diari vegn duvrà per elavuraziun externa mo cura che la funcziun da quest vegn duvrada
- tenor la configuraziun actuala dal project na vegn nagin code duvrà che arcunescha logs da quests en ina collecziun separada `questLogs`

## 5. Servetschs da terzas varts ed elavuraziun externalisada

### 5-1. Google Firebase

Intent:

- autentificaziun (Firebase Authentication)
- arcunaziun en Firestore
- exequziun da Cloud Functions

Novitadsziuns che pon vegnir elavuradas:

- UID, adressa dad e-mail e status d'autentificaziun
- datas dal diari memorisadas manualmain da l'utilisader
- datas da dumondas da quests

### 5-2. OpenAI

Intent:

- generaziun da quests
- reflexiun davart quests e valitaziun da terminaziun

Novitadsziuns che pon vegnir elavuradas:

- titel/cuntegn dal diari
- text dal quest
- difficultad e categoria
- cuntegn da reflexiun endatà da l'utilisader
- novitadsziuns resumadas dal profil dal quest

### 5-3. Google AdMob / UMP

Intent:

- furnir novitadsziuns publicitaras da banner, interstitial e rewarded
- tractar il consentiment publicitar e las opziuns da privacy

Novitadsziuns che pon vegnir elavuradas:

- identificaturs publicitaris
- novitadsziuns dal device e da la rait
- novitadsziuns d'interacziun cun novitadsziuns publicitaras
- status dal consentiment

## 6. Avis davart transfer internaziunal

L'app po elavurar datas persunalas u novitadsziuns colliadas ordaifer il pajais da l'utilisader en ils suandants cas:

| Element | Detagls |
|---|---|
| Destinatari | Google LLC, OpenAI ed operaturs d'infrastructura colliads |
| Pajais da destinaziun | Stadis Unids, e.u.v. |
| Mument dal transfer | Durant l'annunzia, generaziun/reflexiun da quests, dumondas da novitadsziuns publicitaras e tractament dal consentiment |
| Moda dal transfer | communicaziun da rait criptada |
| Intent dal transfer | autentificaziun, arcunaziun da datas, elavuraziun serverless, generaziun/valitaziun da quests cun IA e novitadsziuns publicitaras |

## 7. Durada d'arcunaziun e d'utilisaziun

L'app arcunescha novitadsziuns tenor ils suandants standards:

- novitadsziuns localas dal diari/dals parameters: fin che l'utilisader las stizza u deinstallescha l'app
- novitadsziuns dal conto Firebase: uschè ditg sco l'utilisader mantegna il conto
- datas arcunadas en Firestore: uschè ditg sco l'utilisader mantegna ils elements memorisads
- datas da tractament da dumondas da quests: a la mesira necessaria per l'elavuraziun serverless
- datas colliadas cun novitadsziuns publicitaras/consentiment: tenor la politica da mintga purschider extern

Ultra da quai cuntegna il project actual la suandanta logica da nettegiar automaticamain:

- nettegiar contos d'utilisaders anonims e datas Firestore da subcollecziuns d'utilisader suenter in tschert temp
- nettegiar contos d'utilisaders regulars inactivs da ditg e datas Firestore da subcollecziuns d'utilisader

Sche quai vegn dentant effectivamain reflectà en l'ambient da producziun po variar tenor il status da deploy ed ils parameters dal server.

## 8. Avis davart la blocada da l'app e la criptaziun locala

L'app porscha ina funcziun separada `Diary App Lock`.

- la frasa da pass da la blocada da l'app è separada dal pled-clav dal conto
- la frasa da pass da la blocada da l'app vegn duvrada per la criptaziun e decriptaziun locala dal diari
- er sche vegn endatada ina frasa da pass incorrecta, po l'app sezza betg adina vegnir bloccada cumplettamain; empè da quai po ina part dal cuntegn dal diari restar illegibla
- tscherts diaris pon vegnir criptads separatamain sin basa da la frasa da pass duvrada il mument da scriver u da sblocar temporarmain

Ils utilisaders duessan mantegnair lur frasa da pass en segirezza. Sche quella va a perder, po la restauraziun da tschertas datas localas esser difficila.

## 9. Avis davart novitadsziuns da quests

Sche l'utilisader activescha novitadsziuns da quests, pon novitadsziuns localas vegnir planisadas per mintga diari cun in quest actual.

- la planisaziun vegn principalmain manada dal sistem intern dal device
- tenor la configuraziun actuala dal project n'exista nagina structura confermada en la quala il text original dal diari vegn transmess periodicamain ad in server central mo per intents da novitadsziun

## 10. Avis davart l'utilisaziun da permissiuns

L'app po duvrar las suandantas permissiuns per furnir sias funcziuns:

- `INTERNET`: communicaziun cun Firebase, OpenAI e SDKs publicitars
- `com.google.android.gms.permission.AD_ID`: utilisaziun d'identificaturs publicitars
- `POST_NOTIFICATIONS`: mussar novitadsziuns da quests
- `RECEIVE_BOOT_COMPLETED`: restaurar novitadsziuns planisadas suenter in restart dal device

Permissiuns vegnan duvradas mo a la mesira necessaria per exequir las funcziuns relevantas.

## 11. Dretgs da l'object da datas e co als exequir

Ils utilisaders pon exequir ils suandants dretgs:

- acceder, modifitgar e stizzar datas entaifer l'app
- stizzar u surscriver datas memorisadas en il cloud
- pretender log-out e stizzada dal conto
- midar las opziuns da privacy da novitadsziuns publicitaras
- deactivar permissiuns da novitadsziuns

Co exequir quests dretgs:

- stizzar u modifitgar directamain diaris entaifer l'app
- stizzar l'app u resettar las datas localas
- far log-out dal conto e pretender separatamain la stizzada
- midar novitadsziuns, identificaturs publicitars e permissiuns en ils parameters dal device
- e-mail da contact: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Mesiras da segirezza

L'app applitgescha u po applitgar las suandantas mesiras da protecziun:

- communicaziun basada sin HTTPS
- blocada locala da l'app da diari e criptaziun
- arcunaziun separada da novitadsziuns da verificaziun da la frasa da pass
- utilisaziun da Firebase Authentication
- dumondas da permissiuns minimalas

I pon dentant sa resultar ristgs tenor il status da segirezza dal device da l'utilisader, sco rooting, jailbreaking, malware u utilisaziun d'in device partì.

## 13. Datas persunalas d'uffants

L'app n'è betg concepida sco servetsch destinà principalmain ad uffants. Tuttina pon opziuns colliadas cun la vegliadetgna entaifer UMP vegnir applitgadas durant il tractament da novitadsziuns publicitaras/consentiment.

## 14. Midadas a questa decleraziun

Questa decleraziun po vegnir revedida pervi da novitadsziuns en las leschas, servetschs da terzas varts u funcziuns da l'app.

- Ultima actualisaziun per la versiun actuala: **2026-04-19**

## 15. Contact

- Sviluppader: frog-im
- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Guida per stizzar il conto: [Instrucziuns per stizzar](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)


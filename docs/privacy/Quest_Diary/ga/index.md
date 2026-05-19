---
title: Polasaí Príobháideachais | QDiary
description: Polasaí Príobháideachais QDiary
---

# Polasaí Príobháideachais (QDiary)

- Ainm na hAipe: QDiary
- Forbróir: frog-im
- Teagmháil: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Dáta Teacht i bhFeidhm: 2026-04-19
- Nuashonrú Deireanach: 2026-04-19

Tá an Polasaí Príobháideachais seo bunaithe ar chur i bhfeidhm reatha na haipe QDiary. Soláthraíonn QDiary gnéithe chun dialanna a scríobh, questanna a ghiniúint agus machnamh a dhéanamh orthu, logáil isteach, sábháil de láimh sa scamall, fógraíocht, agus fógraí. Sa phróiseas sin, féadfaidh sé sonraí pearsanta nó faisnéis a d’fhéadfaí a mheas mar shonraí pearsanta a phróiseáil a mhéid is gá.

## 1. Gnéithe a Chuirtear ar Fáil

Soláthraíonn QDiary na gnéithe seo a leanas:

- Dialanna a scríobh, a chur in eagar, agus a fheiceáil
- Rangú de réir catagóire agus amharc féilire
- Giniúint questanna, machnamh ar questanna, agus láimhseáil chríochnú questanna
- Glas áitiúil na haipe dialainne agus criptiú áitiúil
- Logáil isteach le ríomhphost, fíorú ríomhphoist, logáil isteach anaithnid (aoi), agus athshocrú pasfhocail
- Sábháil agus luchtú sa scamall ar thionscnamh an úsáideora
- Taispeáint fógraí agus láimhseáil roghanna príobháideachais fógraíochta
- Fógraí meabhrúcháin quest

## 2. Catagóirí na Faisnéise a Phróiseáiltear

### 2-1. Faisnéis a Iontrálann an tÚsáideoir go Díreach

- Seoladh ríomhphoist
- Pasfhocal
- Teideal na dialainne, ábhar, dáta, catagóir, agus deacracht
- Freagraí ar questanna, ábhar machnaimh, agus faisnéis faoin quest roghnaithe
- Roghanna a bhaineann le próifíl an quest agus téacs achoimre
- Frása faire do ghlas na haipe dialainne

### 2-2. Faisnéis a Stórálann an Aip ar an nGléas

- Bunachar sonraí áitiúil na dialainne (SQLite)
- Faisnéis faoi stádas questanna do dhialanna áitiúla
- Luachanna stádais a bhaineann le freastal, socruithe, teanga, fógraí, agus fógraíocht
- Luachanna fíoraithe ghlais na haipe, salt, agus meiteashonraí criptiúcháin
- Faisnéis sceidealaithe fógraí quest

### 2-3. Faisnéis Chuntais agus Aitheantais

Féadfar an fhaisnéis seo a leanas a phróiseáil trí Firebase Authentication:

- Firebase UID
- Seoladh ríomhphoist
- Cibé ar críochnaíodh fíorú ríomhphoist
- Cibé an bhfuil logáil isteach anaithnid in úsáid

### 2-4. Faisnéis Fógraíochta agus Toilithe

Agus Google AdMob agus an UMP SDK á n-úsáid, féadfar an fhaisnéis seo a leanas a phróiseáil:

- Aitheantóirí fógraíochta (mar shampla Android AD_ID)
- Seoladh IP agus faisnéis líonra
- Faisnéis ghléis, leagan an chórais oibriúcháin, agus faisnéis na haipe
- Faisnéis faoi imprisean fógraí, cliceálacha, agus próiseáil luaíochtaí
- Stádas toilithe fógraíochta agus stádas na roghanna príobháideachais

### 2-5. Faisnéis a Bhaineann le Fógraí

- Cibé ar tugadh cead d’fhógraí
- Luachanna aitheantais do dhialanna a bhfuil questanna leanúnacha iontu
- Téacs fógra quest
- Amanna fógra sceidealaithe

## 3. Críocha na Próiseála

Próiseálann an aip faisnéis chun na gcríoch seo a leanas:

- Clárú, logáil isteach, fíorú ríomhphoist, agus athshocrú pasfhocail
- Dialanna a scríobh, a shábháil, agus a fheiceáil
- Giniúint questanna, machnamh, agus cinneadh críochnaithe
- Criptiú agus díchriptiú áitiúil a bhaineann le glas na haipe
- Sábháil agus luchtú sa scamall a iarrann an t-úsáideoir
- Fógraí quest a sholáthar
- Fógraí a sholáthar, luaíochtaí fógraíochta a phróiseáil, agus stádas toilithe fógraíochta a léiriú
- Slándáil, láimhseáil earráidí, agus oibriú na seirbhíse

## 4. Stóráil Áitiúil, Stóráil sa Scamall, agus Próiseáil Sheachtrach

### 4-1. Stóráil Áitiúil

Stóráiltear faisnéis faoi dhialanna agus questanna go príomha i mbunachar sonraí áitiúil an ghléis.

- Mura bhfuil glas na haipe cumasaithe: stóráiltear go háitiúil í i bhfoirm ghinearálta
- Má tá glas na haipe cumasaithe: féadfar cuid den fhaisnéis, mar shampla teideal na dialainne, ábhar, agus stádas quest, a chriptiú agus a stóráil go háitiúil

### 4-2. Stóráil sa Scamall

Ní stórálann an aip sonraí i Firebase Firestore ach amháin nuair a ritheann an t-úsáideoir an ghné `Save` go díreach.

Faoi chumraíocht reatha an tionscadail:

- Ní úsáidtear sioncrónú iomlán uathoibríoch
- Ní stóráiltear sonraí in Firestore `savedDiaries` ach amháin nuair a shábhálann an t-úsáideoir iad de láimh
- Agus iad á sábháil, féadfar teideal na dialainne, ábhar, agus stádas quest a stóráil i bhfoirm chriptithe ag brath ar stádas reatha ghlais na haipe
- Ní lódáiltear na sonraí ar ais chuig an stóráil áitiúil ach amháin nuair a ritheann an t-úsáideoir `Load`

### 4-3. Próiseáil Sheachtrach le haghaidh Giniúint agus Machnamh Questanna

Nuair a iarrann an t-úsáideoir giniúint quest nó machnamh, féadfar an fhaisnéis seo a leanas a úsáid le haghaidh próiseála seachtraí trí Firebase Functions:

- Teideal na dialainne
- Ábhar na dialainne nó ábhar an mhachnaimh
- Catagóir
- Deacracht
- An quest roghnaithe
- Faisnéis achoimre phróifíl an quest

Úsáidtear an fhaisnéis seo chun questanna a ghiniúint agus a mheas trí OpenAI API.

Tábhachtach:

- Ní úsáidtear ábhar gaolmhar na dialainne le haghaidh próiseála seachtraí ach amháin nuair a úsáidtear an ghné quest.
- Faoi chumraíocht reatha an tionscadail, ní úsáidtear cód a stórálann logaí quest i mbailiúchán ar leith dar teideal `questLogs`.

## 5. Seirbhísí Tríú Páirtí agus Próiseáil Sheachfhoinsithe

### 5-1. Google Firebase

Cuspóir:

- Fíordheimhniú (Firebase Authentication)
- Stóráil Firestore
- Rith Cloud Functions

Faisnéis a d’fhéadfaí a phróiseáil:

- UID, seoladh ríomhphoist, agus stádas fíordheimhnithe
- Sonraí dialainne a shábhálann an t-úsáideoir de láimh
- Sonraí iarratais quest

### 5-2. OpenAI

Cuspóir:

- Giniúint quest
- Machnamh ar quest agus measúnú críochnaithe

Faisnéis a d’fhéadfaí a phróiseáil:

- Teideal/ábhar na dialainne
- Téacs an quest
- Deacracht agus catagóir
- Ábhar machnaimh a iontrálann an t-úsáideoir
- Faisnéis achoimre phróifíl an quest

### 5-3. Google AdMob / UMP

Cuspóir:

- Fógraí meirge, idirstitial, agus luaíochta a sholáthar
- Toiliú fógraíochta agus roghanna príobháideachais a láimhseáil

Faisnéis a d’fhéadfaí a phróiseáil:

- Aitheantóirí fógraíochta
- Faisnéis ghléis agus líonra
- Faisnéis idirghníomhaíochta le fógraí
- Stádas toilithe

## 6. Fógra maidir le hAistrithe Idirnáisiúnta

Féadfaidh an aip sonraí pearsanta nó faisnéis ghaolmhar a phróiseáil lasmuigh de thír an úsáideora sna cásanna seo a leanas:

| Mír | Sonraí |
|---|---|
| Faighteoir | Google LLC, OpenAI, agus oibreoirí bonneagair ghaolmhara |
| Tír Chinn Scríbe | Stáit Aontaithe Mheiriceá, srl. |
| Tráth an Aistrithe | Le linn logála isteach, giniúna/machnaimh quest, iarratais ar fhógraí, agus próiseála toilithe |
| Modh an Aistrithe | Cumarsáid líonra chriptithe |
| Cuspóir an Aistrithe | Fíordheimhniú, stóráil sonraí, próiseáil gan fhreastalaí, giniúint/measúnú questanna le IS, agus fógraíocht |

## 7. Tréimhse Coinneála agus Úsáide

Coinníonn an aip faisnéis de réir na gcaighdeán seo a leanas:

- Faisnéis áitiúil dialainne/socruithe: go dtí go scriosann an t-úsáideoir í nó go ndíshuiteálann sé an aip
- Faisnéis chuntais Firebase: fad a choinníonn an t-úsáideoir an cuntas
- Sonraí atá stóráilte in Firestore: fad a choinníonn an t-úsáideoir na míreanna sábháilte
- Sonraí próiseála iarratais quest: a mhéid is gá le haghaidh próiseála gan fhreastalaí
- Sonraí a bhaineann le fógraíocht/toiliú: de réir pholasaí gach soláthraí seachtraigh

Ina theannta sin, áirítear leis an tionscadal reatha an loighic ghlantacháin uathoibríoch seo a leanas:

- Glanadh cuntas úsáideoirí anaithnid agus sonraí Firestore i bhfobhailiúcháin úsáideora tar éis tréimhse áirithe
- Glanadh cuntas úsáideoirí rialta atá neamhghníomhach le fada agus sonraí Firestore i bhfobhailiúcháin úsáideora

Mar sin féin, d’fhéadfadh sé a bheith éagsúil, ag brath ar stádas an imlonnaithe agus ar shocruithe an fhreastalaí, cibé an léirítear é seo go hiarbhír sa timpeallacht táirgthe.

## 8. Fógra maidir le Glas na hAipe agus Criptiú Áitiúil

Soláthraíonn an aip gné ar leith darb ainm `Diary App Lock`.

- Tá frása faire ghlais na haipe ar leithligh ó phasfhocal an chuntais.
- Úsáidtear frása faire ghlais na haipe chun an dialann áitiúil a chriptiú agus a dhíchriptiú.
- Fiú má chuirtear frása faire mícheart isteach, ní fhéadfaidh an aip féin a bheith blocáilte go hiomlán i gcónaí; ina ionad sin, d’fhéadfadh cuid d’ábhar na dialainne fanacht doléite.
- D’fhéadfadh roinnt dialann a bheith criptithe ar leithligh bunaithe ar an bhfrása faire a úsáideadh tráth na scríbhneoireachta nó an díghlasála shealadaigh.

Ba cheart d’úsáideoirí a bhfrása faire a choinneáil slán, agus má chailltear é, d’fhéadfadh sé a bheith deacair cuid de na sonraí áitiúla a aisghabháil.

## 9. Fógra maidir le Fógraí Quest

Má chumasaíonn an t-úsáideoir fógraí quest, féadfar fógraí áitiúla a sceidealú do gach dialann a bhfuil quest leanúnach inti.

- Déantar an sceidealú a láimhseáil go príomha trí sceidealú inmheánach an ghléis.
- Faoi chumraíocht reatha an tionscadail, níl aon struchtúr dearbhaithe ann ina ndéantar buntéacs na dialainne a tharchur go tréimhsiúil chuig freastalaí lárnach chun críocha fógra amháin.

## 10. Fógra maidir le hÚsáid Ceadanna

Féadfaidh an aip na ceadanna seo a leanas a úsáid chun a gnéithe a chur ar fáil:

- `INTERNET`: cumarsáid le Firebase, OpenAI, agus SDKanna fógraíochta
- `com.google.android.gms.permission.AD_ID`: úsáid a bhaint as aitheantóirí fógraíochta
- `POST_NOTIFICATIONS`: fógraí quest a thaispeáint
- `RECEIVE_BOOT_COMPLETED`: fógraí sceidealaithe a athchóiriú tar éis atosú an ghléis

Ní úsáidtear ceadanna ach a mhéid is gá chun na feidhmeanna ábhartha a chur i gcrích.

## 11. Cearta an Ábhair Sonraí agus Conas iad a Fheidhmiú

Féadfaidh úsáideoirí na cearta seo a leanas a fheidhmiú:

- Sonraí laistigh den aip a rochtain, a athrú, agus a scriosadh
- Sonraí atá stóráilte sa scamall a scriosadh nó a fhorscríobh
- Logáil amach agus scriosadh cuntais a iarraidh
- Roghanna príobháideachais fógraíochta a athrú
- Ceadanna fógraí a dhíchumasú

Conas na cearta seo a fheidhmiú:

- Dialanna a scriosadh nó a chur in eagar go díreach laistigh den aip
- An aip a scriosadh nó sonraí áitiúla a athshocrú
- Logáil amach as an gcuntas agus scriosadh a iarraidh ar leithligh
- Fógraí, aitheantóirí fógraíochta, agus ceadanna a athrú i socruithe an ghléis
- Ríomhphost teagmhála: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Bearta Slándála

Cuireann an aip na bearta cosanta seo a leanas i bhfeidhm nó féadfaidh sí iad a chur i bhfeidhm:

- Cumarsáid bunaithe ar HTTPS
- Glas áitiúil na haipe dialainne agus criptiú
- Stóráil ar leithligh ar luachanna fíoraithe an fhrása faire
- Úsáid Firebase Authentication
- An líon íosta ceadanna is gá a iarraidh

Mar sin féin, d’fhéadfadh rioscaí teacht chun cinn ag brath ar stádas slándála ghléas an úsáideora, amhail rooting, jailbreaking, bogearraí mailíseacha, nó úsáid ghléis chomhroinnte.

## 13. Sonraí Pearsanta Leanaí

Níl an aip deartha mar sheirbhís atá dírithe go príomha ar leanaí. Mar sin féin, féadfar roghanna a bhaineann le haois laistigh de UMP a chur i bhfeidhm le linn próiseála fógraíochta/toilithe.

## 14. Athruithe ar an bPolasaí seo

Féadfar an Polasaí seo a athbhreithniú de bharr athruithe i ndlíthe, i seirbhísí tríú páirtí, nó i ngnéithe na haipe.

- Nuashonrú deireanach don leagan reatha: **2026-04-19**

## 15. Teagmháil

- Forbróir: frog-im
- Ríomhphost: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Treoir maidir le cuntas a scriosadh: [Treoracha scriosta](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)


---
title: Polasaí Príobháideachais | know_me
description: know_me (PeopleNote, Memory for People) Polasaí Príobháideachais (Gaeilge)
---

# Polasaí Príobháideachais (know_me / PeopleNote, Memory for People)

- **Ainm an Aip:** know_me (PeopleNote, Memory for People)
- **Forbróir:** frog-im
- **Oifigeach Cosanta Faisnéise Pearsanta / Duine Teagmhála:** frog-im
- **Teagmháil:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Dáta Teacht i bhFeidhm:** 2026-03-04
- **Nuashonraithe go Deireanach:** 2026-03-04

> Ullmhaíodh an Beartas seo bunaithe ar an bhfaisnéis a phróiseálann an aip agus ar na gnéithe gaolmhara atá aici.  
> Má bhaineann aon dlíthe nó rialacháin éigeantacha le tír nó réigiún ar leith, féadfaidh na dlíthe nó na rialacháin sin tosaíocht a bheith acu.

---

## 1. Cuspóir agus Raon Feidhme

Is aip é `know_me` atá deartha chun cabhrú le húsáideoirí faisnéis faoi dhaoine a thaifeadadh agus a bhainistiú, agus, nuair is gá, cúltaca a dhéanamh den fhaisnéis sin, í a athchóiriú, agus í a roinnt mar chomhaid PDF.

Áirítear ar a phríomhghnéithe:

- Faisnéis a bhaineann le duine ar leith a stóráil (amhail ainm, téacs aitheantais, nótaí, tréithe pearsantachta, tír, inscne, faisnéis teagmhála, etc.)
- Aicmiú fillteán, cuardach, agus feidhmeanna cumaisc
- Grianghraif a cheangal agus bainistiú tuairiscí
- Cúltacaí (`.knm`) a easpórtáil agus a iompórtáil
- PDFanna a easpórtáil
- Glasáil na haipe (pasfhocal / patrún)
- Bainistiú fógraíochta agus toilithe (AdMob / UMP)

Ní éilíonn an aip clárú cuntais ar leith, agus stóráiltear príomhshonraí úsáideora na haipe go hiondúil go háitiúil ar ghléas an úsáideora.  
Mar sin féin, féadfaidh roinnt SDKanna tríú páirtí atá san áireamh chun críocha bainistithe fógraíochta agus toilithe cuid d’fhaisnéis a phróiseáil.

---

## 2. Catagóirí na Faisnéise Pearsanta a Phróiseáiltear

### 2-1) Faisnéis a Iontrálann an tÚsáideoir go Díreach

Ní stóráiltear an fhaisnéis seo a leanas ach amháin nuair a iontrálann an t-úsáideoir í go díreach:

- Ainm
- Téacs aitheantais (amhail cuma / tréithe a úsáidtear mar théacs meamraim)
- Nótaí
- Tréithe pearsantachta, tír, inscne
- Uimhir theileafóin
- Téacs a bhaineann le ham láithreachta / am an chruinnithe
- Faisnéis ardáin / suímh
- Ainm / dath an fhillteáin
- Cur síos ar íomhá (caption)

### 2-2) Comhaid a Roghnaítear ar an nGléas

- Comhaid íomhá a roghnaíonn an t-úsáideoir agus grianghraif á gceangal aige
- Comhaid chúltaca `.knm` a roghnaíonn an t-úsáideoir agus cúltacaí á n-iompórtáil aige
- Cosáin shábhála agus comhaid shábháilte a roghnaíonn an t-úsáideoir agus PDFanna / cúltacaí á n-easpórtáil aige

### 2-3) Sonraí a Stóráiltear go hÁitiúil Laistigh den Aip

Féadfar na sonraí seo a leanas a stóráil ar ghléas an úsáideora chun gnéithe na haipe a sholáthar:

- Bunachar sonraí SQLite (`people_note.db`): meiteashonraí do dhaoine / fillteáin / ardáin / suímh / íomhánna
- Comhaid íomhá: criptithe agus stóráilte laistigh d’fhillteán doiciméad na haipe (`.enc`)
- Socruithe na haipe (`SharedPreferences`): téama, sórtáil, roghanna príobháideachais / fógraí, roghanna maiscithe PDF, beartais ghlasála aip, etc.
- Faisnéis ghlasála na haipe: luachanna haishe agus salainn do phasfhocail / phatrúin (`SharedPreferences`)
- Eochracha criptiúcháin áitiúla: stóráilte in `flutter_secure_storage`
- Comhaid shealadacha: réamhamhairc díchriptiúcháin íomhá, comhaid taisce iompórtála / easpórtála, etc. (fillteán sealadach)

### 2-4) Faisnéis a D’fhéadfadh a Bheith Próiseáilte go hUathoibríoch le linn Láimhseála Fógraíochta agus Toilithe

Nuair atá gnéithe fógraíochta nó bainistithe toilithe cumasaithe, féadfaidh SDKanna Google LLC agus comhpháirtithe gaolmhara (amhail AdMob agus UMP) an fhaisnéis seo a leanas a phróiseáil go huathoibríoch:

- Aitheantóirí fógraíochta (AAID / IDFA, etc.)
- Seoladh IP agus faisnéis líonra
- Faisnéis gléis (leagan OS, samhail ghléis, leagan na haipe, etc.)
- Faisnéis idirghníomhaíochta fógra (taispeántais, cliceanna, etc.)
- Stádas toilithe agus faisnéis faoi roghanna príobháideachais
- Faisnéis a bhaineann le diagnóisic, feidhmíocht, agus slándáil

Ní uaslódáiltear príomhthaifid úsáideora na haipe go hiondúil chuig freastalaí an fhorbróra, ach féadfar cuid den fhaisnéis thuas a tharchur chuig seirbhísí tríú páirtí agus gnéithe fógraíochta / toilithe á n-úsáid.

---

## 3. Cuspóir Phróiseáil na Faisnéise Pearsanta

Próiseálann an aip faisnéis phearsanta nó faisnéis ghaolmhar chun na gcríoch seo a leanas:

- Faisnéis a bhaineann le daoine a thaifeadadh agus a bhrabhsáil, dírithe ar theagmhálacha / nótaí
- Gnéithe eagrúcháin a sholáthar amhail aicmiú fillteán, cuardach, agus cumasc
- Grianghraif a cheangal agus a thaispeáint
- Feidhmeanna a iarrann an t-úsáideoir a chomhlíonadh, amhail cúltaca / athchóiriú agus easpórtáil PDF
- Gnéithe slándála glasála aip a sholáthar
- Fógraíocht a sholáthar, toiliú a bhainistiú, gníomhaíocht chalaoiseach a chosc, agus oibleagáidí dlí a chomhlíonadh

---

## 4. Tréimhse Choinneála agus Stórála na Faisnéise Pearsanta

- Sonraí inmheánacha na haipe (SQLite, socruithe áitiúla, íomhánna criptithe): coinnítear ar ghléas an úsáideora iad go dtí go scriostar an aip, go nglantar sonraí na haipe, nó go scriosann an t-úsáideoir na sonraí go díreach
- Comhaid shealadacha: scriostar iad tar éis don tasc ábhartha a bheith críochnaithe nó glantar iad de réir bheartas taisce an chórais oibriúcháin
- Comhaid a easpórtálann an t-úsáideoir (PDFanna, comhaid chúltaca): féadfaidh siad fanacht sa suíomh stórála a roghnaíonn an t-úsáideoir agus ní mór don úsáideoir iad a scriosadh go díreach
- Sonraí a bhaineann le fógraíocht / toiliú (arna bpróiseáil ag tríú páirtithe): faoi réir bheartais gach soláthraí seirbhíse agus na ndlíthe is infheidhme

Mar phrionsabal, ní stórálann an aip príomhthaifid úsáideora ar fhreastalaí an fhorbróra.  
Mar sin féin, déantar comhaid a shábhálann an t-úsáideoir go díreach chuig stóráil sheachtrach a bhainistiú laistigh de thimpeallacht an úsáideora féin.

---

## 5. Nósanna Imeachta agus Modhanna chun Faisnéis Phearsanta a Scriosadh

Nuair atá cuspóir na próiseála bainte amach, nó nuair a iarrann an t-úsáideoir scriosadh, scriosann an aip an fhaisnéis ábhartha nó próiseálann sí í ionas nach ndéanfar tagairt di a thuilleadh, mar seo a leanas.

### 5-1) Nósanna Imeachta um Scriosadh

- Nuair a scriosann an t-úsáideoir go díreach taifid duine aonair, fillteáin, íomhánna, sonraí cúltaca, etc., meastar go bhfuil na sonraí sin faoi réir scriosadh láithreach.
- Nuair a scriosann an t-úsáideoir an aip nó a ghlanann sé sonraí na haipe ó shocruithe an ghléis, baintear na sonraí atá stóráilte i limistéar stórála inmheánaigh na haipe de réir nósanna imeachta scriosta an chórais oibriúcháin.
- Éiríonn comhaid shealadacha faoi réir glanta tar éis don tasc ábhartha críochnú, agus féadfaidh roinnt sonraí taiscthe fanacht go dtí pointe áirithe ag brath ar bheartas an chórais oibriúcháin.

### 5-2) Modhanna Scriosta

- Sonraí SQLite: scriosadh na dtaifead ábhartha
- Socruithe na haipe (`SharedPreferences`): scriosadh na heochrach ábhartha nó gach socrú
- Luachanna `flutter_secure_storage`: scriosadh na míreanna stórála slána ábhartha
- Comhaid inmheánacha na haipe (íomhánna criptithe, comhaid shealadacha, etc.): scriosadh na gcomhad ábhartha
- PDFanna / comhaid chúltaca a shábhálann an t-úsáideoir go díreach chuig stóráil sheachtrach: ní scriostar go huathoibríoch iad ag an aip agus ní mór don úsáideoir iad a scriosadh go díreach

Mura n-éilíonn dlíthe is infheidhme a mhalairt, ní stórálann an forbróir príomhthaifid úsáideora ar leithligh ar fhreastalaí an fhorbróra.

---

## 6. Soláthar do Thríú Páirtithe, Foinsiú Seachtrach, agus Aistriú Trasteorann

Féadfaidh an aip seirbhísí Google a úsáid le haghaidh bainistithe fógraíochta agus toilithe.

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

Ní bhailíonn ná ní dhíolann an forbróir príomhshonraí taifead daoine na haipe trína fhreastalaí féin.

---

## 7. Faisnéis faoi na Ceadanna a Úsáidtear

Féadfaidh an aip na ceadanna seo a leanas a úsáid:

- `INTERNET`: cumarsáid do SDKanna fógraíochta agus gnéithe líonra gaolmhara
- `com.google.android.gms.permission.AD_ID`: úsáid aitheantóirí fógraíochta (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 agus níos ísle): grianghraif a cheangal / a roghnú

Ní úsáidtear ceadanna ach laistigh den raon atá riachtanach chun na gnéithe ábhartha a sholáthar.

---

## 8. Suiteáil, Oibriú, agus Diúltú do Mheicníochtaí Bailithe Uathoibríche

Ní oibríonn an aip seo gnáthfhianáin láithreán gréasáin go díreach.  
Mar sin féin, i ndáil le gnéithe fógraíochta agus bainistithe toilithe, féadfaidh SDKanna tríú páirtí aitheantóirí fógraíochta, faisnéis líonra, faisnéis gléis, agus sonraí comhchosúla a phróiseáil go huathoibríoch.

Féadfaidh úsáideoirí na socruithe ábhartha a choigeartú ar na bealaí seo a leanas:

- Roghanna a athrú laistigh de roghanna príobháideachais na haipe nó den scáileán bainistithe toilithe (nuair a chuirtear ar fáil iad)
- An aitheantóir fógraíochta a athshocrú nó a scriosadh i socruithe chóras oibriúcháin an ghléis
- Fógraí pearsantaithe a theorannú nó roghanna príobháideachais gaolmhara a choigeartú i socruithe chóras oibriúcháin an ghléis

Má theorannaíonn an t-úsáideoir fógraíocht phearsantaithe, féadfar fógraí neamhphearsantaithe a sholáthar, nó féadfar roinnt gnéithe a bhaineann le fógraí a shrianadh.

---

## 9. Cearta Úsáideora agus Conas Iad a Fheidhmiú

Faoi réir na ndlíthe is infheidhme, féadfaidh na cearta seo a leanas a bheith ag úsáideoirí:

- Rochtain ar fhaisnéis phearsanta, ceartú uirthi, nó scriosadh di a iarraidh
- Fionraí nó srianadh na próiseála a iarraidh
- Toiliú le haghaidh próiseála bunaithe ar thoiliú a tharraingt siar
- Roghanna fógraíochta / toilithe a athrú

Féadfar na cearta seo a fheidhmiú ar na bealaí seo a leanas:

- Sonraí a mhodhnú nó a scriosadh go díreach laistigh den aip
- Sonraí áitiúla a thúsú trí shonraí na haipe a scriosadh nó an aip a dhíshuiteáil
- Toiliú fógraíochta a athrú trí roghanna príobháideachais / scáileán toilithe na haipe (i réigiúin ina gcuirtear ar fáil é)
- An t-aitheantóir fógraíochta a athshocrú / a scriosadh nó fógraí pearsantaithe a theorannú trí shocruithe OS an ghléis
- Teagmháil: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Bearta Slándála

Cuireann an forbróir na bearta seo a leanas i bhfeidhm nó déanann sé iarracht iad a chur i bhfeidhm:

- Stóráiltear taifid úsáideora go hiondúil go háitiúil ar an ngléas
- Stóráiltear comhaid íomhá ceangailte go háitiúil i bhfoirm chriptithe (bunaithe ar AES-GCM)
- Stóráiltear faisnéis ghlasála na haipe i bhfoirm haishe seachas i ngnáth-théacs
- Stóráiltear comhaid chúltaca tar éis iad a chriptiú bunaithe ar phasfhocal úsáideora
- Tá cumarsáid le SDKanna tríú páirtí criptithe (HTTPS / TLS)
- Úsáidtear ceadanna leis an íosraon rochtana atá riachtanach

Mar sin féin, ní féidir rioscaí a eascraíonn as riocht slándála ghléas an úsáideora (amhail rooting / jailbreaking, aipeanna mailíseacha, nó nochtadh stórála comhroinnte) a dhíchur go hiomlán.

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

Nuashonraithe go Deireanach: **2026-03-04**
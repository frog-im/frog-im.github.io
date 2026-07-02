---
title: Decleraziun da protecziun da datas | FileGuard
description: Decleraziun da protecziun da datas da FileGuard
lang: rm
last_updated: 2026-06-23
---

# Decleraziun da protecziun da datas (FileGuard)

- **App:** FileGuard
- **Sviluppader:** frog-im
- **Contact per la protecziun da datas:** frog-im
- **E-mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data d'entrada en vigur:** 23 da zercladur 2026
- **Ultima actualisaziun:** 23 da zercladur 2026

> Questa decleraziun descriva l'implementaziun actuala da l'app FileGuard. Leschas obligatoricas en tes pajais u en tia regiun pon avair precedenza.

---

## 1. Champ d'applicaziun e intent

FileGuard è in utensil da segirezza che ta permetta da tegnair datotecas tschernidas, medias registradas, notas e text dal clipboard en vaults criptads sin tes apparat e da crear datotecas da backup criptadas.

L'app na pretenda nagina registraziun u annunzia. Il sviluppader na gestiunescha nagin server che survegn tias datotecas da vault, cuntegn da datotecas, pleds-clav, nums da vault u istorgia d'activitad. Sin Android po l'app dentant duvrar Google AdMob e Google User Messaging Platform (UMP) per reclama e tschernas da protecziun da datas.

## 2. Infurmaziuns elavuradas

### 2.1 Datas da vault tschernidas u creadas da tai

L'app po elavurar las suandantas infurmaziuns sin tes apparat:

- Fotos, videos, documents ed autras datotecas che ti tschernas tras il selectader da datotecas dal sistem
- Fotos u videos registrads cun l'app, inclusiv audio registrà cun in video
- Text dal clipboard che ti salvas manualmain u che vegn detectà cur che ti activeschas la protecziun automatica dal clipboard
- Num da datoteca, tip MIME, grondezza, temp da creaziun, legenda ed infurmaziuns colliadas cun la prevista
- Num ed identificatur dal vault, classificaziun da segirezza, status da la datoteca originala e referenza da la datoteca originala
- Pachets criptads d'export, transfer u backup che ti creas

Questas infurmaziuns vegnan elavuradas sin tes apparat per furnir las funcziuns da l'app. Il sviluppader na las chargia betg si sin in server gestiunà dal sviluppader.

### 2.2 Infurmaziuns d'autentificaziun e segirezza

L'app po elavurar las suandantas infurmaziuns en ina memoria segira sin tes apparat:

- Salts, parameters da derivaziun da clav e pachets da clavs criptads duvrads per derivar u proteger clavs da criptaziun
- Datas d'access al vault e clavs localas protegidas d'ina clav liada al apparat per access biometric
- Preferenzas da segirezza sco protecziun da screenshots, stizzar il clipboard, reautentificaziun biometrica e protecziun automatica

Tes pled-clav en text cler na vegn betg tramess al sviluppader. L'autentificaziun biometrica vegn fatga dal sistem operativ. L'app na rimna betg maletgs da dets u da fatscha, ni models biometrics; ella survegn mo il resultat da l'autentificaziun.

### 2.3 Infurmaziuns localas d'activitad e backup

L'app po memorisar localmain:

- Il tip, la descripziun, il temp ed ils identificaturs d'objects colliads per eveniments da protecziun, serrar, stizzar, stizzar l'original, backup e restauraziun
- Fin a 500 endataziuns dal log d'activitad
- Destinaziun dal backup, temp dal davos backup, dumber d'objects e status da success u sbagl
- Sche il backup automatic è activà e il pled-clav necessari per actualisar quel backup
- Tschernas da protecziun da datas per reclama, tscherna da processar datas restrenschidas e dumber d'objects protegids duvrà per la frequenza da reclama

Parameters sensibels, inclusiv il status dal backup ed il pled-clav dal backup automatic, vegnan memorisads en ina memoria locala criptada cun ina clav dal apparat. Ti es responsabel da tegnair segir tes pled-clav da backup.

### 2.4 Infurmaziuns elavuradas durant reclama e consentiment

Sin la plattafurma da reclama sustegnida, actualmain Android, po l'app duvrar Google AdMob e UMP. Google e furniturs da tecnologia da reclama pon elavurar:

- Identificaturs colliads cun reclama, instanza da l'app u apparat
- Adressa IP e lieu approximativ deducì da infurmaziuns sco l'adressa IP
- Model dal apparat, sistem operativ, versiun da l'app, lingua ed infurmaziuns da rait
- Dumondas da reclama, impressiuns, clics, interacziuns e diagnostica
- Status da consentiment e tschernas regiunalas da protecziun da datas

Questas infurmaziuns pon vegnir duvradas per furniziun da reclama, reclama betg persunalisada, limitaziun da frequenza, mesiraziun, prevenziun da fraud, administraziun dal consentiment, segirezza e conformitad legala. L'app è implementada uschia che Google Mobile Ads SDK vegn inizialisà mo suenter che UMP inditgescha che reclama po vegnir dumandada.

Vesair la [Politica da protecziun da datas da Google](https://policies.google.com/privacy) e las [infurmaziuns davart tecnologias da reclama da Google](https://policies.google.com/technologies/ads).

## 3. Intents da l'elavuraziun

FileGuard elavura infurmaziuns per:

- Memorisar e mussar cuntegn tschernì u registrà en vaults criptads
- Controllar l'access al vault cun serrar, pleds-clav ed autentificaziun biometrica
- Importar, exportar, spustar, stizzar e persequitar il status da la datoteca originala dal cuntegn
- Crear e restaurar backups criptads en in lieu tschernì da tai
- Mantegnair preferenzas da segirezza e stizzar datotecas temporaras decriptadas e cuntegn dal clipboard
- Mussar activitad da segirezza locala e status d'errur
- Furnir reclama Android, controllar la frequenza da reclama e porscher tschernas da protecziun da datas
- Prevegnir abus, segirar il servetsch e satisfar ad obligaziuns legalas

## 4. Memorisaziun e retenziun

| Categoria | Memorisaziun e retenziun | Co stizzar |
|---|---|---|
| Datotecas e metadata da vault criptadas | Memorisadas en la memoria locala privata da l'app fin che ti las stizzas | Stizza l'object u il vault en l'app, stizza las datas da l'app u disinstallescha |
| Datas d'access e parameters da segirezza | Memorisads en memoria segira dal sistem operativ ed en memoria criptada cun clav dal apparat fin ch'els vegnan midads u che las datas da l'app vegnan allontanadas | Deactivescha la funcziun relevanta, stizza las datas da l'app u disinstallescha |
| Istorgia d'activitad | Fin a 500 endataziuns en memoria locala criptada | Stizza las datas da l'app u disinstallescha |
| Datotecas temporaras decriptadas | Scrittas temporarmain en il cache da l'app e stizzadas al start, al passar en il fund u al terminar la funcziun tenor il meglier effort | Serrar l'app u stizzar ses cache/datas |
| Cuntegn dal clipboard | Elavurà tras il clipboard dal sistem operativ cur che copiar u protecziun automatica vegn duvrà | Stizzar automatic tenor meglier effort, copiar auter cuntegn u reaviar il apparat |
| Datotecas da backup criptadas | Memorisadas en in ordinatur dal apparat, in furnitur da documents u in lieu sincronisà cun cloud che ti tschernas fin che ti las stizzas | Stizzar tras il manager da datotecas u servetsch da memoria relevant |
| Datas da reclama da Google | Retegnidas tenor las politicas da Google e dals processaders e tenor obligaziuns legalas | Midar ils parameters da reclama da l'app/apparat u duvrar ils controls da protecziun da datas da Google |

Il sistem operativ, il producent dal apparat, il furnitur da documents u il furnitur da backup en cloud pon tegnair copias separadas da las datas da l'app u da las datotecas da backup che ti creas. Quellas copias èn suttamessas a las politicas dal furnitur relevant.

## 5. Terzas partidas, furniturs da servetsch e vendita

Il sviluppader na venda betg cuntegn da vault, pleds-clav u istorgia d'activitad en l'app e na las dat betg a terzas partidas tras in server gestiunà dal sviluppader.

Cur che funcziuns da reclama u consentiment Android funcziuneschan, pon Google LLC, affiliads da Google, furniturs da tecnologia da reclama e processaders colliads elavurar las infurmaziuns descrittas en Secziun 2.4. Vesair il [Avis da transfer internaziunal da datas](policy/) separà.

Sche ti tschernas directamain in'app externa u in servetsch cloud tras in selectader da datotecas, funcziun da parter u destinaziun da backup, po quel furnitur elavurar datotecas tenor tia instrucziun. Sia politica da protecziun da datas e ses parameters da segirezza valan, ed il sviluppader na controlescha betg las praticas dal furnitur.

## 6. Transfers internaziunals da datas

Cuntegn da vault na vegn betg transferì ad in server gestiunà dal sviluppader. Infurmaziuns da reclama e consentiment pon vegnir elavuradas da Google e processaders colliads en ils Stadis Unids ed auters pajais nua ch'els gestiuneschan infrastructura.

Sche ti tschernas in servetsch cloud a l'exteriur sco lieu per in backup criptà, po la datoteca vegnir sincronisada cun servers ordaifer tes pajais tenor tia instrucziun. Vesair il [Avis da transfer internaziunal da datas](policy/) per detagls.

## 7. Permissiuns

L'app po duvrar las suandantas permissuns u capacitads dal sistem cur che ti dovras la funcziun relevanta:

- **Datotecas e fotos:** Importar mo cuntegn che ti tschernas
- **Camera:** Registrar fotos u videos per il vault
- **Microfon:** Includer audio cur che ti registreschas video
- **Biometria:** Confermar access al vault u midadas da parameters sensibels
- **Internet e status da rait sin Android:** Dumandar reclama AdMob ed infurmaziuns da consentiment UMP
- **Advertising ID sin Android:** Sustegnair funcziuns da reclama da Google
- **Clipboard:** Copiar cuntegn u proteger text dal clipboard cur che ti activeschas explicitamain la protecziun automatica

Refusar ina permissiun po deactivar mo la funcziun colliada. Cur ch'il selectader da datotecas dal sistem vegn duvrà, è l'access generalmain limità als objects che ti tschernas.

## 8. Mesiras da segirezza e limitaziuns

L'implementaziun actuala dovra mesiras che includan:

- Criptaziun AES-256-GCM per cuntegn da vault ed indexs da vault
- Derivaziun da clav PBKDF2-HMAC-SHA256 per clavs basadas sin pled-clav
- Protecziun Android Keystore u StrongBox per clavs localas sin apparats Android sustegnids
- Criptaziun cun clav dal apparat per parameters sensibels ed istorgia d'activitad
- Serrar il vault e nettegiar datotecas temporaras e clipboard tenor meglier effort cur che l'app va en il fund
- Protecziun facultativa da screenshots e reautentificaziun biometrica
- Pachets da backup portabels criptads cun pled-clav

Nagina metoda da segirezza na removescha mintga ristga. Enguladitsch dal apparat, malware, vulnerabilitads dal sistem operativ, pleds-clav flaivels, datotecas partidas da tai u problems da segirezza tar in furnitur extern da memoria pon exponer infurmaziuns.

Avrir u exportar cuntegn decriptà en in'autra app po crear ina copia separada. Stizzar la datoteca originala e nettegiar datotecas temporaras u clipboard po vegnir limità dal sistem operativ; perquai duessas verifitgar l'allontanament da cuntegn sensibil.

## 9. Tes dretgs e tias tschernas

La pli gronda part da las infurmaziuns resta mo sin tes apparat, uschia che il sviluppader na po betg acceder, curreger u stizzar ellas a distanza. Ti pos:

- Stizzar objects da vault u vaults en l'app
- Midar parameters da segirezza, biometria, protecziun automatica, clipboard e backup automatic
- Stizzar datas u cache da l'app, u disinstallar l'app
- Stizzar datotecas da backup ed exportadas dal lieu da memoria
- Nua che disponibel, midar il consentiment tras las opziuns da protecziun da datas per reclama Google en l'app
- Stizzar u resetar l'identificatur da reclama u limitar la persunalisaziun da reclama en ils parameters dal apparat

Ti pos contactar nus davart infurmaziuns che ti has furnì directamain al sviluppader, sco in e-mail da dumonda. Nua che applicabel, po il dretg local dar a tai dretgs d'access, correctura, stizzar, restricziun, retratga dal consentiment e reclamaziun tar in'autoritad da surveglianza.

## 10. Uffants

FileGuard n'è betg concepì principalmain per uffants e na pretenda betg che uffants furneschian infurmaziuns persunalas. Guardians pon duvrar controls parentals furnids dal apparat u dal store d'apps. La configuraziun da consentiment per persunas sut la vegliadetgna per reclama Android duai vegnir examinada separadamain en vista al public previs ed al dretg applicabel avant la distribuziun.

## 11. Contact

Per dumondas davart questa Decleraziun:

- **Contact:** frog-im
- **E-mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Per datas da reclama elavuradas da Google, dovra ils controls da protecziun da datas e las proceduras da contact descrittas en la [Politica da protecziun da datas da Google](https://policies.google.com/privacy).

## 12. Midadas da questa Decleraziun

Nus pudain actualisar questa Decleraziun cur che leschas, funcziuns da l'app, permissuns u praticas da SDK da terzas partidas sa midan. Midadas materialas pon vegnir communitgadas sin questa pagina, en l'app u tras la pagina da distribuziun.

Ultima actualisaziun: **23 da zercladur 2026**

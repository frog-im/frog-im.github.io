---
title: Informativa sulla Privacy | know_me
description: know_me (PeopleNote, Memory for People) Informativa sulla Privacy (Italiano)
---

# Informativa sulla Privacy (know_me / PeopleNote, Memory for People)

- **Nome dell'app:** know_me (PeopleNote, Memory for People)
- **Sviluppatore:** frog-im
- **Responsabile della protezione dei dati / Referente:** frog-im
- **Contatto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data di entrata in vigore:** 2026-03-04
- **Ultimo aggiornamento:** 2026-03-04

> La presente Informativa è stata redatta sulla base delle informazioni trattate dall'app e delle relative funzionalità.  
> Qualora in uno specifico Paese o in una specifica regione si applichino leggi o regolamenti obbligatori, tali leggi o regolamenti potranno prevalere.

---

## 1. Finalità e Ambito di Applicazione

`know_me` è un'app progettata per aiutare gli utenti a registrare e gestire informazioni relative a persone e, quando necessario, a eseguire backup, ripristinare e condividere tali informazioni come file PDF.

Le sue funzionalità principali includono:

- Memorizzazione di informazioni specifiche relative a una persona (come nome, testo identificativo, note, tratti della personalità, Paese, genere, informazioni di contatto, ecc.)
- Classificazione in cartelle, ricerca e funzioni di unione
- Allegare foto e gestire descrizioni
- Esportazione e importazione di backup (`.knm`)
- Esportazione di PDF
- Blocco dell'app (password/schema)
- Gestione della pubblicità e del consenso (AdMob/UMP)

L'app non richiede la registrazione di un account separato e i dati principali dell'utente vengono generalmente archiviati localmente sul dispositivo dell'utente.  
Tuttavia, alcuni SDK di terze parti inclusi per la gestione della pubblicità e del consenso possono trattare alcune informazioni.

---

## 2. Categorie di Dati Personali Trattati

### 2-1) Informazioni inserite direttamente dall'utente

Le seguenti informazioni vengono memorizzate solo quando l'utente le inserisce direttamente:

- Nome
- Testo identificativo (ad esempio aspetto/caratteristiche utilizzati come testo di promemoria)
- Note
- Tratti della personalità, Paese, genere
- Numero di telefono
- Testo relativo al momento di apparizione / al momento dell'incontro
- Informazioni sulla piattaforma/sito
- Nome/colore della cartella
- Descrizione dell'immagine (caption)

### 2-2) File selezionati sul dispositivo

- File immagine selezionati dall'utente durante l'allegazione di foto
- File di backup `.knm` selezionati dall'utente durante l'importazione dei backup
- Percorsi di salvataggio e file salvati selezionati dall'utente durante l'esportazione di PDF/backup

### 2-3) Dati memorizzati localmente all'interno dell'app

I seguenti dati possono essere memorizzati sul dispositivo dell'utente al fine di fornire le funzionalità dell'app:

- Database SQLite (`people_note.db`): metadati relativi a persone/cartelle/piattaforme/siti/immagini
- File immagine: cifrati e memorizzati nella cartella documenti dell'app (`.enc`)
- Impostazioni dell'app (`SharedPreferences`): tema, ordinamento, opzioni privacy/pubblicità, opzioni di mascheramento PDF, criteri di blocco dell'app, ecc.
- Informazioni sul blocco dell'app: valori hash e salt per password/schemi (`SharedPreferences`)
- Chiavi di cifratura locali: memorizzate in `flutter_secure_storage`
- File temporanei: anteprime di decifratura immagini, file di cache di importazione/esportazione, ecc. (cartella temporanea)

### 2-4) Informazioni che possono essere trattate automaticamente durante la gestione della pubblicità e del consenso

Quando le funzionalità di pubblicità o di gestione del consenso sono abilitate, gli SDK di Google LLC e di partner correlati (come AdMob e UMP) possono trattare automaticamente le seguenti informazioni:

- Identificatori pubblicitari (AAID/IDFA, ecc.)
- Indirizzo IP e informazioni di rete
- Informazioni sul dispositivo (versione del sistema operativo, modello del dispositivo, versione dell'app, ecc.)
- Informazioni sulle interazioni con gli annunci (impressioni, clic, ecc.)
- Stato del consenso e informazioni sulle scelte in materia di privacy
- Informazioni relative a diagnostica, prestazioni e sicurezza

I dati principali dell'utente dell'app generalmente non vengono caricati sul server dello sviluppatore, ma alcune delle informazioni sopra indicate possono essere trasmesse a servizi di terze parti mentre sono in uso le funzionalità di pubblicità/consenso.

---

## 3. Finalità del Trattamento dei Dati Personali

L'app tratta dati personali o informazioni correlate per le seguenti finalità:

- Registrare e consultare informazioni relative a persone incentrate su contatti/note
- Fornire funzionalità organizzative come classificazione in cartelle, ricerca e unione
- Allegare e visualizzare foto
- Eseguire funzionalità richieste dall'utente, come backup/ripristino ed esportazione in PDF
- Fornire funzionalità di sicurezza per il blocco dell'app
- Fornire pubblicità, gestire il consenso, prevenire attività fraudolente e adempiere agli obblighi di legge

---

## 4. Periodo di Conservazione e Archiviazione dei Dati Personali

- Dati interni dell'app (SQLite, impostazioni locali, immagini cifrate): conservati sul dispositivo dell'utente fino a quando l'app non viene eliminata, i dati dell'app vengono cancellati oppure l'utente elimina direttamente i dati
- File temporanei: eliminati al termine dell'attività pertinente oppure cancellati in base alla politica di cache del sistema operativo
- File esportati dall'utente (PDF, file di backup): possono rimanere nella posizione di archiviazione selezionata dall'utente e devono essere eliminati direttamente dall'utente
- Dati relativi a pubblicità/consenso (trattati da terze parti): soggetti alle politiche di ciascun fornitore di servizi e alle leggi applicabili

In linea di principio, l'app non memorizza i dati principali dell'utente sul server dello sviluppatore.  
Tuttavia, i file che l'utente salva direttamente in una memoria esterna sono gestiti all'interno dell'ambiente dell'utente stesso.

---

## 5. Procedure e Metodi di Cancellazione dei Dati Personali

Quando la finalità del trattamento è stata raggiunta oppure quando l'utente richiede la cancellazione, l'app distrugge le informazioni pertinenti oppure le tratta in modo che non siano più riferibili, come segue.

### 5-1) Procedure di cancellazione

- Quando l'utente elimina direttamente singoli record di persone, cartelle, immagini, dati di backup, ecc., tali dati sono considerati soggetti a cancellazione immediata.
- Quando l'utente elimina l'app o cancella i dati dell'app dalle impostazioni del dispositivo, i dati memorizzati nell'area di archiviazione interna dell'app vengono rimossi secondo le procedure di cancellazione del sistema operativo.
- I file temporanei diventano soggetti a pulizia dopo il termine dell'attività pertinente e alcuni dati memorizzati nella cache possono rimanere fino a un certo momento in base alla politica del sistema operativo.

### 5-2) Metodi di cancellazione

- Dati SQLite: cancellazione dei record pertinenti
- Impostazioni dell'app (`SharedPreferences`): cancellazione della chiave pertinente o di tutte le impostazioni
- Valori di `flutter_secure_storage`: cancellazione dei pertinenti elementi di archiviazione sicura
- File interni dell'app (immagini cifrate, file temporanei, ecc.): cancellazione dei file pertinenti
- PDF/file di backup salvati direttamente dall'utente in una memoria esterna: non vengono eliminati automaticamente dall'app e devono essere eliminati direttamente dall'utente

Salvo ove diversamente richiesto dalle leggi applicabili, lo sviluppatore non memorizza separatamente i dati principali dell'utente sul server dello sviluppatore.

---

## 6. Comunicazione a Terzi, Affidamento del Trattamento e Trasferimento Transfrontaliero

L'app può utilizzare servizi di Google per la gestione della pubblicità e del consenso.

| Voce | Dettagli |
|---|---|
| **Destinatario / Responsabile del trattamento incaricato** | Google LLC e le sue affiliate (operatori di AdMob/UMP) |
| **Paese di trasferimento** | Stati Uniti e regioni in cui è gestita l'infrastruttura di Google |
| **Momento del trasferimento** | In modo continuativo durante richieste di annunci, verifiche dello stato del consenso, inizializzazione dell'SDK e funzionamento |
| **Metodo di trasferimento** | Trasmissione tramite comunicazione di rete tra l'app e i server di terze parti |
| **Base giuridica del trasferimento transfrontaliero** | Trattamento effettuato nell'ambito necessario per fornire il servizio sulla base delle basi giuridiche applicabili oppure, ove necessario, sulla base del consenso dell'interessato |
| **Finalità** | Erogazione di annunci, misurazione degli annunci, gestione del consenso, prevenzione delle frodi e conformità a politiche/leggi |
| **Categorie di dati (esempi)** | Identificatori pubblicitari (AAID/IDFA), informazioni IP/rete, informazioni su dispositivo/app, informazioni sulle interazioni con gli annunci, stato del consenso |
| **Periodo di conservazione** | Soggetto alle politiche di Google e alle leggi applicabili |
| **Effetti del rifiuto** | Gli annunci personalizzati possono essere limitati, possono essere mostrati annunci non personalizzati oppure alcune funzionalità relative agli annunci possono essere limitate |

Lo sviluppatore non raccoglie né vende i dati principali dei record relativi alle persone tramite un proprio server.

---

## 7. Informazioni sulle Autorizzazioni Utilizzate

L'app può utilizzare le seguenti autorizzazioni:

- `INTERNET`: comunicazione per SDK pubblicitari e relative funzionalità di rete
- `com.google.android.gms.permission.AD_ID`: utilizzo di identificatori pubblicitari (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 e versioni precedenti): allegare/selezionare foto

Le autorizzazioni sono utilizzate solo nell'ambito necessario a fornire le relative funzionalità.

---

## 8. Installazione, Funzionamento e Rifiuto dei Meccanismi di Raccolta Automatica

Questa app non utilizza direttamente cookie generali di siti web.  
Tuttavia, in relazione alle funzionalità di pubblicità e gestione del consenso, SDK di terze parti possono trattare automaticamente identificatori pubblicitari, informazioni di rete, informazioni sul dispositivo e dati simili.

Gli utenti possono modificare le impostazioni pertinenti nei seguenti modi:

- Modificare le scelte all'interno delle opzioni privacy dell'app o della schermata di gestione del consenso (ove disponibile)
- Reimpostare o eliminare l'identificatore pubblicitario nelle impostazioni del sistema operativo del dispositivo
- Limitare gli annunci personalizzati o modificare le relative opzioni sulla privacy nelle impostazioni del sistema operativo del dispositivo

Se l'utente limita la pubblicità personalizzata, possono essere mostrati annunci non personalizzati oppure alcune funzionalità relative agli annunci possono essere limitate.

---

## 9. Diritti dell'Utente e Modalità di Esercizio

Fatte salve le leggi applicabili, gli utenti possono avere i seguenti diritti:

- Richiedere l'accesso, la rettifica o la cancellazione dei dati personali
- Richiedere la sospensione o la limitazione del trattamento
- Revocare il consenso per il trattamento basato sul consenso
- Modificare le scelte relative a pubblicità/consenso

Tali diritti possono essere esercitati nei seguenti modi:

- Modificare o eliminare direttamente i dati all'interno dell'app
- Inizializzare i dati locali eliminando i dati dell'app o disinstallando l'app
- Modificare il consenso alla pubblicità tramite le opzioni privacy/schermata di consenso dell'app (nelle regioni in cui è disponibile)
- Reimpostare/eliminare l'identificatore pubblicitario oppure limitare gli annunci personalizzati tramite le impostazioni del sistema operativo del dispositivo
- Contatto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Misure di Sicurezza

Lo sviluppatore applica o si impegna ad applicare le seguenti misure:

- I dati dell'utente sono generalmente memorizzati localmente sul dispositivo
- I file immagine allegati sono memorizzati localmente in forma cifrata (basata su AES-GCM)
- Le informazioni sul blocco dell'app sono memorizzate in forma hash e non in testo semplice
- I file di backup vengono memorizzati dopo essere stati cifrati sulla base di una password dell'utente
- La comunicazione con SDK di terze parti è cifrata (HTTPS/TLS)
- Le autorizzazioni sono utilizzate con un ambito di accesso minimo

Tuttavia, i rischi derivanti dallo stato di sicurezza del dispositivo dell'utente (come root/jailbreak, app dannose o esposizione di memoria condivisa) non possono essere completamente eliminati.

---

## 11. Informazioni Relative ai Dati Sensibili

Questa app non richiede l'inserimento di dati sensibili.  
Si consiglia agli utenti di non inserire contenuti sensibili, come informazioni sanitarie, opinioni politiche, religione, informazioni biometriche o informazioni relative alla vita sessuale, nelle note o nei campi di inserimento libero.

Se un utente inserisce volontariamente contenuti sensibili, tali informazioni possono essere memorizzate come dati locali sul dispositivo gestito direttamente dall'utente.

---

## 12. Protezione dei Dati Personali dei Minori

Questa app non è progettata principalmente per i minori.  
I tutori possono gestire l'utilizzo tramite le funzionalità di controllo parentale fornite dal dispositivo o dallo store delle app.

---

## 13. Processo Decisionale Automatizzato

Questa app non effettua processi decisionali automatizzati basati su dati personali che producano effetti giuridici o impatti significativi analoghi.

---

## 14. Avviso sulla Sicurezza dei Dati (Google Play, ecc.)

Lo sviluppatore si impegna a mantenere e aggiornare gli elementi di divulgazione relativi alla sicurezza dei dati negli store di app (come Google Play) in conformità alle effettive pratiche di trattamento dell'app e alle effettive pratiche di trattamento degli SDK di terze parti.

Tuttavia, le informazioni mostrate negli store di app possono variare a seconda della versione dell'app, del Paese di distribuzione, della configurazione degli SDK di terze parti e delle modifiche alle politiche.

---

## 15. Avviso Open Source

L'app utilizza determinate librerie open source.  
Le informazioni sulle relative licenze possono essere trovate nella schermata pertinente all'interno dell'app oppure negli avvisi forniti tramite il canale di distribuzione.

---

## 16. Contatti

Per richieste relative alla presente Informativa sulla Privacy:

- **Responsabile della protezione dei dati / Referente:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 17. Modifiche alla presente Informativa sulla Privacy

La presente Informativa può essere rivista a causa di modifiche a leggi/politiche, funzionalità dell'app o SDK di terze parti.  
In caso di modifiche sostanziali, potrà essere fornito un avviso tramite notifiche all'interno dell'app, la pagina di distribuzione oppure aggiornamenti della pagina dell'informativa.

Ultimo aggiornamento: **2026-03-04**
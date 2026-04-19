---
title: Informativa sulla privacy | QDiary
description: Informativa sulla privacy di QDiary
---

# Informativa sulla privacy (QDiary)

- Nome dell'app: QDiary
- Sviluppatore: frog-im
- Contatto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Data di entrata in vigore: 2026-04-19
- Ultimo aggiornamento: 2026-04-19

La presente Informativa sulla privacy è redatta sulla base dell'implementazione attuale dell'app QDiary. QDiary fornisce funzionalità di scrittura del diario, generazione e riflessione sulle quest, accesso, salvataggio manuale sul cloud, pubblicità e notifiche e, in tale contesto, può trattare dati personali o informazioni che possono costituire dati personali nella misura necessaria.

## 1. Funzionalità fornite

QDiary fornisce le seguenti funzionalità:

- Scrittura, modifica e visualizzazione diari
- Classificazione per categoria e visualizzazione calendario
- Generazione di quest, riflessione sulle quest e gestione del completamento delle quest
- Blocco locale dell'app diario e crittografia locale
- Accesso tramite e-mail, verifica dell'e-mail, accesso anonimo (ospite) e reimpostazione della password
- Salvataggio e caricamento sul cloud avviati dall'utente
- Visualizzazione di annunci e gestione delle opzioni privacy relative agli annunci
- Notifiche promemoria delle quest

## 2. Categorie di informazioni trattate

### 2-1. Informazioni inserite direttamente dall'utente

- Indirizzo e-mail
- Password
- Titolo del diario, contenuto, data, categoria e difficoltà
- Risposte alle quest, contenuti di riflessione e informazioni sulla quest selezionata
- Valori selezionati relativi al profilo delle quest e testo di riepilogo
- Frase segreta per il blocco dell'app diario

### 2-2. Informazioni memorizzate dall'app sul dispositivo

- Database locale del diario (SQLite)
- Informazioni sullo stato delle quest per i diari locali
- Valori di stato relativi a presenza, impostazioni, lingua, notifiche e annunci
- Valori di verifica del blocco dell'app, salt e metadati di crittografia
- Informazioni sulla pianificazione delle notifiche delle quest

### 2-3. Informazioni sull'account e sull'identificazione

Le seguenti informazioni possono essere trattate tramite Firebase Authentication:

- UID Firebase
- Indirizzo e-mail
- Stato della verifica dell'e-mail
- Stato dell'accesso anonimo

### 2-4. Informazioni relative a pubblicità e consenso

Quando si utilizzano Google AdMob e l'SDK UMP, possono essere trattate le seguenti informazioni:

- Identificatori pubblicitari (come Android AD_ID)
- Indirizzo IP e informazioni di rete
- Informazioni sul dispositivo, versione del sistema operativo e informazioni sull'app
- Informazioni su impressioni pubblicitarie, clic e gestione delle ricompense
- Stato del consenso pubblicitario e stato delle opzioni privacy

### 2-5. Informazioni relative alle notifiche

- Stato dell'autorizzazione alle notifiche
- Valori identificativi dei diari che contengono quest in corso
- Testo della notifica della quest
- Orari programmati delle notifiche

## 3. Finalità del trattamento

L'app tratta le informazioni per le seguenti finalità:

- Registrazione, accesso, verifica dell'e-mail e reimpostazione della password
- Scrittura, salvataggio e visualizzazione dei diari
- Generazione delle quest, riflessione e determinazione del completamento
- Crittografia e decrittografia locali associate al blocco dell'app
- Salvataggio e caricamento sul cloud richiesti dall'utente
- Fornitura di notifiche delle quest
- Fornitura di annunci, gestione delle ricompense pubblicitarie e applicazione dello stato del consenso pubblicitario
- Sicurezza, gestione degli errori e funzionamento del servizio

## 4. Archiviazione locale, archiviazione cloud e trattamento esterno

### 4-1. Archiviazione locale

Le informazioni del diario e delle quest sono memorizzate principalmente nel database locale del dispositivo.

- Se il blocco dell'app non è attivato: archiviazione locale in forma generale
- Se il blocco dell'app è attivato: alcune informazioni, come il titolo del diario, il contenuto e lo stato delle quest, possono essere crittografate e memorizzate localmente

### 4-2. Archiviazione cloud

L'app memorizza i dati in Firebase Firestore solo quando l'utente esegue direttamente la funzione `Save`.

Secondo la configurazione attuale del progetto:

- Non viene utilizzata la sincronizzazione automatica completa
- I dati vengono memorizzati in Firestore `savedDiaries` solo quando l'utente li salva manualmente
- Al momento del salvataggio, il titolo del diario, il contenuto e lo stato delle quest possono essere memorizzati in forma crittografata a seconda dello stato attuale del blocco dell'app
- I dati vengono ricaricati nell'archiviazione locale solo quando l'utente esegue `Load`

### 4-3. Trattamento esterno per la generazione e la riflessione sulle quest

Quando l'utente richiede la generazione di una quest o una riflessione, le seguenti informazioni possono essere utilizzate per un trattamento esterno tramite Firebase Functions:

- Titolo del diario
- Contenuto del diario o contenuto della riflessione
- Categoria
- Difficoltà
- Quest selezionata
- Informazioni di riepilogo del profilo della quest

Queste informazioni vengono utilizzate per la generazione e la valutazione delle quest tramite l'API di OpenAI.

Importante:

- I contenuti del diario pertinenti vengono utilizzati per il trattamento esterno solo quando viene utilizzata la funzionalità quest.
- Secondo la configurazione attuale del progetto, non viene utilizzato alcun codice che memorizzi i log delle quest in una raccolta separata `questLogs`.

## 5. Servizi di terze parti e trattamento affidato a terzi

### 5-1. Google Firebase

Finalità:

- Autenticazione (Firebase Authentication)
- Archiviazione Firestore
- Esecuzione di Cloud Functions

Informazioni che possono essere trattate:

- UID, indirizzo e-mail e stato di autenticazione
- Dati del diario salvati manualmente dall'utente
- Dati delle richieste di quest

### 5-2. OpenAI

Finalità:

- Generazione di quest
- Riflessione sulle quest e valutazione del completamento

Informazioni che possono essere trattate:

- Titolo/contenuto del diario
- Testo della quest
- Difficoltà e categoria
- Contenuto della riflessione inserito dall'utente
- Informazioni di riepilogo del profilo della quest

### 5-3. Google AdMob / UMP

Finalità:

- Fornitura di annunci banner, interstitial e con ricompensa
- Gestione del consenso pubblicitario e delle opzioni privacy

Informazioni che possono essere trattate:

- Identificatori pubblicitari
- Informazioni sul dispositivo e sulla rete
- Informazioni sulle interazioni con gli annunci
- Stato del consenso

## 6. Avviso sul trasferimento internazionale

L'app può trattare dati personali o informazioni correlate al di fuori del Paese dell'utente nei seguenti casi:

| Voce | Dettagli |
|---|---|
| Destinatari | Google LLC, OpenAI e operatori di infrastrutture correlati |
| Paese di destinazione | Stati Uniti, ecc. |
| Momento del trasferimento | Durante l'accesso, la generazione/riflessione sulle quest, le richieste pubblicitarie e il trattamento del consenso |
| Metodo di trasferimento | Comunicazione di rete crittografata |
| Finalità del trasferimento | Autenticazione, archiviazione dati, elaborazione serverless, generazione/valutazione di quest tramite IA e fornitura di pubblicità |

## 7. Periodo di conservazione e utilizzo

L'app conserva le informazioni secondo i seguenti criteri:

- Informazioni locali del diario/impostazioni: fino a quando l'utente le elimina o disinstalla l'app
- Informazioni sull'account Firebase: finché l'utente mantiene l'account
- Dati memorizzati in Firestore: finché l'utente conserva gli elementi salvati
- Dati di elaborazione delle richieste di quest: nella misura necessaria per l'elaborazione serverless
- Dati relativi a pubblicità/consenso: secondo le politiche di ciascun fornitore esterno

Inoltre, il progetto attuale include la seguente logica di pulizia automatica:

- Pulizia degli account utente anonimi e dei dati Firestore delle sottocollezioni utente dopo un determinato periodo
- Pulizia degli account utente regolari inattivi da lungo tempo e dei dati Firestore delle sottocollezioni utente

Tuttavia, l'effettiva applicazione di ciò nell'ambiente di produzione può variare a seconda dello stato di distribuzione e della configurazione del server.

## 8. Avviso sul blocco dell'app e sulla crittografia locale

L'app fornisce una funzione separata `Diary App Lock`.

- La frase segreta del blocco dell'app è separata dalla password dell'account.
- La frase segreta del blocco dell'app viene utilizzata per la crittografia e la decrittografia locale del diario.
- Anche se viene inserita una frase segreta errata, l'app stessa potrebbe non essere sempre completamente bloccata; invece, alcuni contenuti del diario potrebbero rimanere illeggibili.
- Alcuni diari possono essere crittografati separatamente in base alla frase segreta utilizzata al momento della scrittura o dello sblocco temporaneo.

Gli utenti devono conservare la propria frase segreta in modo sicuro e, in caso di smarrimento, il recupero di alcuni dati locali potrebbe risultare difficile.

## 9. Avviso sulle notifiche delle quest

Se l'utente abilita le notifiche delle quest, possono essere programmate notifiche locali per ciascun diario con una quest in corso.

- La pianificazione viene gestita principalmente tramite il sistema di pianificazione interno del dispositivo.
- Secondo la configurazione attuale del progetto, non è stata confermata alcuna struttura in cui il testo originale del diario venga trasmesso periodicamente a un server centrale esclusivamente per finalità di notifica.

## 10. Avviso sull'uso delle autorizzazioni

L'app può utilizzare le seguenti autorizzazioni per fornire le proprie funzionalità:

- `INTERNET`: comunicazione con Firebase, OpenAI e SDK pubblicitari
- `com.google.android.gms.permission.AD_ID`: utilizzo degli identificatori pubblicitari
- `POST_NOTIFICATIONS`: visualizzazione delle notifiche delle quest
- `RECEIVE_BOOT_COMPLETED`: ripristino delle notifiche programmate dopo il riavvio del dispositivo

Le autorizzazioni vengono utilizzate solo nella misura necessaria per eseguire le relative funzionalità.

## 11. Diritti dell'interessato e modalità di esercizio

Gli utenti possono esercitare i seguenti diritti:

- Accedere, modificare ed eliminare i dati all'interno dell'app
- Eliminare o sovrascrivere i dati memorizzati nel cloud
- Richiedere la disconnessione e l'eliminazione dell'account
- Modificare le opzioni privacy relative alla pubblicità
- Disattivare le autorizzazioni alle notifiche

Modalità di esercizio di tali diritti:

- Eliminare o modificare direttamente i diari all'interno dell'app
- Eliminare l'app o reimpostare i dati locali
- Disconnettersi dall'account e richiedere separatamente l'eliminazione
- Modificare notifiche, identificatori pubblicitari e autorizzazioni nelle impostazioni del dispositivo
- E-mail di contatto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Misure di sicurezza

L'app applica o può applicare le seguenti misure di protezione:

- Comunicazione basata su HTTPS
- Blocco e crittografia locale dell'app diario
- Memorizzazione separata dei valori di verifica della frase segreta
- Utilizzo di Firebase Authentication
- Richiesta delle autorizzazioni minime necessarie

Tuttavia, possono insorgere rischi a seconda dello stato di sicurezza del dispositivo dell'utente, come rooting, jailbreak, malware o utilizzo di un dispositivo condiviso.

## 13. Dati personali dei minori

L'app non è progettata come un servizio destinato principalmente ai minori. Tuttavia, durante il trattamento di annunci/consenso possono essere applicate opzioni relative all'età all'interno di UMP.

## 14. Modifiche alla presente informativa

La presente Informativa può essere modificata in caso di cambiamenti normativi, dei servizi di terze parti o delle funzionalità dell'app.

- Ultimo aggiornamento per la versione attuale: **2026-04-19**

## 15. Contatti

- Sviluppatore: frog-im
- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)


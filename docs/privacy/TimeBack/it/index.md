---
title: Informativa sulla Privacy | TimeBack
description: Informativa sulla privacy di TimeBack
lang: it
last_updated: 2026-06-06
---

# Informativa sulla privacy (TimeBack)

- **Nome dell'app:** TimeBack
- **Sviluppatore:** frog-im
- **Contatto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data di entrata in vigore:** 03-06-2026
- **Ultimo aggiornamento:** 2026-06-06

La presente Informativa sulla privacy si basa sull'attuale implementazione dell'app TimeBack. TimeBack fornisce la revisione del tempo di utilizzo, gli obiettivi giornalieri, i record del tempo recuperato, le riflessioni, le sfide, le notifiche, la condivisione e le funzionalità pubblicitarie.

## 1. Caratteristiche

TimeBack fornisce le seguenti funzionalità:

- Revisione del tempo di utilizzo dell'app tramite l'autorizzazione di accesso all'utilizzo di Android
- Obiettivi di utilizzo quotidiano, promemoria e notifiche di utilizzo sulla barra di stato
- Notifiche di avviso con limiti rigidi e visualizzazione in sovrapposizione
- Selezione dell'app per eccezioni sovrapposte
- Registrazioni delle attività in tempo recuperato
- Registri della riflessione quotidiana
- Progresso della sfida e gestione della checklist
- Condivisione di immagini relative alle statistiche di utilizzo
- Annunci Google AdMob e opzioni sulla privacy basate su UMP

## 2. Informazioni che elaboriamo

### 2-1. Autorizzazione di accesso all'utilizzo in lettura delle informazioni

Se l'utente concede l'autorizzazione `PACKAGE_USAGE_STATS` ad Android, l'app potrebbe leggere le seguenti informazioni dal dispositivo:

- Nome del pacchetto dell'app
- Nome dell'app
- Tempo di utilizzo dell'app
- Intervallo di data e ora utilizzato per l'aggregazione dell'utilizzo

Queste informazioni vengono utilizzate per fornire statistiche sull'utilizzo e confrontare l'utilizzo con gli obiettivi dell'utente.

### 2-2. Informazioni immesse o configurate dall'utente

- Obiettivo di utilizzo quotidiano
- Stato e intervallo di attivazione del promemoria di utilizzo
- Impostazione della visualizzazione dell'utilizzo della barra di stato
- Categoria, titolo, ora di inizio e durata dell'attività di tempo recuperato
- Testo di riflessione quotidiana
- Progressi della sfida e voci della lista di controllo
- Elenco delle app per le eccezioni sovrapposte

### 2-3. Informazioni archiviate sul dispositivo

L'app può memorizzare le seguenti informazioni in un database SQLite locale o in SharedPreferences:

- Record del tempo di utilizzo dell'app
- Obiettivi e impostazioni giornalieri
- Registrazioni delle attività in tempo recuperato
- Registri della riflessione quotidiana
- Progresso della sfida e stato della lista di controllo
- Stato di completamento dell'onboarding
- Impostazioni come promemoria sull'utilizzo, avvisi di limiti rigidi, visualizzazione della barra di stato e app per eccezioni in sovrapposizione
- Consenso degli annunci locali e stato dell'opzione sulla privacy

In base all'implementazione attuale, questi record locali non vengono caricati automaticamente sui server frog-im.

### 2-4. Dati pubblicitari e di consenso

Quando vengono utilizzati gli annunci per dispositivi mobili di Google SDK (AdMob) e UMP, Google o le sue società affiliate possono elaborare informazioni quali:

- Identificatori pubblicitari, come Android AD_ID
- Indirizzo IP e informazioni sulla rete
- Informazioni sul dispositivo, versione OS e informazioni sull'app
- Impressioni degli annunci, clic, dati di misurazione e segnali di errore
- Consenso agli annunci e stato dell'opzione privacy
- Posizione approssimativa

## 3. Finalità del trattamento

L'app elabora le informazioni per i seguenti scopi:

- Lettura del tempo di utilizzo, visualizzazione delle statistiche e confronto dell'utilizzo con gli obiettivi
- Memorizzazione dei record di tempo recuperato e di riflessione immessi dall'utente
- Gestire l'avanzamento della sfida
- Fornire promemoria e notifiche sulla barra di stato
- Fornire notifiche di avviso di limiti rigidi, visualizzazione in sovrapposizione e gestione delle eccezioni in sovrapposizione
- Condivisione di immagini delle statistiche di utilizzo quando richiesto dall'utente
- Pubblicazione di annunci, misurazione del rendimento degli annunci e applicazione delle scelte di consenso degli annunci
- Mantenere la stabilità dell'app e rispondere agli errori

## 4. Archiviazione locale ed elaborazione esterna

### 4-1. Archiviazione locale

TimeBack memorizza i dati dell'utente principalmente nella memoria interna dell'app sul dispositivo. In base all'attuale implementazione, i record di utilizzo, gli obiettivi, le riflessioni e le informazioni sulle sfide non vengono caricati automaticamente sui server frog-im.

L'archiviazione locale può includere quanto segue.

| Magazzinaggio | Oggetti immagazzinati | Scopo | Metodo di cancellazione |
|---|---|---|---|
| SQLite database | Record di utilizzo delle app, nomi dei pacchetti, nomi delle app, tempo di utilizzo, aggregati basati sulla data | Mostra statistiche sull'utilizzo e confronta l'utilizzo con gli obiettivi | Funzionalità di eliminazione in-app, cancellazione dei dati dell'app o disinstallazione dell'app |
| SQLite database | Attività per il tempo recuperato, riflessioni, progressi della sfida, voci della checklist | Mostra i record e gestisci i progressi | Funzionalità di eliminazione in-app, cancellazione dei dati dell'app o disinstallazione dell'app |
| Preferenze condivise | Stato di completamento dell'onboarding, impostazioni dei promemoria, impostazioni degli avvisi sui limiti rigidi, impostazioni di visualizzazione della barra di stato, elenco delle app con eccezioni di overlay, stato del consenso degli annunci locali | Mantieni le impostazioni dell'app | Cancellazione dei dati dell'app o disinstallazione dell'app |
| File temporanei/cache | Immagini condivise delle statistiche di utilizzo e file temporanei simili | Eseguire la condivisione richiesta dall'utente | Eliminato dopo la condivisione, ove possibile, o in base ai criteri di pulizia OS/app |

Quando l'utente cancella i dati dell'app o disinstalla l'app, i dati archiviati nella memoria interna dell'app vengono generalmente eliminati. Tuttavia, il backup Android, il backup del produttore, il backup su cloud o i file condivisi direttamente dall'utente potrebbero essere conservati separatamente in base alle politiche di tali servizi.

Le registrazioni dell'utilizzo e il testo di riflessione possono rivelare routine o interessi personali. Sui dispositivi condivisi, gli utenti devono utilizzare misure di sicurezza adeguate come il blocco del dispositivo o account OS separati.

### 4-2. Caricamenti del server

In base al progetto attuale, TimeBack non carica automaticamente record di utilizzo, riflessioni o record di sfide sui server frog-im. Se l'utente utilizza la funzione di condivisione, un'immagine statistica generata potrebbe essere trasferita all'app o al servizio esterno selezionato dall'utente.

### 4-3. Elaborazione pubblicitaria

Google AdMob e UMP vengono utilizzati per la pubblicità in-app e la gestione del consenso. Le informazioni relative alla pubblicità potrebbero essere elaborate sull'infrastruttura di Google.

## 5. Servizi e processori di terze parti

### 5-1. Google AdMob/UMP

Scopo:

- Pubblicazione di banner pubblicitari
- Consenso degli annunci e gestione delle opzioni sulla privacy
- Misurazione delle prestazioni degli annunci e prevenzione delle frodi

Informazioni che potranno essere trattate:

- Identificatori pubblicitari
- Informazioni sul dispositivo e sulla rete
- Informazioni sull'interazione con gli annunci
- Stato del consenso e dell'opzione privacy

### 5-2. Condivisione di app o servizi di destinazione

Se l'utente utilizza direttamente la funzionalità di condivisione delle immagini delle statistiche di utilizzo, l'app o il servizio esterno selezionato potrebbe elaborare l'immagine condivisa. Tale trattamento è regolato dalla privacy policy del servizio selezionato.

## 6. Avviso di trasferimento transfrontaliero

I dati potrebbero essere trattati al di fuori del Paese dell'utente nei seguenti casi.

| Articolo | Dettagli |
|---|---|
| Destinatario | Google LLC e le sue affiliate |
| Destinazione | Stati Uniti e altri paesi/regioni in cui si trova l'infrastruttura di Google |
| Tempistica | Quando l'app viene eseguita, richiede annunci, mostra o misura annunci, elabora i clic o gestisce il consenso |
| Metodo | Comunicazione di rete crittografata (HTTPS/TLS) |
| Scopo | Pubblicazione di annunci, gestione dello stato di personalizzazione, misurazione, analisi, miglioramento della stabilità del servizio, conformità legale |
| Dati | Identificatori pubblicitari, informazioni su dispositivo/app/rete, informazioni sull'interazione degli annunci, stato del consenso, posizione approssimativa, ecc. |
| Conservazione | In conformità con le politiche di Google e la legge applicabile |

Per i dettagli, consultare [Cross-Border Transfer Notice](./policy/).

## 7. Elenco delle app installate ed eccezioni di sovrapposizione

Su Android, se l'utente configura app per eccezioni di sovrapposizione, l'app può leggere i nomi dei pacchetti e i nomi delle app avviabili sul dispositivo per visualizzare un elenco di selezione. I nomi dei pacchetti selezionati dall'utente come eccezioni vengono archiviati in SharedPreferences sul dispositivo e vengono utilizzati solo per evitare di mostrare sovrapposizioni di avvisi di limiti rigidi su tali app.

## 8. Conservazione

L'app conserva le informazioni secondo i seguenti standard:

- Informazioni su utilizzo locale, obiettivo, riflessione e sfida: finché l'utente non lo elimina, cancella i dati dell'app o disinstalla l'app
- Impostazioni SharedPreferences: finché l'utente non cancella i dati dell'app o non disinstalla l'app
- File temporanei per immagini condivise: secondo necessità per la condivisione o secondo i criteri di pulizia OS
- Dati pubblicitari e relativi al consenso: secondo le politiche di Google e di altre terze parti pertinenti

## 9. Autorizzazioni

L'app può utilizzare le seguenti autorizzazioni:

- `PACKAGE_USAGE_STATS`: leggi il tempo di utilizzo dell'app
- `POST_NOTIFICATIONS`: mostra promemoria sull'utilizzo e notifiche sulla barra di stato
- `SYSTEM_ALERT_WINDOW`: mostra sovrapposizioni di avvisi sui limiti rigidi
- `INTERNET`: comunica con l'annuncio SDKs e mostra le pagine delle note legali
- `ACCESS_NETWORK_STATE`: controlla lo stato della rete
- `com.google.android.gms.permission.AD_ID`: utilizza identificatori pubblicitari

Le autorizzazioni vengono utilizzate solo se necessarie per le funzionalità dell'app. Gli utenti possono revocare le autorizzazioni nelle impostazioni del dispositivo, ma le funzionalità correlate potrebbero essere limitate.

## 10. Diritti e scelte dell'utente

Gli utenti possono:

- Visualizza, modifica o elimina i record all'interno dell'app
- Elimina le informazioni locali cancellando i dati dell'app o disinstallando l'app
- Modifica le impostazioni di accesso all'utilizzo, notifica e identificatore pubblicitario nelle impostazioni del dispositivo
- Revoca l'autorizzazione dell'overlay e modifica le impostazioni dell'app per le eccezioni dell'overlay
- Modifica le opzioni sulla privacy degli annunci
- Contattaci per domande sulla privacy o richieste di cancellazione

E-mail di contatto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Misure di sicurezza

L'app applica o può applicare le seguenti garanzie:

- Comunicazione esterna basata su HTTPS/TLS
- Elaborazione dei dati local-first
- Richieste di autorizzazione minime necessarie per le funzionalità dell'app
- Applicazione dello stato di consenso alla pubblicità

Condizioni di sicurezza del dispositivo come rooting, jailbreak, malware o utilizzo di dispositivi condivisi possono creare ulteriori rischi.

## 12. Privacy dei bambini

TimeBack non è progettato principalmente per i bambini. Durante l'elaborazione della pubblicità e del consenso potrebbero essere applicate le impostazioni relative all'età o le norme della piattaforma di Google Mobile Ads SDK e UMP.

## 13. Modifiche

La presente Politica potrebbe essere aggiornata a causa di modifiche legislative, configurazione di servizi di terze parti o funzionalità dell'app. Le modifiche sostanziali verranno comunicate tramite avviso in-app o aggiornando questa pagina.

## 14. Contatto

- Sviluppatore: frog-im
- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

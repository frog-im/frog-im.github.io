---
title: Informativa sulla privacy | Subtitle Tool
description: Informativa sulla privacy di Subtitle Tool (Subtitle Player & Editor) - Italiano
lang: it
last_updated: 2026-03-11
---

# Informativa sulla privacy (Subtitle Tool / Subtitle Player & Editor)

- **Nome dell’app:** Subtitle Player & Editor (indicato anche come **Subtitle Tool** nella presente Informativa)
- **Sviluppatore:** frog-im
- **Contatto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data di entrata in vigore:** 2026-03-11

> La presente Informativa è redatta con riferimento alle leggi applicabili, tra cui il Korean Personal Information Protection Act (PIPA), il GDPR / UK GDPR, la Swiss FADP e le pertinenti leggi statali sulla privacy degli Stati Uniti. Se si applicano norme locali obbligatorie, tali norme prevalgono.

---

## 1. Finalità e ambito di applicazione

Questa app offre:

- riproduzione e modifica dei sottotitoli
- riproduzione di video + sottotitoli da file selezionati dall’utente
- overlay flottante di sottotitoli / testi mostrato sopra altre app su Android

La gestione dei sottotitoli supportata può includere formati quali:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

L’app **non** crea un account utente e **non** carica i file di sottotitoli o multimediali dell’utente sui server del sviluppatore. Il parsing, la modifica, l’anteprima dei sottotitoli e la maggior parte dell’elaborazione relativa alla riproduzione vengono eseguiti **localmente sul dispositivo**.

Tuttavia, per finalità pubblicitarie, gestione del consenso e conformità legale, SDK di terze parti come **Google Mobile Ads SDK (AdMob)** e **Google UMP** possono trattare alcune informazioni, come identificatori pubblicitari, segnali del dispositivo e scelte di consenso.

---

## 2. Categorie di informazioni che trattiamo

### 2-1) File selezionati esplicitamente dall’utente

L’app interagisce con i file selezionati esplicitamente dall’utente, tra cui:

- **File di sottotitoli**
  - Esempi: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Utilizzi:
    - riproduzione dei sottotitoli all’interno dell’app
    - modifica dei sottotitoli
    - visualizzazione dei sottotitoli in overlay
    - conversione ed esportazione dei sottotitoli

- **File multimediali**
  - Esempi: file video o audio locali scelti dall’utente
  - Utilizzi:
    - riproduzione video + sottotitoli
    - allineamento temporale dell’overlay con il contenuto multimediale attualmente in riproduzione

Punti importanti:

- I file selezionati dall’utente vengono elaborati localmente sul dispositivo.
- L’app non carica tali file sui server del sviluppatore.
- I percorsi e i contenuti dei file vengono utilizzati solo per riproduzione, overlay, modifica, salvataggio e azioni richieste dall’utente.

### 2-2) Impostazioni locali e valori memorizzati

Per fornire impostazioni persistenti e ripristinare lo stato precedente, l’app memorizza alcuni valori localmente sul dispositivo utilizzando `SharedPreferences` o un analogo archivio locale fornito dal sistema operativo.

Tali valori non vengono inviati ai server del sviluppatore e vengono normalmente rimossi se i dati dell’app vengono cancellati o se l’app viene disinstallata.

#### (1) Impostazioni dell’overlay

Gli esempi includono:

- `overlay_box_x`
- `overlay_box_y`
- `overlay_text_font`
- `overlay_text_color`
- `overlay_outline_enabled`
- `overlay_outline_color`
- `overlay_outline_width`
- `overlay_force_landscape`
- `overlay_interstitial_count`

Finalità:

- ripristinare la posizione dell’overlay
- ripristinare lo stile dei sottotitoli per l’overlay e per la riproduzione dei sottotitoli nell’app
- mantenere le preferenze relative a contorno / carattere / orientamento
- controllare la logica della frequenza di visualizzazione degli annunci in alcuni flussi correlati all’overlay

#### (2) Posizioni recenti di riproduzione o overlay

Gli esempi includono:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Finalità:

- ripristinare o suggerire recenti posizioni iniziali di sottotitoli/overlay
- riprendere più comodamente la riproduzione video + sottotitoli

#### (3) Valori di preferenza relativi ad annunci e privacy

Gli esempi possono includere:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Finalità:

- memorizzare le scelte di privacy relative agli annunci
- applicare le impostazioni di privacy e configurazione pubblicitaria di UMP / AdMob

#### (4) Output di sottotitoli creati dall’utente

Quando l’utente salva o esporta file di sottotitoli, l’app può scrivere nuovi file di sottotitoli in una posizione selezionata dall’utente, ad esempio:

- Download
- un’altra cartella selezionata tramite un selettore di sistema
- una posizione di archiviazione gestita dall’utente

Questi file salvati dall’utente possono rimanere sul dispositivo dopo l’eliminazione dell’app, a meno che l’utente non li elimini manualmente.

#### (5) File temporanei e cache

L’app e le librerie di terze parti possono creare file temporanei o di cache per il normale funzionamento, come:

- dati di cache del file picker
- dati temporanei di conversione dei sottotitoli
- dati di cache relativi alla riproduzione

Questi sono destinati esclusivamente al funzionamento locale e non vengono caricati sui server del sviluppatore.

#### (6) Cache dello stato di consenso UMP

Nelle regioni in cui si applica Google UMP, l’SDK può memorizzare localmente sul dispositivo lo stato del consenso.

Generalmente questo può essere reimpostato mediante:

- cancellazione dei dati dell’app, oppure
- modifica delle scelte di consenso all’interno dell’app, ove sia disponibile una voce relativa alle opzioni sulla privacy

### 2-3) Elaborazione relativa all’overlay Android e ai permessi

Su Android, l’overlay flottante dei sottotitoli può utilizzare:

- il permesso `SYSTEM_ALERT_WINDOW` / visualizzazione sopra altre app
- il permesso `POST_NOTIFICATIONS`
- una notifica di servizio in primo piano richiesta per il servizio overlay

Finalità:

- mostrare l’overlay dei sottotitoli sopra altre app
- mantenere in esecuzione il servizio overlay
- consentire ad Android di mostrare le notifiche necessarie per overlay / servizio
- leggere le informazioni delle notifiche multimediali quando necessario per supportare la progressione dei sottotitoli

Questi permessi vengono utilizzati solo per le funzionalità dell’app che l’utente sceglie di usare.

### 2-4) Annunci, consenso e dati correlati (SDK di terze parti)

L’app utilizza SDK Google per annunci / consenso, tra cui:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

L’app può mostrare:

- banner pubblicitari
- annunci interstiziali
- annunci con ricompensa o interstiziali con ricompensa

Questi SDK possono trattare dati come:

- identificatori pubblicitari (ad esempio AAID / IDFA, ove applicabile)
- informazioni basate su IP e relative alla rete
- metadati del dispositivo e dell’app
- segnali di interazione con gli annunci
- scelte di consenso

Le finalità possono includere:

- erogazione degli annunci
- misurazione e reportistica pubblicitaria
- limitazione della frequenza
- prevenzione delle frodi
- conformità legale

Lo sviluppatore si impegna a configurare tali SDK in modo coerente con le scelte di consenso dell’utente e con la legge applicabile.

---

## 3. Come trattiamo e conserviamo i dati

- **Impostazioni locali e dati relativi a posizioni recenti**
  - conservati sul dispositivo fino a quando i dati dell’app non vengono cancellati o l’app non viene rimossa

- **File temporanei / cache**
  - conservati solo per il tempo necessario al funzionamento, quindi rimossi dall’app ove praticabile o successivamente puliti dal sistema operativo

- **File di sottotitoli salvati dall’utente**
  - rimangono nella posizione di salvataggio scelta dall’utente finché l’utente non li elimina

- **Dati pubblicitari / di consenso gestiti da terze parti**
  - conservati secondo le politiche di Google e la legge applicabile

---

## 4. Trattamento da parte di terzi e trasferimenti transfrontalieri

Per annunci e gestione del consenso, alcune informazioni possono essere trattate da Google e dai partner correlati.

| Voce | Dettagli |
|---|---|
| Destinatario | Google LLC e affiliate / responsabili del trattamento correlati |
| Finalità | Erogazione degli annunci, misurazione, prevenzione delle frodi, gestione del consenso e conformità legale |
| Possibili dati | Identificatori pubblicitari, informazioni su dispositivo/app, informazioni basate su IP, dati di interazione con gli annunci, stato del consenso |
| Destinazione | Stati Uniti e altre regioni in cui opera l’infrastruttura di Google |
| Conservazione | Secondo le politiche di Google e la legge applicabile |

Lo sviluppatore si impegna a mantenere le informative sulla privacy negli store coerenti con il comportamento effettivo degli SDK.

---

## 5. I tuoi diritti e le tue scelte

A seconda della tua giurisdizione, potresti avere diritti quali:

- accesso
- rettifica
- cancellazione
- limitazione
- portabilità
- opposizione
- revoca del consenso laddove il consenso costituisca la base giuridica

I controlli pratici includono:

- modifica delle scelte relative ad annunci / privacy nell’app, ove disponibili
- cancellazione dei dati dell’app per rimuovere impostazioni locali e preferenze memorizzate nella cache
- disinstallazione dell’app
- eliminazione manuale dei file di sottotitoli esportati dall’archiviazione dell’utente
- utilizzo dei controlli a livello di sistema operativo, come impostazioni delle notifiche, reimpostazione dell’ID pubblicitario o impostazioni di personalizzazione degli annunci

Per i dati trattati da Google, gli utenti dovrebbero inoltre fare riferimento, ove pertinente, agli strumenti di privacy e account di Google.

---

## 6. Privacy dei minori

Questa app non è destinata principalmente ai minori.

La sua finalità principale è la riproduzione, la modifica e la visualizzazione in overlay dei sottotitoli, oltre alle relative funzioni di utilità. Ove appropriato, la configurazione degli SDK pubblicitari può applicare indicatori relativi all’età o rivolti ai minori in conformità con i requisiti della piattaforma e le impostazioni dello sviluppatore.

---

## 7. Misure di sicurezza

Nei limiti dell’architettura dell’app, lo sviluppatore si impegna a:

- ridurre al minimo la raccolta mantenendo sul dispositivo la maggior parte dell’elaborazione di sottotitoli e contenuti multimediali
- utilizzare file picker di sistema e accesso ai file avviato dall’utente
- utilizzare i permessi di sistema in modo trasparente
- fare affidamento, ove applicabile, sul trasporto di rete cifrato utilizzato dagli SDK di terze parti

Nessun metodo di archiviazione o trasmissione è completamente sicuro, ma l’app è progettata per evitare raccolte non necessarie da parte dello sviluppatore.

---

## 8. Software open source

L’app utilizza software open source, comprese librerie relative a:

- parsing e serializzazione dei sottotitoli
- selezione dei file
- preferenze locali
- finestre overlay
- riproduzione video
- WebView

Le informative open source sono disponibili all’interno dell’app. Per alcuni componenti, l’app può utilizzare una copia modificata localmente di un pacchetto open source, mantenendo l’avviso di licenza originale.

---

## 9. Contatti

Se hai domande o richieste relative alla privacy:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Ti preghiamo di includere nella comunicazione il nome dell’app **Subtitle Player & Editor**.

---

## 10. Modifiche alla presente Informativa

La presente Informativa può essere aggiornata se:

- cambiano le funzionalità dell’app
- cambiano i permessi o l’uso degli SDK
- cambiano i requisiti legali o della piattaforma

Le modifiche sostanziali saranno riportate nella pagina aggiornata dell’informativa e, ove opportuno, anche nell’app.

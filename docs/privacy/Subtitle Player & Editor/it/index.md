---
title: Informativa sulla Privacy | Subtitle Tool
description: Informativa sulla privacy di Subtitle Player & Editor (Subtitle Tool)
lang: it
last_updated: 2025-12-12
---

# Informativa sulla Privacy (Subtitle Player & Editor / «Subtitle Tool»)

- **Nome dell’app:** Subtitle Player & Editor (di seguito, «Subtitle Tool»)  
- **Sviluppatore:** frog-im  
- **Contatto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Data di efficacia:** 2025-12-12  

> La presente Informativa è redatta facendo riferimento a normative applicabili quali la legge coreana sulla protezione delle informazioni personali (PIPA), il GDPR/UK GDPR, la legge svizzera FADP e le leggi statunitensi in materia di privacy a livello statale.  
> In caso di requisiti specifici per una determinata giurisdizione, tali requisiti prevalgono sulle disposizioni di questa Informativa.

---

## 1. Finalità e Ambito di Applicazione

Questa app fornisce funzioni di **modifica dei metadati dei file audio** (titolo, artista, ecc.) archiviati sul dispositivo e una funzione di **sovrapposizione di testi/lyrics e sottotitoli**.  
L’app **non crea un account utente** e **non carica** i contenuti dell’utente su nostri server. Il trattamento avviene di norma **in locale sul dispositivo dell’utente**.

Tuttavia, per finalità di **pubblicità** e di **adempimento di obblighi legali**, partner terzi (ad es. Google Mobile Ads SDK (AdMob) e UMP) possono raccogliere e trattare informazioni quali **identificatori pubblicitari**.  
La raccolta del consenso e la gestione delle preferenze sulla privacy seguono le specifiche di **Google UMP (User Messaging Platform)**.

---

## 2. Categorie di Informazioni Trattate

### 2-1) File Selezionati Esplicitamente dall’Utente

- **Percorsi e contenuti di file audio / immagini di copertina:** trattati **esclusivamente in locale** sul dispositivo per finalità di modifica e salvataggio.  
- **FFmpegKit** viene utilizzato in locale per operazioni di codifica, modifica dei metadati ed estrazione di miniature.  
- L’app **non carica** tali file selezionati dall’utente sui nostri server.

### 2-2) Impostazioni Locali e Valori Memorizzati

Per garantire le funzionalità principali e il comfort dell’utente, l’app memorizza i seguenti valori **in locale sul dispositivo**.  
Questi valori non vengono inviati ai nostri server e vengono **eliminati quando l’app o i suoi dati vengono rimossi**.

#### (1) Preferenze (`shared_preferences`)

| Tipo | Chiave/Contenuto | Finalità | Archiviazione | Cancellazione |
|---|---|---|---|---|
| Posizione/font dell’overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Ripristinare la posizione dell’overlay e la dimensione del font | SharedPreferences sul dispositivo | Eliminati alla cancellazione dei dati dell’app o alla disinstallazione |
| Impostazioni annunci/privacy | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Annunci non personalizzati, segnale U.S. RDP, tag child-directed (COPPA), etichetta di età, limite di classificazione dei contenuti pubblicitari | SharedPreferences sul dispositivo | Come a sinistra |

#### (2) File Temporanei (directory temporanea del sistema)

- **Esempi:** `cover_*.jpg`, `tmp_*.flac`  
- **Utilizzo:** estrazione di copertine, tagging FLAC, codifica temporanea  
- **Posizione:** cartella temporanea del sistema operativo (`systemTemp`)  
- **Conservazione:** l’app tenta di eliminarli al termine dell’elaborazione; possono inoltre essere rimossi dalle procedure di pulizia del sistema operativo.

#### (3) Salvataggio Selezionato dall’Utente (SAF)

- Quando l’utente utilizza la funzione «Salva con nome», i file audio finali possono essere scritti in posizioni da lui indicate (ad es. cartella Download, archiviazione cloud).  
- Questi file risiedono nella **memoria esterna** e **possono restare anche dopo la disinstallazione dell’app**. L’utente può eliminarli manualmente.

#### (4) Stato del Consenso (Cache UMP)

- Nelle regioni SEE/Regno Unito/Svizzera, l’SDK UMP **memorizza localmente in cache lo stato del consenso agli annunci dell’utente**.  
- Tale stato può essere reimpostato cancellando i dati dell’app oppure tramite la schermata **Opzioni sulla privacy** presente nell’app (se disponibile).

---

### 2-3) Dati Relativi a Annunci e Consenso (SDK di Terze Parti)

- **Google Mobile Ads SDK (AdMob) e UMP** possono raccogliere e trattare, ad esempio: **identificatori pubblicitari (AAID/IDFA)**, **intervalli di indirizzi IP**, **informazioni su dispositivo/app**, **segnali di interazione con gli annunci**, **stato del consenso**, ecc.  
- **Finalità:** erogazione di annunci, limitazione della frequenza, prevenzione delle frodi, misurazione delle prestazioni, adempimenti legali.  
- **Regioni che richiedono il consenso (SEE/Regno Unito/Svizzera):** il consenso viene raccolto tramite le schermate UMP e, ove richiesto, viene fornita una schermata di **Opzioni sulla privacy**.  
  Nelle regioni prive di tali requisiti (ad es. Corea), questa opzione **potrebbe non essere mostrata**.

---

## 3. Trattamento e Periodi di Conservazione

- **Impostazioni locali:** memorizzate sul dispositivo fino a quando l’utente non cancella i dati dell’app o disinstalla l’app stessa.  
- **File temporanei:** creati durante la codifica/estrazione, vengono eliminati dopo l’elaborazione oppure possono essere conservati temporaneamente nelle cache del sistema.  
- **Dati relativi ad annunci/consenso (terze parti):** sono conservati e cancellati in conformità alle **policy di Google**.

---

## 4. Trasferimenti a Terzi e Flussi Transfrontalieri

Per finalità pubblicitarie e di gestione del consenso, alcune informazioni sull’utente possono essere trasmesse all’infrastruttura di Google e ivi trattate.

| Voce | Dettagli |
|---|---|
| **Destinatario** | Google LLC e le sue affiliate/sotto-responsabili del trattamento |
| **Destinazione** | Stati Uniti (e altre regioni in cui è ospitata l’infrastruttura di Google) |
| **Finalità** | Erogazione di annunci, misurazione/prestazioni, conformità legale, gestione del consenso |
| **Dati** | Identificatori pubblicitari, intervalli IP, informazioni su dispositivo/app, interazioni con annunci, stato del consenso, ecc. |
| **Conservazione** | In conformità alle policy di Google |
| **Effetto del rifiuto** | La pubblicità personalizzata può essere limitata; possono essere mostrati annunci non personalizzati |

Rispettiamo i requisiti della sezione **«Sicurezza dei dati» di Google Play** e manteniamo tali dichiarazioni allineate al trattamento effettivo.

---

## 5. Diritti dell’Utente e Modalità di Esercizio

- **Disattivazione degli annunci personalizzati / modifica del consenso**  
  - Nelle regioni supportate (SEE/Regno Unito/Svizzera): è possibile modificare le preferenze in **Impostazioni → Opzioni sulla privacy**.  
  - In altre regioni: è possibile utilizzare le impostazioni del sistema operativo per **reimpostare gli ID pubblicitari / limitare il tracciamento degli annunci**.
- **Reimpostazione delle informazioni locali:** la cancellazione dei dati dell’app o la disinstallazione reimposta le coordinate dell’overlay, la dimensione del font e altre impostazioni locali.  
- I diritti previsti dal **GDPR/UK GDPR/FADP svizzero e dalle leggi statunitensi sulla privacy** (accesso, rettifica, cancellazione, portabilità, limitazione, revoca del consenso ecc.) possono essere esercitati nella misura prevista da tali normative.  
  Per i dati relativi agli annunci trattati da Google, si prega di utilizzare i **processi messi a disposizione da Google**.

---

## 6. Privacy dei Minori

Questa app **non è destinata ai minori**.  
Se un minore al di sotto dell’età minima legale utilizza l’app, dovrebbe interromperne l’uso e, insieme al proprio tutore, utilizzare le funzioni del sistema operativo per limitare la pubblicità.  
Se del caso, possiamo applicare tag come **TFUA (child-directed tag)** o opzioni simili a tutela dei minori.

---

## 7. Misure di Sicurezza

- **Minimizzazione dei dati** nella raccolta e nell’archiviazione  
- Uso limitato di file temporanei e loro eliminazione dopo il trattamento, quando possibile  
- Trattamento rigorosamente **nei limiti dei permessi del sistema operativo**  
- Crittografia **TLS o equivalente** durante la trasmissione a terzi (in linea con gli standard dei relativi SDK)

---

## 8. Sicurezza dei Dati (Google Play)

Compiliamo e manteniamo accuratamente la sezione **«Sicurezza dei dati»** nella Play Console e la aggiorniamo tempestivamente in caso di modifiche.

---

## 9. Software Open Source

L’app utilizza software open source come **FFmpeg**.  
All’interno dell’app è presente un file informativo (ad es. `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) che spiega come ottenere il codice sorgente.  
Su richiesta, forniremo il codice sorgente secondo le modalità indicate in tale file.

---

## 10. Contatti

- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Modifiche alla Presente Informativa

Potremo aggiornare la presente Informativa in seguito a modifiche legali o del servizio.  
Le modifiche saranno pubblicate **all’interno dell’app** e su questa **pagina dedicata alla privacy**.  
In caso di modifiche sostanziali, forniremo un preavviso **di almeno 7 giorni** prima della data di efficacia.

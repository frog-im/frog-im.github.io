---
title: Informativa sulla privacy | LyriFloat
description: Informativa sulla privacy di LyriFloat (Italiano)
lang: it
last_updated: 2025-10-30
---

# Informativa sulla privacy (LyriFloat)

- **Nome app:** LyriFloat
- **Sviluppatore:** frog-im  
- **Contatto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com) 
- **Data di entrata in vigore:** 2025-10-30

> La presente Informativa è redatta con riferimento alle leggi applicabili, tra cui la legge coreana sulla protezione delle informazioni personali (PIPA), il GDPR/UK GDPR, la LPD svizzera e le leggi statunitensi in materia di privacy a livello statale. In presenza di requisiti specifici per giurisdizione, tali requisiti prevalgono.

---

## 1. Finalità e ambito del trattamento

L’app fornisce funzioni di **modifica dei metadati** (titolo, artista ecc.) dei file audio **archiviati sul dispositivo** e un **overlay dei testi**.  
L’app **non** crea un account utente e **non** carica contenuti dell’utente su server propri. Il trattamento avviene **di norma sul dispositivo dell’utente**.

Tuttavia, per **finalità pubblicitarie** e di **conformità legale**, partner terzi (ad es. Google Mobile Ads SDK (AdMob), UMP) possono raccogliere e trattare informazioni come gli **identificatori pubblicitari**. La raccolta del consenso e le opzioni sulla privacy seguono le specifiche della **Google UMP (User Messaging Platform)**.

---

## 2. Categorie di informazioni trattate

### 2-1) File selezionati esplicitamente dall’utente
- **Percorsi e contenuti di audio/immagini di copertina:** trattati **localmente** sul dispositivo esclusivamente per l’editing/salvataggio.  
- **FFmpegKit** è utilizzato localmente per encoding, modifica metadati ed estrazione di miniature.  
- L’app **non carica** i file selezionati dall’utente sui nostri server.

### 2-2) Impostazioni locali e valori memorizzati

Per le funzioni principali e la comodità d’uso, l’app memorizza i seguenti valori **localmente sul dispositivo**.  
Questi valori non vengono inviati ai nostri server e **si eliminano quando l’utente cancella i dati dell’app o disinstalla l’app**.

#### (1) Preferenze (`shared_preferences`)
| Tipo | Chiave/Contenuto | Finalità | Posizione di archiviazione | Eliminazione |
|---|---|---|---|---|
| Posizione/font overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Ripristino della posizione dell’overlay e della dimensione del font | SharedPreferences del dispositivo | Eliminati alla cancellazione dei dati o alla disinstallazione |
| Pubblicità/Privacy | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Annunci non personalizzati, U.S. RDP, tag COPPA, tag età, limite classificazione contenuti pubblicitari | SharedPreferences del dispositivo | Come a sinistra |

#### (2) File temporanei (directory temporanea di sistema)
- **Esempi:** `cover_*.jpg`, `tmp_*.flac`  
- **Uso:** estrazione cover art, tagging FLAC, encoding temporanei  
- **Posizione:** cartella temporanea dell’OS (`systemTemp`)  
- **Conservazione:** rimossi dall’app dopo il completamento quando possibile; soggetti anche a pulizia periodica dell’OS

#### (3) Salvataggio scelto dall’utente (SAF)
- Con “Salva con nome”, i file finali possono essere scritti in percorsi scelti dall’utente (es. Download, cloud).  
- Tali file risiedono in **archiviazione esterna** e **permangono dopo la disinstallazione**. L’utente può eliminarli manualmente.

#### (4) Stato del consenso (cache SDK UMP)
- Nelle regioni SEE/UK/CH, l’SDK UMP **memorizza localmente** lo stato del consenso pubblicitario.  
- Reimpostabile cancellando i dati dell’app o tramite la schermata **Opzioni privacy** quando disponibile.

---

### 2-3) Dati pubblicitari e relativi al consenso (SDK di terze parti)
- **Google Mobile Ads SDK (AdMob) e UMP** possono raccogliere/trattare, ad esempio: **identificatori pubblicitari (AAID/IDFA)**, **intervalli IP**, **informazioni su dispositivo/app**, **segnali di interazione con gli annunci**, **stato del consenso**, ecc.  
- **Finalità:** erogazione degli annunci, limitazione frequenza, prevenzione frodi, misurazioni di performance, conformità legale  
- **Regioni con obbligo di consenso (SEE/UK/CH):** il consenso è raccolto tramite UMP e viene fornita la schermata **Opzioni privacy** quando richiesto.  
  Nelle regioni prive di tale obbligo (es. KR), l’opzione **potrebbe non essere mostrata**.

---

## 3. Trattamento e periodi di conservazione

- **Impostazioni locali:** conservate sul dispositivo fino alla cancellazione dei dati dell’app o alla disinstallazione  
- **File temporanei:** creati durante encoding/estrazione; rimossi al termine o possono restare temporaneamente nelle cache dell’OS  
- **Dati pubblicitari/consenso (terzi):** secondo le **policy di Google**

---

## 4. Comunicazioni a terzi e trasferimenti transfrontalieri

Per pubblicità e gestione del consenso, le informazioni degli utenti possono essere trasmesse all’infrastruttura di Google ed elaborate su di essa.

| Voce | Dettagli |
|---|---|
| **Destinatario** | Google LLC e affiliate/sub-responsabili |
| **Destinazione** | Stati Uniti (e altre regioni in cui è situata l’infrastruttura Google) |
| **Finalità** | Erogazione annunci, performance/misurazione, conformità legale, gestione del consenso |
| **Dati** | Identificatori pubblicitari, intervalli IP, info dispositivo/app, interazioni con annunci, stato consenso, ecc. |
| **Conservazione** | In base alle policy di Google |
| **Effetto del rifiuto** | Personalizzazione limitata; possono essere mostrati solo annunci non personalizzati |

Rispettiamo i requisiti di divulgazione della sezione **“Sicurezza dei dati” di Google Play** e manteniamo le informazioni allineate al trattamento effettivo.

---

## 5. Diritti dell’interessato e modalità di esercizio

- **Disattivare annunci personalizzati / modificare il consenso**  
  - Nelle regioni supportate (SEE/UK/CH): modificare in **Impostazioni → Opzioni privacy**.  
  - Altre regioni: utilizzare le impostazioni dell’OS per **reimpostare l’ID pubblicitario / limitare il tracciamento**.
- **Reimpostare le informazioni locali:** cancellando i dati dell’app o disinstallando si reimpostano coordinate dell’overlay, dimensione del font e altre impostazioni locali.
- I diritti previsti da **GDPR/UK GDPR/LPD svizzera/leggi statunitensi a livello statale** (accesso, rettifica, cancellazione, portabilità, limitazione, revoca del consenso, ecc.) possono essere esercitati secondo le procedure previste.  
  Per i dati pubblicitari trattati da Google, utilizzare le **procedure di Google**.

---

## 6. Privacy dei minori

Questa app **non è rivolta ai minori**. Un minore al di sotto dell’età legale minima deve interrompere l’uso e, con il tutore, utilizzare le funzioni di limitazione degli annunci a livello di OS. Se del caso, possiamo applicare **TFUA (child-directed tag)** o opzioni equivalenti di protezione dei minori.

---

## 7. Misure di sicurezza

- **Minimizzazione dei dati** nella raccolta e archiviazione  
- **Uso limitato** di file temporanei e tentativi di eliminazione dopo l’elaborazione  
- Trattamento **nel perimetro dei permessi dell’OS**  
- **Crittografia in transito** (TLS o equivalente) per i trasferimenti a terzi secondo gli standard degli SDK

---

## 8. Sicurezza dei dati (Google Play)

Manteniamo accurata la sezione **“Sicurezza dei dati”** nella Play Console e la aggiorniamo tempestivamente in caso di modifiche.

---

## 9. Avvisi open source

L’app utilizza software open source come **FFmpeg**. Un file informativo (ad es. `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) incluso nell’app spiega come ottenere il codice sorgente. Su richiesta, forniremo il sorgente secondo le indicazioni del file.

---

## 10. Contatti

- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Modifiche alla presente Informativa

Possiamo rivedere la presente Informativa a seguito di modifiche normative o di servizio. Le variazioni saranno pubblicate **nell’app** e in questa **pagina di policy**.  
In caso di modifiche sostanziali, verrà fornito un preavviso **di almeno 7 giorni** prima della data di efficacia.

---

## Appendice: Guida per l’utente

- **Link in-app:** aprire questa pagina da **Impostazioni → Privacy**.  
- **Comportamento regionale:** in SEE/UK/CH vengono mostrate le Opzioni privacy. **In KR e in alcune altre regioni, il pulsante potrebbe non mostrare opzioni aggiuntive** se non richiesto dalla legge.




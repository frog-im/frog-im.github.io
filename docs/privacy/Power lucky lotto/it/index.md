---
title: Informativa sulla privacy | Power lucky lotto
description: Informativa sulla privacy di Power lucky lotto (Italiano)
lang: it
last_updated: 2026-01-29
---

# Informativa sulla privacy (Power lucky lotto)

- **Nome app:** Power lucky lotto  
- **Sviluppatore:** frog-im  
- **Contatto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Data di efficacia:** 2026-01-29  

> Questa informativa è redatta facendo riferimento alle leggi applicabili (PIPA coreana, GDPR/UK GDPR, FADP svizzera, leggi sulla privacy di alcuni stati USA, ecc.).  
> Se nella tua area vigono requisiti obbligatori specifici, tali requisiti prevalgono.

---

## 1. Finalità e ambito

Power lucky lotto è un’app per gestire giochi di lotteria e consultare registri. Funzionalità principali:

- Selezione/configurazione paese e gioco (es. KR 6/45, US Powerball)  
- Generazione/salvataggio numeri e visualizzazione dei log (storico)  
- Visualizzazione ed eliminazione tabelle di log (lista/dettaglio)  
- Modifica/gestione dati risultati tramite JSON (statistiche/visualizzazione)  
- Pubblicità (incluse reward ads) e gestione del consenso (quando richiesto)

L’app **non richiede la creazione di un account** e, di default, **non carica i tuoi dati sui server dello sviluppatore**.  
La maggior parte del trattamento avviene **sul dispositivo**.

Tuttavia, per **pubblicità**, **gestione del consenso** e **conformità**, SDK di terze parti come  
**Google Mobile Ads SDK (AdMob)** e **Google UMP** possono raccogliere/trattare alcuni dati (es. identificativi pubblicitari).

---

## 2. Tipologie di dati trattati

### 2-1) Dati salvati localmente sul dispositivo

#### (1) Impostazioni (SharedPreferences)

| Categoria | Chiave (esempio) | Scopo | Memoria | Cancellazione |
|---|---|---|---|---|
| Setup completato | `setup_done` | Stato configurazione iniziale | SharedPreferences | Eliminazione dati/disinstallazione |
| Storico paesi | `selected_countries` | Paesi selezionati di recente | Idem | Idem |
| Paese attivo | `active_country` | Paese attualmente selezionato | Idem | Idem |
| Giochi selezionati | `selected_lotto_ids` | ID giochi selezionati | Idem | Idem |
| Gioco attivo | `active_lotto_id` | ID gioco attivo | Idem | Idem |
| **Selezione orario seed (opzionale)** | `birth_datetime_iso` | Orario seed scelto dall’utente (può servire come seed/personalizzazione) | Idem | Idem |

#### (2) Dati log (SQLite)

- Tabelle tipiche: `log_...`  
- Campi possibili: `id`, `date_id` o `date_text`, `choice1..choiceN`, `isFinger`

I log sono consultabili ed eliminabili dall’app (per tabella o per riga).

#### (3) File JSON (per gioco)

- Esempio: `game_json/<gameId>.json`  
- Scopo: dati di estrazioni/risultati gestiti e modificabili dall’utente (statistiche/visualizzazione)

---

### 2-2) Pubblicità, consenso e dati correlati (SDK di terze parti)

AdMob/UMP possono trattare:

- ID pubblicitario (AAID/IDFA)  
- Informazioni basate su IP, posizione approssimativa, rete  
- Informazioni dispositivo/app (versioni, lingua, diagnostica)  
- Interazioni con annunci (impression, click, completamento reward)  
- Scelte/stato del consenso (UMP)

---

## 3. Periodo di conservazione

- Impostazioni locali: fino a cancellazione dati app o disinstallazione  
- Log SQLite: fino a eliminazione da parte dell’utente o cancellazione dati/disinstallazione  
- File JSON: nel directory documenti dell’app; export/backup sono sotto responsabilità dell’utente  
- Dati pubblicità/consenso: secondo policy Google e leggi applicabili

---

## 4. Terze parti e trasferimenti internazionali

| Voce | Dettagli |
|---|---|
| Destinatari | Google LLC, affiliate e sub-responsabili |
| Destinazioni | USA e altre aree con infrastruttura Google |
| Scopo | Erogazione/misurazione annunci, antifrode, consenso, conformità |
| Dati | ID pubblicitario, info IP, info dispositivo/app, interazioni, consenso |
| Conservazione | Secondo policy Google e norme |
| Impatto se rifiuti | Minore personalizzazione; annunci non personalizzati o meno annunci |

---

## 5. Diritti dell’utente

In base alla legge applicabile, potresti avere diritti di accesso, rettifica, cancellazione, limitazione, opposizione, portabilità e revoca del consenso (se pertinente).

- Modifica scelte ads/consenso: tramite “Privacy Options” in-app (se disponibile) o impostazioni OS (reimposta ID pubblicitario, limita personalizzazione).  
- Reset dati locali: cancella dati app o disinstalla.

---

## 6. Privacy dei minori

L’app **non è progettata per i minori**. Se necessario, si raccomandano controlli parentali e limitazioni pubblicitarie a livello di sistema.

---

## 7. Misure di sicurezza

- Minimizzazione dei dati salvati localmente  
- Elaborazione sul dispositivo quando possibile  
- Trasporto sicuro (TLS) per comunicazioni SDK (nei limiti delle capacità dell’SDK)

---

## 8. Data safety (Google Play)

Se distribuita su Google Play, lo sviluppatore si impegna a mantenere aggiornate le dichiarazioni Data safety in caso di modifiche a SDK o pratiche.

---

## 9. Avvisi open source

L’app può utilizzare librerie open source (icone paesi, archiviazione, ads/consenso, UI).  
Le licenze sono disponibili nella schermata “Licenze open source” (o equivalente) dell’app.

---

## 10. Contatti

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
Indica “Power lucky lotto” nella richiesta.

---

## 11. Modifiche a questa informativa

Può cambiare per aggiornamenti normativi, nuove funzioni (es. nuovi SDK) o politiche interne.  
Le modifiche minori saranno pubblicate nell’app o su questa pagina; le modifiche rilevanti saranno comunicate in anticipo ove richiesto.

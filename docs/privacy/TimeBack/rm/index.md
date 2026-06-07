---
title: Politica da protecziun da datas | TimeBack
description: Politica de confidențialitate TimeBack
lang: rm
last_updated: 2026-06-06
---

# Politica de confidențialitate (TimeBack)

- **Numele aplicației:** TimeBack
- **Dezvoltator:** frog-im
- **Contact:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data intrării în vigoare:** 2026-06-03
- **Ultima actualizare:** 2026-06-06

Această politică de confidențialitate se bazează pe implementarea actuală a aplicației TimeBack. TimeBack oferă o analiză a timpului de ecran, obiective zilnice, înregistrări ale timpului recuperat, reflecții, provocări, notificări, partajare și funcții de publicitate.

## 1. Caracteristici

TimeBack oferă următoarele caracteristici:

- Revizuirea timpului de utilizare a aplicației prin permisiunea de acces pentru utilizarea Android
- Obiective zilnice de utilizare, mementouri și notificări de utilizare din bara de stare
- Notificări de avertizare cu limită strictă și afișare suprapusă
- Selecția aplicației de excepție prin suprapunere
- Înregistrări ale activității la timp recuperat
- Înregistrări zilnice de reflecție
- Progresul provocării și gestionarea listelor de verificare
- Partajarea imaginilor statistice de utilizare
- Anunțuri Google AdMob și opțiuni de confidențialitate bazate pe UMP

## 2. Informații pe care le procesăm

### 2-1. Permisiune de acces de utilizare pentru citirea informațiilor

Dacă utilizatorul acordă permisiunea Android `PACKAGE_USAGE_STATS`, aplicația poate citi următoarele informații de pe dispozitiv:

- Numele pachetului aplicației
- Numele aplicației
- Timp de utilizare a aplicației
- Intervalul de date și oră utilizat pentru agregarea utilizării

Aceste informații sunt folosite pentru a furniza statistici de utilizare și pentru a compara utilizarea cu obiectivele utilizatorilor.

### 2-2. Informații introduse sau configurate de utilizator

- Obiectiv de utilizare zilnică
- Stare și interval activate pentru memento de utilizare
- Setarea afișajului de utilizare a barei de stare
- Categoria de activitate în timpul revendicării, titlul, ora de începere și durata
- Text de reflecție zilnică
- Provocați progresul și intrările din lista de verificare
- Suprapunerea listei de aplicații cu excepții

### 2-3. Informații stocate pe dispozitiv

Aplicația poate stoca următoarele informații într-o bază de date locală SQLite sau SharedPreferences:

- Înregistrările timpului de utilizare a aplicației
- Obiective și setări zilnice
- Înregistrări ale activității la timp recuperat
- Înregistrări zilnice de reflecție
- Provocarea progresului și starea listei de verificare
- Starea de finalizare a integrării
- Setări, cum ar fi mementouri de utilizare, avertismente de limită, afișarea barei de stare și aplicații de excepție suprapuse
- Consimțământul pentru anunțuri locale și starea opțiunii de confidențialitate

Pe baza implementării curente, aceste înregistrări locale nu sunt încărcate automat pe serverele frog-im.

### 2-4. Date de publicitate și consimțământ

Când sunt utilizate anunțuri mobile Google SDK (AdMob) și UMP, Google sau afiliații săi pot prelucra informații precum:

- Identificatori de publicitate, cum ar fi Android AD_ID
- IP adresa și informații despre rețea
- Informații despre dispozitiv, versiunea OS și informații despre aplicație
- Afișări de anunțuri, clicuri, date de măsurare și semnale de eroare
- Consimțământul publicitar și starea opțiunii de confidențialitate
- Locație aproximativă

## 3. Scopurile Prelucrării

Aplicația prelucrează informații în următoarele scopuri:

- Citirea timpului de utilizare, afișarea statisticilor și compararea utilizării cu obiectivele
- Stocarea înregistrărilor de timp recuperat și de reflecție introduse de utilizator
- Gestionarea progresului provocării
- Furnizarea de mementouri și notificări din bara de stare
- Furnizarea de notificări de avertizare cu limită strictă, afișare suprapusă și gestionarea excepțiilor de suprapunere
- Partajarea imaginilor cu statistici de utilizare la cererea utilizatorului
- Difuzarea de anunțuri, măsurarea performanței anunțurilor și aplicarea opțiunilor de consimțământ pentru anunțuri
- Menținerea stabilității aplicației și răspunsul la erori

## 4. Stocare locală și procesare externă

### 4-1. Stocare locală

TimeBack stochează datele utilizatorului în principal în memoria internă a aplicației de pe dispozitiv. Pe baza implementării curente, înregistrările de utilizare, obiectivele, reflecțiile și informațiile despre provocări nu sunt încărcate automat pe serverele frog-im.

Stocarea locală poate include următoarele.

| Depozitare | Articole depozitate | Scop | Metoda de ștergere |
|---|---|---|---|
| baza de date SQLite | Înregistrări de utilizare a aplicațiilor, nume de pachete, nume de aplicații, timp de utilizare, agregate bazate pe dată | Afișați statistici de utilizare și comparați utilizarea cu obiectivele | Funcții de ștergere în aplicație, ștergerea datelor aplicației sau dezinstalarea aplicației |
| baza de date SQLite | Activități în timp recuperat, reflecții, progresul provocării, intrări în lista de verificare | Afișați înregistrările și gestionați progresul | Funcții de ștergere în aplicație, ștergerea datelor aplicației sau dezinstalarea aplicației |
| SharedPreferences | Starea de finalizare a integrării, setări de memento, setări de avertizare de limită, setări de afișare a barei de stare, lista de aplicații de excepție suprapusă, stare locală de consimțământ pentru anunțuri | Păstrați setările aplicației | Ștergerea datelor aplicației sau dezinstalarea aplicației |
| Fișiere temporare/cache | Imagini cu statistici de utilizare partajate și fișiere temporare similare | Efectuați partajarea solicitată de utilizator | Șters după distribuire, acolo unde este posibil, sau conform politicilor de curățare OS/aplicații |

Când utilizatorul șterge datele aplicației sau dezinstalează aplicația, datele stocate în stocarea internă a aplicației sunt în general șterse. Cu toate acestea, backupul Android, backupul producătorului, backupul în cloud sau fișierele partajate direct de utilizator pot fi păstrate separat, în conformitate cu politicile acelor servicii.

Înregistrările de utilizare și textul de reflecție pot dezvălui rutine sau interese personale. Pe dispozitivele partajate, utilizatorii ar trebui să folosească măsuri de protecție adecvate, cum ar fi blocarea dispozitivului sau conturi OS separate.

### 4-2. Încărcări de server

Pe baza proiectului actual, TimeBack nu încarcă automat înregistrări de utilizare, reflecții sau înregistrări de provocare pe serverele frog-im. Dacă utilizatorul folosește funcția de partajare, o imagine statistică generată poate fi transferată către aplicația sau serviciul extern selectat de utilizator.

### 4-3. Procesare de publicitate

Google AdMob și UMP sunt folosite pentru publicitatea în aplicație și gestionarea consimțământului. Informațiile legate de publicitate pot fi procesate pe infrastructura Google.

## 5. Servicii și procesatori terți

### 5-1. Google AdMob / UMP

Scop:

- Livrare de anunțuri banner
- Consimțământul publicitar și gestionarea opțiunilor de confidențialitate
- Măsurarea performanței reclamelor și prevenirea fraudei

Informații care pot fi prelucrate:

- Identificatori de publicitate
- Informații despre dispozitiv și rețea
- Informații despre interacțiunea cu anunțurile
- Consimțământul și starea opțiunii de confidențialitate

### 5-2. Partajarea aplicațiilor sau serviciilor țintă

Dacă utilizatorul utilizează direct caracteristica de partajare a imaginilor cu statistici de utilizare, aplicația sau serviciul extern selectat poate procesa imaginea partajată. Această prelucrare este guvernată de politica de confidențialitate a serviciului selectat.

## 6. Notificare de transfer transfrontalier

Informațiile pot fi prelucrate în afara țării utilizatorului în următoarele cazuri.

| Articol | Detalii |
|---|---|
| Destinatar | Google LLC și afiliații săi |
| Destinaţie | Statele Unite și alte țări/regiuni în care se află infrastructura Google |
| Sincronizare | Când aplicația rulează, solicită anunțuri, afișează sau măsoară anunțuri, procesează clicurile sau gestionează consimțământul |
| Metodă | Comunicație de rețea criptată (HTTPS/TLS) |
| Scop | Livrarea anunțurilor, gestionarea stării de personalizare, măsurare, analiză, îmbunătățirea stabilității serviciilor, conformitatea legală |
| Date | Identificatori de publicitate, informații despre dispozitiv/aplicație/rețea, informații despre interacțiunea cu anunțurile, starea consimțământului, locația aproximativă etc. |
| Retenţie | În conformitate cu politicile Google și cu legea aplicabilă |

Pentru detalii, consultați [Cross-Border Transfer Notice](./policy/).

## 7. Lista de aplicații instalată și excepții de suprapunere

Pe Android, dacă utilizatorul configurează aplicații de excepție suprapuse, aplicația poate citi numele pachetelor și numele aplicațiilor aplicațiilor care pot fi lansate pe dispozitiv pentru a afișa o listă de selecție. Numele pachetelor selectate de utilizator ca excepții sunt stocate în SharedPreferences de pe dispozitiv și sunt utilizate numai pentru a evita afișarea suprapunerilor de avertismente de limită strictă deasupra acelor aplicații.

## 8. Retentie

Aplicația reține informații în conformitate cu următoarele standarde:

- Informații locale despre utilizare, obiectiv, reflecție și provocare: până când utilizatorul le șterge, șterge datele aplicației sau dezinstalează aplicația
- Setări SharedPreferences: până când utilizatorul șterge datele aplicației sau dezinstalează aplicația
- Fișiere temporare pentru imaginile partajate: după cum este necesar pentru partajare sau conform politicilor de curățare OS
- Publicitate și date legate de consimțământ: conform politicilor Google și ale altor terțe părți relevante

## 9. Permisiuni

Aplicația poate folosi următoarele permisiuni:

- `PACKAGE_USAGE_STATS`: citiți timpul de utilizare a aplicației
- `POST_NOTIFICATIONS`: afișați mementouri de utilizare și notificări din bara de stare
- `SYSTEM_ALERT_WINDOW`: afișați suprapuneri de avertismente de limită strictă
- `INTERNET`: comunicați cu anunțurile SDK și afișați paginile cu notificări legale
- `ACCESS_NETWORK_STATE`: verificați starea rețelei
- `com.google.android.gms.permission.AD_ID`: utilizați identificatori de publicitate

Permisiunile sunt folosite numai după cum este necesar pentru funcțiile aplicației. Utilizatorii pot revoca permisiunile din setările dispozitivului, dar funcțiile asociate pot fi limitate.

## 10. Drepturile și opțiunile utilizatorului

Utilizatorii pot:

- Vizualizați, editați sau ștergeți înregistrările din aplicație
- Ștergeți informațiile locale ștergând datele aplicației sau dezinstalând aplicația
- Modificați setările privind accesul, notificarea și identificatorul de publicitate în setările dispozitivului
- Revocați permisiunea de suprapunere și modificați setările aplicației pentru excepția suprapunerii
- Modificați opțiunile de confidențialitate a anunțurilor
- Contactați-ne pentru întrebări de confidențialitate sau solicitări de ștergere

E-mail de contact: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Măsuri de securitate

Aplicația aplică sau poate aplica următoarele măsuri de protecție:

- Comunicare externă bazată pe HTTPS/TLS
- Local-în primul rând prelucrarea datelor
- Solicitări minime de permisiuni necesare pentru funcțiile aplicației
- Aplicarea stării de consimțământ publicitar

Condițiile de securitate ale dispozitivului, cum ar fi rooting, jailbreaking, malware sau utilizarea dispozitivului partajat pot crea riscuri suplimentare.

## 12. Confidențialitatea copiilor

TimeBack nu este conceput în primul rând pentru copii. Setările legate de vârstă sau politicile platformei Google Mobile Ads SDK și UMP se pot aplica în timpul procesării publicității și a consimțământului.

## 13. Schimbări

Această politică poate fi actualizată din cauza modificărilor aduse legii, configurației serviciilor terță parte sau caracteristicilor aplicației. Modificările materiale vor fi notificate prin notificare în aplicație sau prin actualizarea acestei pagini.

## 14. Contact

- Dezvoltator: frog-im
- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

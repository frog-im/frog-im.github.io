---
title: Datenschutzerklärung | know_me
description: know_me (PeopleNote, Memory for People) Datenschutzerklärung (Deutsch)
---

# Datenschutzerklärung (know_me / PeopleNote, Memory for People)

- **Name der App:** know_me (PeopleNote, Memory for People)
- **Entwickler:** frog-im
- **Datenschutzbeauftragter / Ansprechpartner:** frog-im
- **Kontakt:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Inkrafttretensdatum:** 2026-03-04
- **Zuletzt aktualisiert:** 2026-03-04

> Diese Richtlinie wurde auf Grundlage der von der App verarbeiteten Informationen und ihrer damit verbundenen Funktionen erstellt.  
> Sofern in einem bestimmten Land oder einer bestimmten Region zwingende Gesetze oder Vorschriften gelten, können diese Vorrang haben.

---

## 1. Zweck und Geltungsbereich

`know_me` ist eine App, die Nutzern dabei helfen soll, Informationen über Personen zu erfassen und zu verwalten sowie diese Informationen bei Bedarf zu sichern, wiederherzustellen und als PDF-Dateien zu teilen.

Zu den Hauptfunktionen gehören:

- Speicherung personenbezogener Informationen zu einzelnen Personen (wie Name, Identifikationstext, Notizen, Persönlichkeitsmerkmale, Land, Geschlecht, Kontaktdaten usw.)
- Ordnerklassifizierung, Suche und Zusammenführungsfunktionen
- Anhängen von Fotos und Verwaltung von Beschreibungen
- Export und Import von Sicherungen (`.knm`)
- Export von PDF-Dateien
- App-Sperre (Passwort/Muster)
- Werbe- und Einwilligungsverwaltung (AdMob/UMP)

Für die App ist keine separate Kontoregistrierung erforderlich, und die Kerndaten des Nutzers werden in der Regel lokal auf dem Gerät des Nutzers gespeichert.  
Bestimmte Drittanbieter-SDKs, die für Werbung und Einwilligungsverwaltung eingebunden sind, können jedoch einige Informationen verarbeiten.

---

## 2. Kategorien verarbeiteter personenbezogener Daten

### 2-1) Vom Nutzer direkt eingegebene Informationen

Die folgenden Informationen werden nur gespeichert, wenn der Nutzer sie direkt eingibt:

- Name
- Identifikationstext (z. B. Aussehen/Merkmale als Notiztext)
- Notizen
- Persönlichkeitsmerkmale, Land, Geschlecht
- Telefonnummer
- Text im Zusammenhang mit dem Auftretenszeitpunkt / Zeitpunkt des Treffens
- Plattform-/Website-Informationen
- Ordnername/Farbe
- Bildbeschreibung (caption)

### 2-2) Auf dem Gerät ausgewählte Dateien

- Bilddateien, die der Nutzer beim Anhängen von Fotos auswählt
- `.knm`-Sicherungsdateien, die der Nutzer beim Import von Sicherungen auswählt
- Speicherpfade und gespeicherte Dateien, die der Nutzer beim Export von PDFs/Sicherungen auswählt

### 2-3) Lokal innerhalb der App gespeicherte Daten

Die folgenden Daten können auf dem Gerät des Nutzers gespeichert werden, um die Funktionen der App bereitzustellen:

- SQLite-Datenbank (`people_note.db`): Metadaten zu Personen/Ordnern/Plattformen/Websites/Bildern
- Bilddateien: verschlüsselt und im Dokumentenordner der App gespeichert (`.enc`)
- App-Einstellungen (`SharedPreferences`): Design, Sortierung, Datenschutz-/Werbeoptionen, PDF-Maskierungsoptionen, Richtlinien für die App-Sperre usw.
- Informationen zur App-Sperre: Hash-Werte und Salt-Werte für Passwörter/Muster (`SharedPreferences`)
- Lokale Verschlüsselungsschlüssel: gespeichert in `flutter_secure_storage`
- Temporäre Dateien: Vorschaudateien für Bildentschlüsselung, Import-/Export-Cache-Dateien usw. (temporärer Ordner)

### 2-4) Informationen, die bei Werbung und Einwilligungsverwaltung automatisch verarbeitet werden können

Wenn Funktionen für Werbung oder Einwilligungsverwaltung aktiviert sind, können SDKs von Google LLC und verbundenen Partnern (wie AdMob und UMP) die folgenden Informationen automatisch verarbeiten:

- Werbe-IDs (AAID/IDFA usw.)
- IP-Adresse und Netzwerkinformationen
- Geräteinformationen (Betriebssystemversion, Gerätemodell, App-Version usw.)
- Informationen zur Interaktion mit Werbung (Impressionen, Klicks usw.)
- Einwilligungsstatus und Informationen zu Datenschutzeinstellungen
- Diagnose-, Leistungs- und sicherheitsbezogene Informationen

Die Kerndaten des Nutzers werden in der Regel nicht auf den Server des Entwicklers hochgeladen, jedoch können einige der oben genannten Informationen an Drittanbieterdienste übermittelt werden, solange Werbe-/Einwilligungsfunktionen genutzt werden.

---

## 3. Zweck der Verarbeitung personenbezogener Daten

Die App verarbeitet personenbezogene Daten oder damit zusammenhängende Informationen zu folgenden Zwecken:

- Erfassung und Anzeige personenbezogener Informationen mit Schwerpunkt auf Kontakten/Notizen
- Bereitstellung von Organisationsfunktionen wie Ordnerklassifizierung, Suche und Zusammenführung
- Anhängen und Anzeigen von Fotos
- Durchführung nutzerseitig angeforderter Funktionen wie Sicherung/Wiederherstellung und PDF-Export
- Bereitstellung von Sicherheitsfunktionen für die App-Sperre
- Bereitstellung von Werbung, Verwaltung von Einwilligungen, Verhinderung betrügerischer Aktivitäten und Erfüllung gesetzlicher Verpflichtungen

---

## 4. Aufbewahrungs- und Speicherfrist personenbezogener Daten

- Interne App-Daten (SQLite, lokale Einstellungen, verschlüsselte Bilder): werden auf dem Gerät des Nutzers gespeichert, bis die App gelöscht, die App-Daten gelöscht oder die Daten vom Nutzer direkt entfernt werden
- Temporäre Dateien: werden nach Abschluss der jeweiligen Aufgabe gelöscht oder gemäß der Cache-Richtlinie des Betriebssystems bereinigt
- Vom Nutzer exportierte Dateien (PDFs, Sicherungsdateien): können am vom Nutzer gewählten Speicherort verbleiben und müssen vom Nutzer direkt gelöscht werden
- Werbe-/einwilligungsbezogene Daten (durch Dritte verarbeitet): unterliegen den Richtlinien des jeweiligen Dienstanbieters und den geltenden Gesetzen

Grundsätzlich speichert die App keine Kerndaten des Nutzers auf dem Server des Entwicklers.  
Dateien, die der Nutzer direkt in externen Speicher speichert, werden jedoch in der eigenen Umgebung des Nutzers verwaltet.

---

## 5. Verfahren und Methoden zur Löschung personenbezogener Daten

Wenn der Zweck der Verarbeitung erreicht wurde oder der Nutzer die Löschung verlangt, löscht die App die betreffenden Informationen oder verarbeitet sie so, dass nicht mehr auf sie zugegriffen wird, wie nachfolgend beschrieben.

### 5-1) Löschverfahren

- Wenn der Nutzer einzelne Personeneinträge, Ordner, Bilder, Sicherungsdaten usw. direkt löscht, werden diese Daten unverzüglich zur Löschung vorgesehen.
- Wenn der Nutzer die App löscht oder die App-Daten in den Geräteeinstellungen löscht, werden im internen Speicherbereich der App gespeicherte Daten gemäß den Löschverfahren des Betriebssystems entfernt.
- Temporäre Dateien werden nach Abschluss der jeweiligen Aufgabe zur Bereinigung vorgesehen, und einige zwischengespeicherte Daten können abhängig von der Richtlinie des Betriebssystems noch für einen bestimmten Zeitraum verbleiben.

### 5-2) Löschmethoden

- SQLite-Daten: Löschung der entsprechenden Datensätze
- App-Einstellungen (`SharedPreferences`): Löschung des entsprechenden Schlüssels oder sämtlicher Einstellungen
- Werte in `flutter_secure_storage`: Löschung der entsprechenden sicheren Speichereinträge
- Interne App-Dateien (verschlüsselte Bilder, temporäre Dateien usw.): Löschung der entsprechenden Dateien
- Vom Nutzer direkt in externem Speicher gespeicherte PDFs/Sicherungsdateien: werden nicht automatisch von der App gelöscht und müssen vom Nutzer selbst gelöscht werden

Sofern gesetzlich nichts anderes vorgeschrieben ist, speichert der Entwickler die Kerndaten des Nutzers nicht gesondert auf dem Server des Entwicklers.

---

## 6. Weitergabe an Dritte, Auftragsverarbeitung und grenzüberschreitende Übermittlung

Die App kann Google-Dienste für Werbung und Einwilligungsverwaltung verwenden.

| Punkt | Details |
|---|---|
| **Empfänger / Auftragsverarbeiter** | Google LLC und verbundene Unternehmen (Betreiber von AdMob/UMP) |
| **Land der Übermittlung** | Vereinigte Staaten und Regionen, in denen die Google-Infrastruktur betrieben wird |
| **Zeitpunkt der Übermittlung** | Fortlaufend bei Werbeanfragen, Prüfungen des Einwilligungsstatus, SDK-Initialisierung und Betrieb |
| **Art der Übermittlung** | Übertragung durch Netzwerkkommunikation zwischen der App und Servern Dritter |
| **Rechtsgrundlage für die grenzüberschreitende Übermittlung** | Verarbeitung im zur Bereitstellung des Dienstes erforderlichen Umfang auf Grundlage anwendbarer Rechtsgrundlagen oder, soweit erforderlich, auf Grundlage der Einwilligung der betroffenen Person |
| **Zweck** | Bereitstellung von Werbung, Werbemessung, Einwilligungsverwaltung, Betrugsprävention und Einhaltung von Richtlinien/Gesetzen |
| **Datenkategorien (Beispiele)** | Werbe-IDs (AAID/IDFA), IP-/Netzwerkinformationen, Geräte-/App-Informationen, Informationen zur Werbeinteraktion, Einwilligungsstatus |
| **Aufbewahrungsfrist** | Unterliegt den Richtlinien von Google und den geltenden Gesetzen |
| **Folgen einer Verweigerung** | Personalisierte Werbung kann eingeschränkt werden, nicht personalisierte Werbung kann angezeigt werden oder bestimmte werbebezogene Funktionen können eingeschränkt sein |

Der Entwickler erhebt oder verkauft die Kerndaten zu Personeneinträgen der App nicht über einen eigenen Server.

---

## 7. Informationen zu verwendeten Berechtigungen

Die App kann die folgenden Berechtigungen verwenden:

- `INTERNET`: Kommunikation für Werbe-SDKs und damit verbundene Netzwerkfunktionen
- `com.google.android.gms.permission.AD_ID`: Verwendung von Werbe-IDs (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 und darunter): Anhängen/Auswählen von Fotos

Berechtigungen werden nur in dem Umfang verwendet, der zur Bereitstellung der jeweiligen Funktionen erforderlich ist.

---

## 8. Einrichtung, Betrieb und Ablehnung automatischer Erfassungsmechanismen

Diese App verwendet nicht direkt allgemeine Website-Cookies.  
Im Zusammenhang mit Werbe- und Einwilligungsverwaltungsfunktionen können Drittanbieter-SDKs jedoch automatisch Werbe-IDs, Netzwerkinformationen, Geräteinformationen und ähnliche Daten verarbeiten.

Nutzer können die entsprechenden Einstellungen auf folgende Weise anpassen:

- Auswahl innerhalb der Datenschutzoptionen oder des Einwilligungsverwaltungsbildschirms der App ändern (sofern verfügbar)
- Die Werbe-ID in den Einstellungen des Gerätebetriebssystems zurücksetzen oder löschen
- Personalisierte Werbung einschränken oder zugehörige Datenschutzoptionen in den Einstellungen des Gerätebetriebssystems anpassen

Wenn der Nutzer personalisierte Werbung einschränkt, kann nicht personalisierte Werbung angezeigt werden oder bestimmte werbebezogene Funktionen können eingeschränkt sein.

---

## 9. Rechte der Nutzer und deren Ausübung

Vorbehaltlich der geltenden Gesetze können Nutzer folgende Rechte haben:

- Auskunft über personenbezogene Daten sowie Berichtigung oder Löschung verlangen
- Einschränkung oder Aussetzung der Verarbeitung verlangen
- Eine Einwilligung für einwilligungsbasierte Verarbeitung widerrufen
- Werbe-/Einwilligungseinstellungen ändern

Diese Rechte können auf folgende Weise ausgeübt werden:

- Daten direkt innerhalb der App ändern oder löschen
- Lokale Daten zurücksetzen, indem App-Daten gelöscht oder die App deinstalliert wird
- Die Werbeeinwilligung über die Datenschutzoptionen/den Einwilligungsbildschirm der App ändern (in Regionen, in denen dies bereitgestellt wird)
- Die Werbe-ID über die Einstellungen des Gerätebetriebssystems zurücksetzen/löschen oder personalisierte Werbung einschränken
- Kontakt: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Sicherheitsmaßnahmen

Der Entwickler setzt folgende Maßnahmen um oder bemüht sich um deren Umsetzung:

- Nutzerdaten werden in der Regel lokal auf dem Gerät gespeichert
- Angehängte Bilddateien werden lokal in verschlüsselter Form gespeichert (auf Basis von AES-GCM)
- Informationen zur App-Sperre werden in gehashter Form und nicht im Klartext gespeichert
- Sicherungsdateien werden nach Verschlüsselung auf Grundlage eines Nutzerpassworts gespeichert
- Die Kommunikation mit Drittanbieter-SDKs ist verschlüsselt (HTTPS/TLS)
- Berechtigungen werden mit möglichst geringem Zugriffsumfang verwendet

Risiken, die sich aus dem Sicherheitszustand des Geräts des Nutzers ergeben (wie Rooting/Jailbreak, schädliche Apps oder Offenlegung gemeinsam genutzten Speichers), können jedoch nicht vollständig ausgeschlossen werden.

---

## 11. Hinweise zu sensiblen Daten

Diese App erfordert keine Eingabe sensibler Daten.  
Nutzern wird empfohlen, in Notizen oder Freitextfeldern keine sensiblen Inhalte wie Gesundheitsdaten, politische Ansichten, Religionszugehörigkeit, biometrische Informationen oder Informationen zum Sexualleben einzugeben.

Wenn ein Nutzer freiwillig sensible Inhalte eingibt, können diese Informationen als lokale Daten auf dem vom Nutzer direkt verwalteten Gerät gespeichert werden.

---

## 12. Schutz personenbezogener Daten von Kindern

Diese App ist nicht in erster Linie für Kinder konzipiert.  
Erziehungsberechtigte können die Nutzung über Jugendschutzfunktionen verwalten, die vom Gerät oder vom App-Store bereitgestellt werden.

---

## 13. Automatisierte Entscheidungsfindung

Diese App führt keine automatisierte Entscheidungsfindung auf Grundlage personenbezogener Daten durch, die rechtliche Wirkungen oder ähnlich erhebliche Auswirkungen entfaltet.

---

## 14. Hinweis zur Datensicherheit (Google Play usw.)

Der Entwickler bemüht sich, die Angaben zur Datensicherheit in App-Marktplätzen (wie Google Play) entsprechend den tatsächlichen Verarbeitungspraktiken der App und der tatsächlichen Verarbeitungspraktiken von Drittanbieter-SDKs aufrechtzuerhalten und zu aktualisieren.

Die in App-Stores angezeigten Informationen können jedoch je nach App-Version, Vertriebsland, Konfiguration der Drittanbieter-SDKs und Richtlinienänderungen variieren.

---

## 15. Hinweis zu Open Source

Die App verwendet bestimmte Open-Source-Bibliotheken.  
Informationen zu den entsprechenden Lizenzen finden sich auf dem entsprechenden Bildschirm innerhalb der App oder in Mitteilungen, die über den Vertriebskanal bereitgestellt werden.

---

## 16. Kontakt

Bei Anfragen zu dieser Datenschutzerklärung:

- **Datenschutzbeauftragter / Ansprechpartner:** frog-im
- **E-Mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 17. Änderungen dieser Datenschutzerklärung

Diese Richtlinie kann aufgrund von Änderungen von Gesetzen/Richtlinien, App-Funktionen oder Drittanbieter-SDKs überarbeitet werden.  
Bei wesentlichen Änderungen kann eine Benachrichtigung über Hinweise innerhalb der App, die Vertriebsseite oder Aktualisierungen der Richtlinienseite erfolgen.

Zuletzt aktualisiert: **2026-03-04**
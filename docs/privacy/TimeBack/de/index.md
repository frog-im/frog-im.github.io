---
title: Datenschutzerklärung | TimeBack
description: TimeBack-Datenschutzrichtlinie
lang: de
last_updated: 2026-06-06
---

# Datenschutzrichtlinie (TimeBack)

- **App-Name:** TimeBack
- **Entwickler:** frog-im
- **Kontakt:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Datum des Inkrafttretens:** 03.06.2026
- **Letzte Aktualisierung:** 06.06.2026

Diese Datenschutzrichtlinie basiert auf der aktuellen Implementierung der TimeBack-App. TimeBack bietet Bildschirmzeitüberprüfung, Tagesziele, zurückgewonnene Zeitaufzeichnungen, Reflexionen, Herausforderungen, Benachrichtigungen, Freigabe- und Werbefunktionen.

## 1. Funktionen

TimeBack bietet die folgenden Funktionen:

- Überprüfung der App-Nutzungszeit durch Android-Nutzungszugriffsberechtigung
- Tägliche Nutzungsziele, Erinnerungen und Nutzungsbenachrichtigungen in der Statusleiste
- Warnmeldungen zu festen Grenzwerten und Overlay-Anzeige
- Auswahl der Overlay-Ausnahme-App
- Aktivitätsaufzeichnungen für zurückgewonnene Zeit
- Tägliche Reflexionsaufzeichnungen
- Herausforderungsfortschritt und Checklistenverwaltung
- Bildfreigabe von Nutzungsstatistiken
- Google AdMob-Anzeigen und UMP-basierte Datenschutzoptionen

## 2. Informationen, die wir verarbeiten

### 2-1. Informationen zum Lesen durch Nutzungszugriffsberechtigung

Wenn der Benutzer Android `PACKAGE_USAGE_STATS` die Berechtigung erteilt, kann die App die folgenden Informationen vom Gerät lesen:

- Name des App-Pakets
- App-Name
- App-Nutzungszeit
- Datums- und Zeitbereich, der für die Nutzungsaggregation verwendet wird

Diese Informationen werden verwendet, um Nutzungsstatistiken bereitzustellen und die Nutzung mit den Benutzerzielen zu vergleichen.

### 2-2. Vom Benutzer eingegebene oder konfigurierte Informationen

- Tägliches Nutzungsziel
- Status und Intervall der Aktivierung der Nutzungserinnerung
- Einstellung für die Anzeige der Statusleistennutzung
- Aktivitätskategorie, Titel, Startzeit und Dauer der zurückgeforderten Zeit
- Täglicher Reflexionstext
- Herausforderungsfortschritte und Checklisteneinträge
- Overlay-Ausnahme-App-Liste

### 2-3. Auf dem Gerät gespeicherte Informationen

Die App speichert möglicherweise die folgenden Informationen in einer lokalen SQLite-Datenbank oder SharedPreferences:

- Aufzeichnungen zur App-Nutzungszeit
- Tägliche Ziele und Einstellungen
- Aktivitätsaufzeichnungen für zurückgewonnene Zeit
- Tägliche Reflexionsaufzeichnungen
- Herausforderungsfortschritt und Checklistenstatus
- Onboarding-Abschlussstatus
- Einstellungen wie Nutzungserinnerungen, Hard-Limit-Warnungen, Statusleistenanzeige und Overlay-Ausnahme-Apps
- Status der lokalen Anzeigeneinwilligung und der Datenschutzoption

Basierend auf der aktuellen Implementierung werden diese lokalen Datensätze nicht automatisch auf frog-im-Server hochgeladen.

### 2-4. Werbe- und Einwilligungsdaten

Bei der Verwendung von Google Mobile Ads SDK (AdMob) und UMP können Google oder seine verbundenen Unternehmen Informationen verarbeiten wie:

- Werbekennungen wie Android AD_ID
- IP Adress- und Netzwerkinformationen
- Geräteinformationen, OS-Version und App-Informationen
- Anzeigenimpressionen, Klicks, Messdaten und Fehlersignale
- Anzeigeneinwilligungs- und Datenschutzoptionsstatus
- Ungefährer Standort

## 3. Zwecke der Verarbeitung

Die App verarbeitet Informationen zu folgenden Zwecken:

- Nutzungszeit ablesen, Statistiken anzeigen und Nutzung mit Zielen vergleichen
- Speichern der vom Benutzer eingegebenen Rückgewinnungszeit- und Reflexionsdatensätze
- Verwalten des Herausforderungsfortschritts
- Bereitstellung von Erinnerungen und Statusleistenbenachrichtigungen
- Bereitstellung von Warnmeldungen zu harten Grenzwerten, Overlay-Anzeige und Overlay-Ausnahmebehandlung
- Teilen von Nutzungsstatistikbildern auf Anfrage des Benutzers
- Anzeigen schalten, Anzeigenleistung messen und Optionen zur Anzeigeneinwilligung anwenden
- Aufrechterhaltung der App-Stabilität und Reaktion auf Fehler

## 4. Lokale Speicherung und externe Verarbeitung

### 4-1. Lokaler Speicher

TimeBack speichert Benutzerdaten hauptsächlich im internen Speicher der App auf dem Gerät. Basierend auf der aktuellen Implementierung werden Nutzungsaufzeichnungen, Ziele, Überlegungen und Herausforderungsinformationen nicht automatisch auf frog-im-Server hochgeladen.

Der lokale Speicher kann Folgendes umfassen.

| Lagerung | Gespeicherte Gegenstände | Zweck | Löschmethode |
|---|---|---|---|
| SQLite-Datenbank | App-Nutzungsdatensätze, Paketnamen, App-Namen, Nutzungszeit, datumsbasierte Aggregate | Zeigen Sie Nutzungsstatistiken an und vergleichen Sie die Nutzung mit Zielen | In-App-Löschfunktionen, Löschen von App-Daten oder Deinstallieren der App |
| SQLite-Datenbank | Zurückgewonnene Zeitaktivitäten, Reflexionen, Herausforderungsfortschritte, Checklisteneinträge | Zeigen Sie Aufzeichnungen an und verwalten Sie den Fortschritt | In-App-Löschfunktionen, Löschen von App-Daten oder Deinstallieren der App |
| SharedPreferences | Onboarding-Abschlussstatus, Erinnerungseinstellungen, Einstellungen für Hard-Limit-Warnungen, Einstellungen für die Anzeige der Statusleiste, Overlay-Ausnahme-App-Liste, lokaler Werbeeinwilligungsstatus | Behalten Sie die App-Einstellungen bei | App-Daten löschen oder App deinstallieren |
| Temporäre Dateien/Cache | Freigegebene Nutzungsstatistikbilder und ähnliche temporäre Dateien | Führen Sie die vom Benutzer angeforderte Freigabe durch | Wird nach Möglichkeit nach der Freigabe oder gemäß den Bereinigungsrichtlinien von OS/app gelöscht |

Wenn der Benutzer App-Daten löscht oder die App deinstalliert, werden im Allgemeinen die im internen Speicher der App gespeicherten Daten gelöscht. Android-Backups, Hersteller-Backups, Cloud-Backups oder direkt vom Benutzer freigegebene Dateien können jedoch gemäß den Richtlinien dieser Dienste separat aufbewahrt werden.

Nutzungsaufzeichnungen und Reflexionstexte können persönliche Routinen oder Interessen offenbaren. Auf gemeinsam genutzten Geräten sollten Benutzer geeignete Sicherheitsvorkehrungen wie eine Gerätesperre oder separate OS-Konten verwenden.

### 4-2. Server-Uploads

Basierend auf dem aktuellen Projekt lädt TimeBack Nutzungsdatensätze, Reflexionen oder Challenge-Datensätze nicht automatisch auf frog-im-Server hoch. Wenn der Benutzer die Freigabefunktion nutzt, kann ein generiertes Statistikbild an die vom Benutzer ausgewählte externe App oder den externen Dienst übertragen werden.

### 4-3. Werbeverarbeitung

Google AdMob und UMP werden für In-App-Werbung und Einwilligungsverwaltung verwendet. Werbebezogene Informationen können auf der Google-Infrastruktur verarbeitet werden.

## 5. Dienste und Auftragsverarbeiter von Drittanbietern

### 5-1. Google AdMob / UMP

Zweck:

- Lieferung von Bannerwerbung
- Umgang mit Anzeigeneinwilligungen und Datenschutzoptionen
- Messung der Anzeigenleistung und Betrugsprävention

Informationen, die verarbeitet werden können:

- Werbekennungen
- Geräte- und Netzwerkinformationen
- Informationen zur Anzeigeninteraktion
- Einwilligungs- und Datenschutzoptionsstatus

### 5-2. Teilen von Ziel-Apps oder -Diensten

Wenn der Benutzer direkt die Bildfreigabefunktion für Nutzungsstatistiken verwendet, kann die ausgewählte externe App oder der ausgewählte externe Dienst das freigegebene Bild verarbeiten. Diese Verarbeitung unterliegt den Datenschutzbestimmungen des ausgewählten Dienstes.

## 6. Mitteilung zur grenzüberschreitenden Übertragung

In den folgenden Fällen können Informationen außerhalb des Landes des Nutzers verarbeitet werden.

| Artikel | Details |
|---|---|
| Empfänger | Google LLC und seine Partner |
| Ziel | USA und andere Länder/Regionen, in denen sich die Google-Infrastruktur befindet |
| Timing | Wenn die App ausgeführt wird, Anzeigen anfordert, Anzeigen zeigt oder misst, Klicks verarbeitet oder Einwilligungen verarbeitet |
| Verfahren | Verschlüsselte Netzwerkkommunikation (HTTPS/TLS) |
| Zweck | Anzeigenbereitstellung, Handhabung des Personalisierungsstatus, Messung, Analyse, Verbesserung der Servicestabilität, Einhaltung gesetzlicher Vorschriften |
| Daten | Werbekennungen, Geräte-/App-/Netzwerkinformationen, Informationen zur Anzeigeninteraktion, Einwilligungsstatus, ungefährer Standort usw. |
| Zurückbehaltung | In Übereinstimmung mit den Richtlinien von Google und geltendem Recht |

Einzelheiten finden Sie im [Cross-Border Transfer Notice](./policy/).

## 7. Liste der installierten Apps und Overlay-Ausnahmen

Wenn der Benutzer unter Android Overlay-Ausnahme-Apps konfiguriert, liest die App möglicherweise die Paketnamen und App-Namen startbarer Apps auf dem Gerät, um eine Auswahlliste anzuzeigen. Vom Benutzer als Ausnahmen ausgewählte Paketnamen werden in SharedPreferences auf dem Gerät gespeichert und nur verwendet, um zu vermeiden, dass über diesen Apps Überlagerungen mit Warnungen zu harten Grenzwerten angezeigt werden.

## 8. Aufbewahrung

Die App speichert Informationen gemäß den folgenden Standards:

- Lokale Nutzungs-, Ziel-, Reflexions- und Herausforderungsinformationen: bis der Benutzer sie löscht, App-Daten löscht oder die App deinstalliert
- SharedPreferences-Einstellungen: bis der Benutzer App-Daten löscht oder die App deinstalliert
- Temporäre Dateien für freigegebene Bilder: nach Bedarf für die Freigabe oder gemäß den OS-Bereinigungsrichtlinien
- Werbe- und einwilligungsbezogene Daten: gemäß den Richtlinien von Google und anderen relevanten Dritten

## 9. Berechtigungen

Die App kann die folgenden Berechtigungen verwenden:

- `PACKAGE_USAGE_STATS`: App-Nutzungszeit lesen
- `POST_NOTIFICATIONS`: Nutzungserinnerungen und Statusleistenbenachrichtigungen anzeigen
- `SYSTEM_ALERT_WINDOW`: Überlagerungen mit Hard-Limit-Warnungen anzeigen
- `INTERNET`: Kommunizieren Sie mit Anzeige SDKs und zeigen Sie Seiten mit rechtlichen Hinweisen an
- `ACCESS_NETWORK_STATE`: Netzwerkstatus prüfen
- `com.google.android.gms.permission.AD_ID`: Werbekennungen verwenden

Berechtigungen werden nur bei Bedarf für App-Funktionen verwendet. Benutzer können Berechtigungen in den Geräteeinstellungen widerrufen, die damit verbundenen Funktionen sind jedoch möglicherweise eingeschränkt.

## 10. Benutzerrechte und Wahlmöglichkeiten

Benutzer können:

- Datensätze in der App anzeigen, bearbeiten oder löschen
- Löschen Sie lokale Informationen, indem Sie App-Daten löschen oder die App deinstallieren
- Ändern Sie die Einstellungen für Nutzungszugriff, Benachrichtigung und Werbekennung in den Geräteeinstellungen
- Widerrufen Sie die Overlay-Berechtigung und ändern Sie die App-Einstellungen für Overlay-Ausnahmen
- Ändern Sie die Datenschutzoptionen für Anzeigen
- Kontaktieren Sie uns bei Fragen zum Datenschutz oder Löschanfragen

Kontakt-E-Mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Sicherheitsmaßnahmen

Die App wendet die folgenden Sicherheitsmaßnahmen an oder kann diese anwenden:

- HTTPS/TLS-basierte externe Kommunikation
- Lokale Datenverarbeitung
- Für App-Funktionen sind minimale Berechtigungsanfragen erforderlich
- Anwendung des Werbeeinwilligungsstatus

Gerätesicherheitsbedingungen wie Rooting, Jailbreaking, Malware oder die Nutzung gemeinsam genutzter Geräte können zusätzliche Risiken schaffen.

## 12. Privatsphäre von Kindern

TimeBack ist nicht in erster Linie für Kinder konzipiert. Während der Werbung und Einwilligungsverarbeitung können altersbezogene Einstellungen oder Plattformrichtlinien von Google Mobile Ads SDK und UMP gelten.

## 13. Änderungen

Diese Richtlinie kann aufgrund von Gesetzesänderungen, Änderungen an der Konfiguration von Drittanbieterdiensten oder App-Funktionen aktualisiert werden. Wesentliche Änderungen werden durch eine In-App-Benachrichtigung oder durch Aktualisierung dieser Seite mitgeteilt.

## 14. Kontakt

- Entwickler: frog-im
- E-Mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

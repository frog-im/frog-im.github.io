---
title: Datenschutzerklärung | QDiary
description: Datenschutzerklärung von QDiary
---

# Datenschutzerklärung (QDiary)

- App-Name: QDiary
- Entwickler: frog-im
- Kontakt: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Inkrafttretensdatum: 2026-04-19
- Letzte Aktualisierung: 2026-04-19

Diese Datenschutzerklärung wurde auf Grundlage der aktuellen Implementierung der QDiary-App erstellt. QDiary bietet Funktionen zum Schreiben von Tagebucheinträgen, zur Generierung und Reflexion von Quests, zum Login, zur manuellen Cloud-Speicherung, zu Werbung und zu Benachrichtigungen. In diesem Zusammenhang können personenbezogene Daten oder Informationen, die personenbezogene Daten darstellen können, im erforderlichen Umfang verarbeitet werden.

## 1. Bereitgestellte Funktionen

QDiary bietet die folgenden Funktionen:

- Schreiben, Bearbeiten und Anzeigen von Tagebucheinträgen
- Kategorisierung und Kalenderansicht
- Quest-Generierung, Quest-Reflexion und Verarbeitung des Quest-Abschlusses
- Lokale Sperrfunktion der Tagebuch-App und lokale Verschlüsselung
- E-Mail-Login, E-Mail-Verifizierung, anonymer (Gast-)Login und Zurücksetzen des Passworts
- Vom Nutzer ausgelöste Cloud-Speicherung und -Ladung
- Anzeige von Werbung und Verarbeitung von Datenschutzoptionen für Werbung
- Quest-Erinnerungsbenachrichtigungen

## 2. Kategorien der verarbeiteten Informationen

### 2-1. Vom Nutzer direkt eingegebene Informationen

- E-Mail-Adresse
- Passwort
- Titel, Inhalt, Datum, Kategorie und Schwierigkeitsgrad des Tagebucheintrags
- Quest-Antworten, Reflexionsinhalte und Informationen zur ausgewählten Quest
- Ausgewählte Werte im Zusammenhang mit dem Quest-Profil und Zusammenfassungstext
- Passphrase für die Sperrfunktion der Tagebuch-App

### 2-2. Von der App auf dem Gerät gespeicherte Informationen

- Lokale Tagebuch-Datenbank (SQLite)
- Quest-Statusinformationen für lokale Tagebücher
- Statuswerte zu Anwesenheit, Einstellungen, Sprache, Benachrichtigungen und Werbung
- Prüfwerte für die App-Sperre, Salt und Verschlüsselungs-Metadaten
- Informationen zur Planung von Quest-Benachrichtigungen

### 2-3. Konto- und Identifikationsinformationen

Die folgenden Informationen können über Firebase Authentication verarbeitet werden:

- Firebase-UID
- E-Mail-Adresse
- Ob die E-Mail-Verifizierung abgeschlossen wurde
- Ob ein anonymer Login verwendet wird

### 2-4. Informationen zu Werbung und Einwilligung

Bei der Verwendung von Google AdMob und dem UMP SDK können die folgenden Informationen verarbeitet werden:

- Werbe-IDs (z. B. Android AD_ID)
- IP-Adresse und Netzwerkinformationen
- Geräteinformationen, Betriebssystemversion und App-Informationen
- Informationen zu Werbeeinblendungen, Klicks und zur Verarbeitung von Belohnungen
- Status der Werbeeinwilligung und der Datenschutzoptionen

### 2-5. Informationen im Zusammenhang mit Benachrichtigungen

- Ob die Benachrichtigungsberechtigung erteilt wurde
- Identifikationswerte für Tagebücher mit laufenden Quests
- Text der Quest-Benachrichtigung
- Geplante Zeiten für Benachrichtigungen

## 3. Zwecke der Verarbeitung

Die App verarbeitet Informationen zu den folgenden Zwecken:

- Registrierung, Login, E-Mail-Verifizierung und Zurücksetzen des Passworts
- Schreiben, Speichern und Anzeigen von Tagebucheinträgen
- Quest-Generierung, Reflexion und Feststellung des Quest-Abschlusses
- Lokale Ver- und Entschlüsselung im Zusammenhang mit der App-Sperre
- Vom Nutzer angeforderte Cloud-Speicherung und -Ladung
- Bereitstellung von Quest-Benachrichtigungen
- Bereitstellung von Werbung, Verarbeitung von Werbebelohnungen und Berücksichtigung des Status der Werbeeinwilligung
- Sicherheit, Fehlerbehandlung und Betrieb des Dienstes

## 4. Lokale Speicherung, Cloud-Speicherung und externe Verarbeitung

### 4-1. Lokale Speicherung

Tagebuch- und Quest-Informationen werden in erster Linie in der lokalen Datenbank des Geräts gespeichert.

- Wenn die App-Sperre nicht aktiviert ist: lokale Speicherung in allgemeiner Form
- Wenn die App-Sperre aktiviert ist: Einige Informationen, wie z. B. der Titel, der Inhalt und der Quest-Status des Tagebuchs, können lokal verschlüsselt gespeichert werden

### 4-2. Cloud-Speicherung

Die App speichert Daten in Firebase Firestore nur dann, wenn der Nutzer die Funktion `Save` direkt ausführt.

Gemäß der aktuellen Projektkonfiguration:

- Es wird keine automatische vollständige Synchronisierung verwendet
- Daten werden nur dann in Firestore `savedDiaries` gespeichert, wenn der Nutzer sie manuell speichert
- Beim Speichern können der Tagebuchtitel, der Inhalt und der Quest-Status je nach aktuellem Status der App-Sperre in verschlüsselter Form gespeichert werden
- Daten werden nur dann zurück in den lokalen Speicher geladen, wenn der Nutzer `Load` ausführt

### 4-3. Externe Verarbeitung für Quest-Generierung und Reflexion

Wenn der Nutzer eine Quest-Generierung oder Reflexion anfordert, können die folgenden Informationen über Firebase Functions für eine externe Verarbeitung verwendet werden:

- Titel des Tagebucheintrags
- Inhalt des Tagebucheintrags oder Reflexionsinhalts
- Kategorie
- Schwierigkeitsgrad
- Ausgewählte Quest
- Zusammenfassungsinformationen zum Quest-Profil

Diese Informationen werden für die Generierung und Auswertung von Quests über die OpenAI API verwendet.

Wichtig:

- Relevante Tagebuchinhalte werden nur dann für eine externe Verarbeitung verwendet, wenn die Quest-Funktion genutzt wird.
- Gemäß der aktuellen Projektkonfiguration wird kein Code verwendet, der Quest-Protokolle in einer separaten `questLogs`-Sammlung speichert.

## 5. Drittanbieterdienste und Auftragsverarbeitung

### 5-1. Google Firebase

Zweck:

- Authentifizierung (Firebase Authentication)
- Speicherung in Firestore
- Ausführung von Cloud Functions

Informationen, die verarbeitet werden können:

- UID, E-Mail-Adresse und Authentifizierungsstatus
- Vom Nutzer manuell gespeicherte Tagebuchdaten
- Daten zu Quest-Anfragen

### 5-2. OpenAI

Zweck:

- Quest-Generierung
- Quest-Reflexion und Bewertung des Quest-Abschlusses

Informationen, die verarbeitet werden können:

- Titel/Inhalt des Tagebucheintrags
- Quest-Text
- Schwierigkeitsgrad und Kategorie
- Vom Nutzer eingegebener Reflexionsinhalt
- Zusammenfassungsinformationen zum Quest-Profil

### 5-3. Google AdMob / UMP

Zweck:

- Bereitstellung von Banner-, Interstitial- und Rewarded-Werbung
- Verarbeitung der Werbeeinwilligung und Datenschutzoptionen

Informationen, die verarbeitet werden können:

- Werbe-IDs
- Geräte- und Netzwerkinformationen
- Informationen zur Werbeinteraktion
- Einwilligungsstatus

## 6. Hinweis zur internationalen Datenübermittlung

Die App kann personenbezogene Daten oder damit zusammenhängende Informationen in den folgenden Fällen außerhalb des Landes des Nutzers verarbeiten:

| Punkt | Details |
|---|---|
| Empfänger | Google LLC, OpenAI und zugehörige Infrastrukturbetreiber |
| Bestimmungsland | Vereinigte Staaten usw. |
| Zeitpunkt der Übermittlung | Beim Login, bei der Quest-Generierung/-Reflexion, bei Werbeanfragen und bei der Verarbeitung der Einwilligung |
| Art der Übermittlung | Verschlüsselte Netzwerkkommunikation |
| Zweck der Übermittlung | Authentifizierung, Datenspeicherung, serverlose Verarbeitung, KI-gestützte Quest-Generierung/-Bewertung und Bereitstellung von Werbung |

## 7. Aufbewahrungs- und Nutzungsdauer

Die App speichert Informationen nach den folgenden Standards:

- Lokale Tagebuch-/Einstellungsinformationen: bis der Nutzer sie löscht oder die App deinstalliert
- Firebase-Kontoinformationen: solange der Nutzer das Konto beibehält
- In Firestore gespeicherte Daten: solange der Nutzer die gespeicherten Elemente behält
- Daten zur Verarbeitung von Quest-Anfragen: soweit für die serverlose Verarbeitung erforderlich
- Daten im Zusammenhang mit Werbung/Einwilligung: gemäß den Richtlinien der jeweiligen externen Anbieter

Darüber hinaus enthält das aktuelle Projekt die folgende automatische Bereinigungslogik:

- Bereinigung anonymer Nutzerkonten und von Firestore-Daten in untergeordneten Sammlungen nach einem bestimmten Zeitraum
- Bereinigung lange inaktiver regulärer Nutzerkonten und von Firestore-Daten in untergeordneten Sammlungen

Ob dies tatsächlich in der Produktionsumgebung umgesetzt wird, kann jedoch je nach Bereitstellungsstatus und Serverkonfiguration variieren.

## 8. Hinweis zur App-Sperre und lokalen Verschlüsselung

Die App bietet eine separate Funktion `Diary App Lock`.

- Die Passphrase für die App-Sperre ist vom Kontopasswort getrennt.
- Die Passphrase für die App-Sperre wird zur lokalen Ver- und Entschlüsselung des Tagebuchs verwendet.
- Auch wenn eine falsche Passphrase eingegeben wird, wird die App selbst möglicherweise nicht immer vollständig gesperrt; stattdessen können einige Tagebuchinhalte unlesbar bleiben.
- Einige Tagebücher können je nach der beim Schreiben oder bei der vorübergehenden Entsperrung verwendeten Passphrase separat verschlüsselt werden.

Nutzer sollten ihre Passphrase sicher aufbewahren. Wenn sie verloren geht, kann die Wiederherstellung einiger lokaler Daten schwierig sein.

## 9. Hinweis zu Quest-Benachrichtigungen

Wenn der Nutzer Quest-Benachrichtigungen aktiviert, können lokale Benachrichtigungen für jedes Tagebuch mit einer laufenden Quest geplant werden.

- Die Planung wird hauptsächlich durch die interne Geräteplanung verarbeitet.
- Gemäß der aktuellen Projektkonfiguration ist keine Struktur bestätigt, bei der der Originaltext des Tagebuchs ausschließlich zu Benachrichtigungszwecken periodisch an einen zentralen Server übertragen wird.

## 10. Hinweis zur Verwendung von Berechtigungen

Die App kann die folgenden Berechtigungen verwenden, um ihre Funktionen bereitzustellen:

- `INTERNET`: Kommunikation mit Firebase, OpenAI und Werbe-SDKs
- `com.google.android.gms.permission.AD_ID`: Verwendung von Werbe-IDs
- `POST_NOTIFICATIONS`: Anzeige von Quest-Benachrichtigungen
- `RECEIVE_BOOT_COMPLETED`: Wiederherstellung geplanter Benachrichtigungen nach einem Neustart des Geräts

Berechtigungen werden nur in dem Umfang verwendet, der zur Ausführung der jeweiligen Funktionen erforderlich ist.

## 11. Rechte der betroffenen Person und deren Ausübung

Nutzer können die folgenden Rechte ausüben:

- Zugriff auf Daten innerhalb der App sowie deren Änderung und Löschung
- Löschen oder Überschreiben von in der Cloud gespeicherten Daten
- Anforderung von Logout und Kontolöschung
- Änderung der Datenschutzoptionen für Werbung
- Deaktivierung von Benachrichtigungsberechtigungen

So können diese Rechte ausgeübt werden:

- Direktes Löschen oder Bearbeiten von Tagebucheinträgen innerhalb der App
- Löschen der App oder Zurücksetzen lokaler Daten
- Abmeldung vom Konto und separate Anforderung der Löschung
- Änderung von Benachrichtigungen, Werbe-IDs und Berechtigungen in den Geräteeinstellungen
- Kontakt-E-Mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Sicherheitsmaßnahmen

Die App wendet die folgenden Schutzmaßnahmen an oder kann sie anwenden:

- HTTPS-basierte Kommunikation
- Lokale Sperrfunktion und Verschlüsselung der Tagebuch-App
- Getrennte Speicherung der Prüfwerte der Passphrase
- Verwendung von Firebase Authentication
- Anforderung minimaler Berechtigungen

Es können jedoch Risiken entstehen, abhängig vom Sicherheitsstatus des Geräts des Nutzers, etwa bei Rooting, Jailbreaking, Malware oder der Nutzung eines gemeinsam verwendeten Geräts.

## 13. Personenbezogene Daten von Kindern

Die App ist nicht als Dienst konzipiert, der sich in erster Linie an Kinder richtet. Allerdings können im Rahmen der Verarbeitung von Werbung und Einwilligungen altersbezogene Optionen innerhalb von UMP angewendet werden.

## 14. Änderungen dieser Erklärung

Diese Erklärung kann aufgrund von Änderungen der Rechtslage, von Drittanbieterdiensten oder von App-Funktionen überarbeitet werden.

- Letzte Aktualisierung für die aktuelle Version: **2026-04-19**

## 15. Kontakt

- Entwickler: frog-im
- E-Mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Anleitung zur Kontolöschung: [Löschanleitung](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)


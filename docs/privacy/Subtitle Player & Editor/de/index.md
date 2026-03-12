---
title: Datenschutzerklärung | Subtitle Tool
description: Datenschutzerklärung für Subtitle Tool (Subtitle Player & Editor) - Deutsch
lang: de
last_updated: 2026-03-11
---

# Datenschutzerklärung (Subtitle Tool / Subtitle Player & Editor)

- **App-Name:** Subtitle Player & Editor (in dieser Richtlinie auch als **Subtitle Tool** bezeichnet)
- **Entwickler:** frog-im
- **Kontakt:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Inkrafttreten:** 2026-03-11

> Diese Richtlinie wurde unter Bezugnahme auf geltende Gesetze erstellt, darunter das koreanische Gesetz zum Schutz personenbezogener Daten (PIPA), die DSGVO / UK GDPR, das Schweizer DSG sowie einschlägige Datenschutzgesetze einzelner US-Bundesstaaten. Soweit zwingende lokale Vorschriften gelten, haben diese Vorrang.

---

## 1. Zweck und Geltungsbereich

Diese App bietet:

- Wiedergabe und Bearbeitung von Untertiteln
- Video- und Untertitelwiedergabe aus vom Nutzer ausgewählten Dateien
- Schwebende Untertitel-/Liedtext-Overlays, die auf Android über anderen Apps angezeigt werden

Die unterstützte Untertitelverarbeitung kann Formate wie die folgenden umfassen:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

Die App erstellt **kein** Benutzerkonto und lädt Benutzer-Untertitel- oder Mediendateien **nicht** auf die eigenen Server des Entwicklers hoch. Das Parsen, Bearbeiten, Vorschauen und der Großteil der wiedergabebezogenen Verarbeitung erfolgen **lokal auf dem Gerät**.

Für Werbung, Einwilligungsverwaltung und rechtliche Compliance können jedoch Drittanbieter-SDKs wie **Google Mobile Ads SDK (AdMob)** und **Google UMP** bestimmte Informationen verarbeiten, z. B. Werbe-IDs, Gerätesignale und Einwilligungsentscheidungen.

---

## 2. Kategorien der von uns verarbeiteten Informationen

### 2-1) Vom Nutzer ausdrücklich ausgewählte Dateien

Die App verarbeitet Dateien, die der Nutzer ausdrücklich auswählt, darunter:

- **Untertiteldateien**
  - Beispiele: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Verwendungszwecke:
    - Untertitelwiedergabe innerhalb der App
    - Bearbeitung von Untertiteln
    - Anzeige von Overlay-Untertiteln
    - Konvertierung und Export von Untertiteln

- **Mediendateien**
  - Beispiele: lokale Video- oder Audiodateien, die der Nutzer auswählt
  - Verwendungszwecke:
    - Video- und Untertitelwiedergabe
    - Timing-Abgleich des Overlays mit aktuell wiedergegebenen Medien

Wichtige Hinweise:

- Vom Nutzer ausgewählte Dateien werden lokal auf dem Gerät verarbeitet.
- Die App lädt diese Dateien nicht auf die eigenen Server des Entwicklers hoch.
- Dateipfade und Dateiinhalte werden nur für Wiedergabe, Overlay, Bearbeitung, Speichern und vom Nutzer angeforderte Aktionen verwendet.

### 2-2) Lokale Einstellungen und gespeicherte Werte

Um dauerhafte Einstellungen bereitzustellen und einen vorherigen Zustand wiederherzustellen, speichert die App einige Werte lokal auf dem Gerät mithilfe von `SharedPreferences` oder ähnlichem vom Betriebssystem bereitgestelltem lokalen Speicher.

Diese Werte werden nicht an die eigenen Server des Entwicklers gesendet und normalerweise entfernt, wenn die App-Daten gelöscht oder die App deinstalliert wird.

#### (1) Overlay-Einstellungen

Beispiele sind:

- `overlay_box_x`
- `overlay_box_y`
- `overlay_text_font`
- `overlay_text_color`
- `overlay_outline_enabled`
- `overlay_outline_color`
- `overlay_outline_width`
- `overlay_force_landscape`
- `overlay_interstitial_count`

Zweck:

- Wiederherstellung der Overlay-Position
- Wiederherstellung des Untertitelstils für das Overlay und die Untertitelwiedergabe in der App
- Beibehaltung von Einstellungen für Kontur / Schriftart / Ausrichtung
- Steuerung der Anzeigenhäufigkeit in bestimmten overlaybezogenen Abläufen

#### (2) Kürzliche Wiedergabe- oder Overlay-Positionen

Beispiele sind:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Zweck:

- Wiederherstellung oder Vorschlag kürzlicher Startpositionen für Untertitel/Overlay
- Komfortableres Fortsetzen der Video- und Untertitelwiedergabe

#### (3) Werbe- und Datenschutzeinstellungen

Beispiele können sein:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Zweck:

- Speicherung von Datenschutzentscheidungen für Werbung
- Anwendung von UMP-/AdMob-Datenschutz- und Anzeigenkonfigurationen

#### (4) Vom Nutzer erstellte Untertitel-Ausgabedateien

Wenn der Nutzer Untertiteldateien speichert oder exportiert, kann die App neue Untertiteldateien an einen vom Nutzer ausgewählten Ort schreiben, zum Beispiel:

- Downloads
- einen anderen über den System-Dateiauswahldialog gewählten Ordner
- einen vom Nutzer verwalteten Speicherort

Diese vom Nutzer gespeicherten Dateien können nach dem Löschen der App auf dem Gerät verbleiben, sofern der Nutzer sie nicht manuell löscht.

#### (5) Temporäre Dateien und Cache

Die App und Drittanbieterbibliotheken können für den normalen Betrieb temporäre Dateien oder Cache-Dateien erstellen, zum Beispiel:

- Cache-Daten des Dateiauswahldialogs
- temporäre Daten für die Untertitelkonvertierung
- wiedergabebezogene Cache-Daten

Diese dienen ausschließlich dem lokalen Betrieb und werden nicht auf die eigenen Server des Entwicklers hochgeladen.

#### (6) UMP-Einwilligungsstatus-Cache

In Regionen, in denen Google UMP gilt, kann das SDK den Einwilligungsstatus lokal auf dem Gerät zwischenspeichern.

Dies kann in der Regel zurückgesetzt werden durch:

- Löschen der App-Daten oder
- Ändern der Einwilligungsentscheidungen innerhalb der App, sofern dort ein Eintrag für Datenschutzoptionen verfügbar ist

### 2-3) Android-Overlay und verarbeitungsbezogene Berechtigungen

Unter Android kann das schwebende Untertitel-Overlay Folgendes verwenden:

- `SYSTEM_ALERT_WINDOW` / Berechtigung zum Anzeigen über anderen Apps
- `POST_NOTIFICATIONS`-Berechtigung
- eine für den Overlay-Dienst erforderliche Vordergrunddienst-Benachrichtigung

Zweck:

- Anzeige des Untertitel-Overlays über anderen Apps
- Aufrechterhaltung des Overlay-Dienstes
- Ermöglichen der erforderlichen Overlay-/Dienstbenachrichtigungen durch Android
- Lesen von Medienbenachrichtigungsinformationen, wenn dies für die Unterstützung des Untertitelfortschritts erforderlich ist

Diese Berechtigungen werden nur für App-Funktionen verwendet, die der Nutzer tatsächlich verwenden möchte.

### 2-4) Werbung, Einwilligung und damit verbundene Daten (Drittanbieter-SDKs)

Die App verwendet Google-Werbe-/Einwilligungs-SDKs, darunter:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

Die App kann Folgendes anzeigen:

- Banneranzeigen
- Interstitial-Anzeigen
- Rewarded- oder Rewarded-Interstitial-Anzeigen

Diese SDKs können Daten wie die folgenden verarbeiten:

- Werbe-IDs (zum Beispiel AAID / IDFA, soweit anwendbar)
- IP-basierte und netzwerkbezogene Informationen
- Geräte- und App-Metadaten
- Signale zur Anzeigeninteraktion
- Einwilligungsentscheidungen

Die Zwecke können unter anderem sein:

- Auslieferung von Werbung
- Anzeigenmessung und Berichterstattung
- Frequenzbegrenzung
- Betrugsprävention
- rechtliche Compliance

Der Entwickler bemüht sich, diese SDKs in einer Weise zu konfigurieren, die mit den Einwilligungsentscheidungen der Nutzer und dem geltenden Recht vereinbar ist.

---

## 3. Wie wir Daten verarbeiten und speichern

- **Lokale Einstellungen und Daten zu letzten Positionen**
  - werden auf dem Gerät gespeichert, bis die App-Daten gelöscht oder die App entfernt wird

- **Temporäre Dateien / Cache**
  - werden nur so lange gespeichert, wie sie für den Betrieb erforderlich sind, und anschließend, soweit praktikabel, von der App entfernt oder später vom Betriebssystem bereinigt

- **Vom Nutzer gespeicherte Untertiteldateien**
  - verbleiben am vom Nutzer gewählten Speicherort, bis der Nutzer sie löscht

- **Werbe-/Einwilligungsdaten, die von Dritten verarbeitet werden**
  - werden gemäß den Google-Richtlinien und dem geltenden Recht gespeichert

---

## 4. Verarbeitung durch Dritte und grenzüberschreitende Datenübermittlungen

Für Werbung und Einwilligungsverwaltung können einige Informationen von Google und verbundenen Partnern verarbeitet werden.

| Punkt | Details |
|---|---|
| Empfänger | Google LLC und verbundene Unternehmen / Auftragsverarbeiter |
| Zweck | Auslieferung von Werbung, Messung, Betrugsprävention, Einwilligungsverwaltung und rechtliche Compliance |
| Mögliche Daten | Werbe-IDs, Geräte-/App-Informationen, IP-basierte Informationen, Anzeigeninteraktionsdaten, Einwilligungsstatus |
| Zielort | Vereinigte Staaten und andere Regionen, in denen die Google-Infrastruktur betrieben wird |
| Speicherdauer | Gemäß den Google-Richtlinien und dem geltenden Recht |

Der Entwickler bemüht sich, die Datenschutzangaben in den App-Stores mit dem tatsächlichen Verhalten der verwendeten SDKs in Einklang zu halten.

---

## 5. Ihre Rechte und Wahlmöglichkeiten

Je nach Ihrer Rechtsordnung können Sie Rechte haben, wie zum Beispiel:

- Auskunft
- Berichtigung
- Löschung
- Einschränkung
- Datenübertragbarkeit
- Widerspruch
- Widerruf der Einwilligung, sofern die Einwilligung die Rechtsgrundlage ist

Praktische Kontrollmöglichkeiten umfassen:

- Änderung von Werbe-/Datenschutzentscheidungen in der App, sofern verfügbar
- Löschen der App-Daten, um lokale Einstellungen und zwischengespeicherte Präferenzen zu entfernen
- Deinstallation der App
- manuelles Löschen exportierter Untertiteldateien aus dem Nutzerspeicher
- Nutzung von Betriebssystem-Steuerungen wie Benachrichtigungseinstellungen, Zurücksetzen der Werbe-ID oder Einstellungen zur Anzeigenpersonalisierung

Für von Google verarbeitete Daten sollten Nutzer gegebenenfalls auch die eigenen Datenschutz- und Kontotools von Google konsultieren.

---

## 6. Datenschutz für Kinder

Diese App ist nicht in erster Linie für Kinder bestimmt.

Ihr Hauptzweck ist die Wiedergabe und Bearbeitung von Untertiteln, die Anzeige von Overlays und damit verbundene Hilfsfunktionen. Soweit erforderlich, kann die Konfiguration der Werbe-SDKs altersbezogene oder auf Kinder gerichtete Kennzeichnungen entsprechend den Plattformanforderungen und den Einstellungen des Entwicklers anwenden.

---

## 7. Sicherheitsmaßnahmen

Im Rahmen der Architektur der App bemüht sich der Entwickler:

- die Datenerhebung zu minimieren, indem die meiste Untertitel- und Medienverarbeitung auf dem Gerät erfolgt
- System-Dateiauswahldialoge und vom Nutzer ausgelösten Dateizugriff zu verwenden
- Systemberechtigungen transparent zu nutzen
- sich, soweit anwendbar, auf verschlüsselte Netzwerkübertragung durch Drittanbieter-SDKs zu verlassen

Keine Methode der Speicherung oder Übertragung ist vollkommen sicher, aber die App ist so konzipiert, dass unnötige Datenerhebung durch den Entwickler vermieden wird.

---

## 8. Open-Source-Software

Die App verwendet Open-Source-Software, darunter Bibliotheken in Bezug auf:

- Untertitel-Parsing und -Serialisierung
- Dateiauswahl
- lokale Präferenzen
- Overlay-Fenster
- Videowiedergabe
- WebView

Hinweise zu Open-Source-Software sind innerhalb der App verfügbar. Für einige Komponenten kann die App eine lokal modifizierte Kopie eines Open-Source-Pakets verwenden, wobei der ursprüngliche Lizenzhinweis erhalten bleibt.

---

## 9. Kontakt

Wenn Sie Fragen oder datenschutzbezogene Anfragen haben:

- **E-Mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Bitte geben Sie in Ihrer Nachricht den App-Namen **Subtitle Player & Editor** an.

---

## 10. Änderungen dieser Richtlinie

Diese Richtlinie kann aktualisiert werden, wenn:

- sich App-Funktionen ändern
- sich Berechtigungen oder die Nutzung von SDKs ändern
- sich gesetzliche oder plattformbezogene Anforderungen ändern

Wesentliche Änderungen werden in der aktualisierten Richtlinienseite und, soweit angemessen, in der App selbst dargestellt.

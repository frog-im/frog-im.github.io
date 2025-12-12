---
title: Datenschutzrichtlinie | Subtitle Tool
description: Datenschutzrichtlinie für Subtitle Player & Editor (Subtitle Tool)
lang: de
last_updated: 2025-12-12
---

# Datenschutzrichtlinie (Subtitle Player & Editor / „Subtitle Tool“)

- **App-Name:** Subtitle Player & Editor (im Folgenden „Subtitle Tool“)  
- **Entwickler:** frog-im  
- **Kontakt:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Geltungsbeginn:** 12.12.2025  

> Diese Richtlinie wird unter Bezugnahme auf einschlägige Gesetze erstellt, darunter das koreanische Datenschutzgesetz (PIPA), die DSGVO / UK-DSGVO, das schweizerische Datenschutzgesetz (FADP) sowie verschiedene US-US-Bundesstaatsgesetze zum Datenschutz.  
> Soweit besondere Anforderungen einzelner Rechtsordnungen bestehen, haben diese Vorrang.

---

## 1. Zweck und Anwendungsbereich

Diese App bietet Funktionen zur **Bearbeitung von Metadaten von Audiodateien** (Titel, Künstler usw.), die auf dem Gerät gespeichert sind, sowie eine **Lyrics-/Untertitel-Overlay-Funktion**.  
Die App **legt kein Benutzerkonto an** und lädt **keine Inhalte des Nutzers** auf eigene Server hoch. Die Verarbeitung erfolgt standardmäßig **auf dem Gerät des Nutzers**.

Zu Zwecken der **Werbung** und des **rechtlichen Compliance-Managements** können jedoch Drittanbieter (z. B. Google Mobile Ads SDK (AdMob), UMP) Informationen wie **Werbe-IDs** verarbeiten.  
Die Einholung von Einwilligungen und die Verwaltung von Datenschutzeinstellungen erfolgen gemäß den Spezifikationen der **Google User Messaging Platform (UMP)**.

---

## 2. Kategorien von verarbeiteten Informationen

### 2-1) Vom Nutzer ausdrücklich ausgewählte Dateien

- **Audiopfad / Cover-Bilder und Inhalte:** werden **lokal** auf dem Gerät verarbeitet und ausschließlich zur Bearbeitung und Speicherung verwendet.  
- **FFmpegKit** wird lokal für Encoding, Metadatenbearbeitung und Thumbnail-Erstellung eingesetzt.  
- Die App **lädt diese vom Nutzer ausgewählten Dateien nicht** auf unsere Server hoch.

### 2-2) Lokale Einstellungen und gespeicherte Werte

Für Grundfunktionen und Bedienkomfort speichert die App die folgenden Werte **lokal auf dem Gerät**.  
Diese Daten werden nicht an unsere Server übermittelt und **bei Löschung der App oder ihrer Daten entfernt**.

#### (1) Präferenzen (`shared_preferences`)

| Typ | Schlüssel / Inhalt | Zweck | Speicherort | Löschung |
|---|---|---|---|---|
| Overlay-Position / Schrift | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Wiederherstellung von Overlay-Position und Schriftgröße | SharedPreferences des Geräts | Wird bei App-Daten-Löschung oder Deinstallation entfernt |
| Anzeigen-/Datenschutz-Einstellungen | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Nicht-personalisierte Werbung, U.S. RDP-Signal, COPPA-Tag, Alterskennzeichnung, Limit für Anzeigeninhalte | SharedPreferences des Geräts | Wie links |

#### (2) Temporäre Dateien (temporäres Systemverzeichnis)

- **Beispiele:** `cover_*.jpg`, `tmp_*.flac`  
- **Verwendung:** Cover-Extraktion, FLAC-Tagging, temporäres Encoding  
- **Speicherort:** temporäres Verzeichnis des Betriebssystems (`systemTemp`)  
- **Aufbewahrung:** werden nach Möglichkeit nach Abschluss der Verarbeitung gelöscht; ggf. zusätzlich durch das Betriebssystem bereinigt.

#### (3) Vom Nutzer gewählte Speicherorte (SAF)

- Wenn der Nutzer „Speichern unter“ verwendet, können endgültige Audiodateien an vom Nutzer ausgewählte Speicherorte geschrieben werden (z. B. Downloads, Cloud-Speicher).  
- Diese Dateien liegen im **externen Speicher** und **können nach Deinstallation der App erhalten bleiben**. Der Nutzer kann sie manuell löschen.

#### (4) Einwilligungsstatus (UMP-Cache)

- In EWR/Vereinigtes Königreich/Schweiz speichert das UMP-SDK den **Werbe-Einwilligungsstatus des Nutzers lokal im Cache**.  
- Dieser lässt sich durch Löschen der App-Daten oder über den **Datenschutz-Optionen-Bildschirm** in der App zurücksetzen (sofern verfügbar).

---

### 2-3) Anzeigendaten und Einwilligungsdaten (Drittanbieter-SDKs)

- **Google Mobile Ads SDK (AdMob) und UMP** können u. a. folgende Daten verarbeiten: **Werbe-IDs (AAID/IDFA)**, **IP-Bereiche**, **Geräte-/App-Informationen**, **Interaktionssignale mit Anzeigen**, **Einwilligungsstatus** usw.  
- **Zwecke:** Auslieferung von Anzeigen, Frequenzbegrenzung, Betrugsprävention, Performance-Messung, rechtliche Compliance.  
- **Regionen mit Einwilligungspflicht (EWR/UK/CH):** Einwilligungen werden mittels UMP-Dialogen eingeholt; ein **Datenschutz-Optionen-Bildschirm** wird bereitgestellt, sofern rechtlich erforderlich.  
  In Regionen ohne entsprechende Vorgaben (z. B. Korea) **kann diese Option entfallen**.

---

## 3. Verarbeitung und Aufbewahrungsdauer

- **Lokale Einstellungen:** bleiben auf dem Gerät gespeichert, bis der Nutzer die App-Daten löscht oder die App deinstalliert.  
- **Temporäre Dateien:** werden während Encoding/Extraktion angelegt und nach Abschluss des Prozesses gelöscht oder können vorübergehend in System-Caches bestehen bleiben.  
- **Anzeigen-/Einwilligungsdaten (Drittanbieter):** werden gemäß den **Richtlinien von Google** aufbewahrt und gelöscht.

---

## 4. Weitergabe an Dritte und grenzüberschreitende Datenübermittlungen

Für Werbung und Einwilligungsverwaltung können bestimmte Nutzerdaten an die Infrastruktur von Google übermittelt und dort verarbeitet werden.

| Punkt | Details |
|---|---|
| **Empfänger** | Google LLC sowie verbundene Unternehmen / Unterauftragsverarbeiter |
| **Zielregion** | USA (sowie weitere Regionen, in denen Googles Infrastruktur betrieben wird) |
| **Zweck** | Anzeigenauslieferung, Messung und Performance, rechtliche Compliance, Einwilligungsmanagement |
| **Daten** | Werbe-IDs, IP-Bereiche, Geräte-/App-Informationen, Anzeigeninteraktionen, Einwilligungsstatus usw. |
| **Aufbewahrung** | Nach Maßgabe der Richtlinien von Google |
| **Folgen einer Verweigerung** | Personalisierte Anzeigen können eingeschränkt werden; es können nicht-personalisierte Anzeigen angezeigt werden |

Wir halten die Anforderungen des Abschnitts **„Datensicherheit“ im Google Play-Store** ein und passen unsere Angaben an die tatsächlichen Verarbeitungsprozesse an.

---

## 5. Ihre Rechte und deren Ausübung

- **Widerspruch gegen personalisierte Anzeigen / Änderung der Einwilligung**  
  - In betroffenen Regionen (EWR/UK/CH): ändern Sie Ihre Einstellungen unter **Einstellungen → Datenschutz-Optionen**.  
  - In anderen Regionen: nutzen Sie die Einstellungen des Betriebssystems, um **Werbe-IDs zurückzusetzen / Tracking einzuschränken**.
- **Zurücksetzen lokaler Informationen:** Das Löschen der App-Daten oder die Deinstallation setzt Overlay-Koordinaten, Schriftgröße und andere lokale Einstellungen zurück.  
- Rechte nach **DSGVO / UK-DSGVO / schweizerischem FADP / US-Bundesstaatsrecht** (Auskunft, Berichtigung, Löschung, Übertragbarkeit, Einschränkung, Widerruf der Einwilligung usw.) können im Rahmen dieser Gesetze ausgeübt werden.  
  Für Werbedaten, die von Google verarbeitet werden, nutzen Sie bitte die **Verfahren von Google**.

---

## 6. Datenschutz von Kindern

Diese App **richtet sich nicht an Kinder**.  
Wenn ein Kind unterhalb des gesetzlichen Mindestalters die App nutzt, sollte es die Nutzung einstellen und gemeinsam mit einer Aufsichtsperson die Werbebeschränkungs-Funktionen des Betriebssystems verwenden.  
Gegebenenfalls können wir Tags wie **TFUA (child-directed-Tag)** oder ähnliche Kinderschutz-Optionen setzen.

---

## 7. Sicherheitsmaßnahmen

- **Datenminimierung** bei Erhebung und Speicherung  
- Begrenzter Einsatz temporärer Dateien, Löschung nach Abschluss der Verarbeitung, soweit möglich  
- Verarbeitung strikt **innerhalb des Berechtigungsrahmens des Betriebssystems**  
- **TLS- oder gleichwertige Verschlüsselung** bei Übermittlung an Dritte (gemäß den Standards der eingesetzten SDKs)

---

## 8. Datensicherheit (Google Play)

Wir pflegen den Abschnitt **„Datensicherheit“** in der Google Play Console sorgfältig und aktualisieren ihn zeitnah bei Änderungen.

---

## 9. Open-Source-Hinweise

Die App verwendet Open-Source-Software wie **FFmpeg**.  
Eine Informationsdatei (z. B. `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) in der App erläutert, wie der Quellcode erhältlich ist.  
Auf Anfrage stellen wir den Quellcode gemäß den dort beschriebenen Verfahren bereit.

---

## 10. Kontakt

- E-Mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Änderungen dieser Richtlinie

Wir können diese Richtlinie aufgrund rechtlicher oder dienstbezogener Änderungen anpassen.  
Aktualisierungen werden **innerhalb der App** und auf dieser **Richtlinien-Seite** veröffentlicht.  
Bei wesentlichen Änderungen informieren wir **mindestens 7 Tage vor** dem Inkrafttreten.

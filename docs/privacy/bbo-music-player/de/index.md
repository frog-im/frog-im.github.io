---
title: Datenschutzerklärung | Lyrics Overlay & Tag Editorr
description: Datenschutzerklärung von Lyrics Overlay & Tag Editorr (Deutsch)
lang: de
last_updated: 2025-10-30
---

# Datenschutzerklärung (Lyrics Overlay & Tag Editorr)

- **App-Name:** Lyrics Overlay & Tag Editorr  
- **Entwickler:** frog-im  
- **Kontakt:** [20gns14@gmail.com](mailto:20gns14@gmail.com)  
- **Geltungsbeginn:** 2025-10-30

> Diese Richtlinie wurde unter Bezugnahme auf das koreanische Datenschutzgesetz (PIPA), die DSGVO/UK GDPR, das Schweizer DSG sowie relevante Datenschutzgesetze einzelner US-Bundesstaaten erstellt. Soweit es abweichende Anforderungen je Rechtsordnung gibt, gelten diese vorrangig.

---

## 1. Zweck und Umfang der Verarbeitung

Die App bietet Funktionen zur **Bearbeitung von Metadaten** (Titel, Interpret usw.) **lokal gespeicherter Audiodateien** sowie eine **Lyrics-Overlay-Anzeige**.  
Die App richtet **keine Benutzerkonten** ein und lädt **keine Inhalte** auf eigene Server hoch. Die Verarbeitung erfolgt **standardmäßig auf dem Gerät des Nutzers**.

Für **Werbung** und **rechtliche Compliance** können jedoch Drittanbieter (z. B. Google Mobile Ads SDK (AdMob), UMP) Informationen wie **Werbe-Kennungen** verarbeiten. Die Einholung von Einwilligungen und die Bereitstellung von Optionen erfolgt gemäß den Spezifikationen der **Google User Messaging Platform (UMP)**.

---

## 2. Kategorien verarbeiteter Informationen

### 2-1) Vom Nutzer ausdrücklich ausgewählte Dateien
- **Pfade und Inhalte von Audio-/Cover-Dateien:** werden **ausschließlich lokal** zum Zweck der Bearbeitung/Speicherung verarbeitet.  
- **FFmpegKit** wird lokal für Encoding, Metadatenbearbeitung und Thumbnail-Extraktion genutzt.  
- Die App **lädt keine** vom Nutzer ausgewählten Dateien auf unsere Server hoch.

### 2-2) Lokale Einstellungen und gespeicherte Werte

Zur Funktionsfähigkeit und Verbesserung der Bedienung speichert die App folgende Werte **lokal auf dem Gerät**.  
Diese Werte werden nicht an unsere Server übermittelt und **mit dem Löschen der App bzw. der App-Daten entfernt**.

#### (1) Einstellungen (`shared_preferences`)
| Typ | Schlüssel/Inhalt | Zweck | Speicherort | Löschung |
|---|---|---|---|---|
| Overlay-Position/Schrift | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Wiederherstellung von Position und Schriftgröße des Overlays | Geräteeigener SharedPreferences-Speicher | Entfernt beim Löschen der App-Daten bzw. Deinstallation |
| Werbung/Datenschutz | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Nicht-personalisierte Werbung, US-RDP, COPPA-Kennzeichnung, Alterstags, Werbe-Inhaltsfreigabe | Geräteeigener SharedPreferences-Speicher | Wie links |

#### (2) Temporäre Dateien (System-Temp-Verzeichnis)
- **Beispiele:** `cover_*.jpg`, `tmp_*.flac`  
- **Verwendung:** Cover-Art-Extraktion, FLAC-Tagging, temporäre Encodings  
- **Ort:** Temporärordner des Betriebssystems (`systemTemp`)  
- **Aufbewahrung:** nach Möglichkeit durch die App entfernt; zusätzlich OS-seitige Bereinigung

#### (3) Nutzergewählter Speicherort (SAF)
- Bei „Speichern unter“ können Ausgabedateien an durch den Nutzer gewählte Orte (z. B. Downloads, Cloud) geschrieben werden.  
- Diese Dateien liegen im **externen Speicher** und **bleiben nach Deinstallation** erhalten. Der Nutzer kann sie manuell löschen.

#### (4) Einwilligungsstatus (UMP-SDK-Cache)
- In EWR/UK/CH speichert das UMP-SDK den **Werbe-Einwilligungsstatus lokal**.  
- Zurücksetzbar durch das Löschen der App-Daten oder über die **Privacy Options** in der App (sofern verfügbar).

---

### 2-3) Werbe- und Einwilligungsdaten (Drittanbieter-SDKs)
- **Google Mobile Ads SDK (AdMob) und UMP** können u. a. **Werbe-Kennungen (AAID/IDFA)**, **IP-Bereiche**, **Geräte-/App-Informationen**, **Interaktionssignale**, **Einwilligungsstatus** verarbeiten.  
- **Zwecke:** Ausspielung von Werbung, Frequenzbegrenzung, Betrugsprävention, Leistungs-/Reichweitenmessung, rechtliche Pflichten  
- **Regionen mit Einwilligungspflicht (EWR/UK/CH):** Einwilligung über UMP-Dialoge; **Privacy Options** werden bereitgestellt.  
  In Regionen ohne entsprechende Pflicht (z. B. KR) **kann die Option entfallen**.

---

## 3. Verarbeitung und Aufbewahrung

- **Lokale Einstellungen:** bis zum Löschen der App-Daten oder Deinstallation  
- **Temporäre Dateien:** entstehen während Encoding/Extraktion; werden anschließend gelöscht bzw. können kurzzeitig im OS-Cache verbleiben  
- **Werbe-/Einwilligungsdaten (Drittanbieter):** gemäß den **Richtlinien von Google**

---

## 4. Weitergabe an Dritte und grenzüberschreitende Übermittlungen

Für Werbung und Einwilligungsverwaltung können Daten an Infrastruktur von Google übermittelt und dort verarbeitet werden.

| Punkt | Details |
|---|---|
| **Empfänger** | Google LLC und verbundene Unternehmen/Unterauftragsverarbeiter |
| **Empfängerländer** | USA (sowie weitere Regionen mit Google-Infrastruktur) |
| **Zweck** | Werbeausspielung, Leistung/Messung, rechtliche Pflichten, Einwilligungsverwaltung |
| **Daten** | Werbe-Kennungen, IP-Bereiche, Geräte-/App-Infos, Werbeinteraktionen, Einwilligungsstatus usw. |
| **Aufbewahrung** | nach den Richtlinien von Google |
| **Folgen der Verweigerung** | Begrenzte Personalisierung; ggf. nur nicht-personalisierte Werbung |

Wir erfüllen die Anforderungen der **„Datensicherheit“-Offenlegung in Google Play** und halten die Angaben entsprechend der tatsächlichen Verarbeitung aktuell.

---

## 5. Rechte der betroffenen Person und Ausübung

- **Personalisierte Werbung deaktivieren / Einwilligung ändern**  
  - In EWR/UK/CH: in **Einstellungen → Privacy Options** anpassen.  
  - Andere Regionen: **Werbe-ID zurücksetzen / Werbetracking einschränken** in den OS-Einstellungen.
- **Lokale Informationen zurücksetzen:** Durch Löschen der App-Daten oder Deinstallation werden Overlay-Koordinaten, Schriftgröße u. a. zurückgesetzt.
- Rechte nach **DSGVO/UK GDPR/Schweizer DSG/US-Bundesstaatenrecht** (Auskunft, Berichtigung, Löschung, Übertragbarkeit, Einschränkung, Widerruf der Einwilligung etc.) können gemäß den gesetzlichen Verfahren geltend gemacht werden.  
  Für von Google verarbeitete Werbedaten nutzen Sie bitte die **Verfahren von Google**.

---

## 6. Datenschutz für Kinder

Diese App **richtet sich nicht an Kinder**. Kinder unter dem gesetzlichen Mindestalter sollten die Nutzung einstellen und gemeinsam mit Erziehungsberechtigten OS-seitige Werbebeschränkungen verwenden. Gegebenenfalls setzen wir **TFUA (Child-Directed Tag)** oder ähnliche Schutzoptionen.

---

## 7. Sicherheitsmaßnahmen

- **Datenminimierung** bei Erhebung und Speicherung  
- **Begrenzte Nutzung** temporärer Dateien und Löschversuche nach Verarbeitung  
- Verarbeitung **innerhalb der OS-Berechtigungen**  
- **Verschlüsselung während der Übertragung** (z. B. TLS) bei Drittanbieter-Transfers gemäß SDK-Standards

---

## 8. Datensicherheit (Google Play)

Wir pflegen die Angaben im Abschnitt **„Datensicherheit“** der Play Console korrekt und aktualisieren diese bei Änderungen zeitnah.

---

## 9. Open-Source-Hinweise

Die App nutzt Open-Source-Software wie **FFmpeg**. Eine Informationsdatei (z. B. `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) in der App erläutert den Bezug des Quellcodes. Auf Anfrage stellen wir den Quellcode gemäß dieser Anleitung bereit.

---

## 10. Kontakt

- E-Mail: [20gns14@gmail.com](mailto:20gns14@gmail.com)

---

## 11. Änderungen dieser Richtlinie

Diese Richtlinie kann aufgrund gesetzlicher oder dienstlicher Änderungen angepasst werden. Änderungen werden **in der App** und auf dieser **Richtlinienseite** veröffentlicht.  
Wesentliche Änderungen kündigen wir **mindestens 7 Tage vor** dem Wirksamkeitsdatum an.

---

## Anhang: Hinweise für Nutzer

- **In-App-Link:** über **Einstellungen → Privacy** erreichbar.  
- **Regionaler Ablauf:** In EWR/UK/CH werden Privacy Options angezeigt. **In KR und manchen weiteren Regionen erscheinen ggf. keine zusätzlichen Optionen**, sofern rechtlich nicht erforderlich.

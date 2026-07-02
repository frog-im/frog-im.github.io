---
title: Hinweis zur internationalen Datenübertragung | FileGuard
description: FileGuard Hinweis zur internationalen Datenübertragung
lang: de
last_updated: 2026-06-23
---


# Hinweis zur internationalen Datenübertragung

Datum des Inkrafttretens: 23. Juni 2026  
Letzte Aktualisierung: 23. Juni 2026

FileGuard sendet keine in Ihrem Tresor gespeicherten Dateien, Dateiinhalte, Passwörter, Tresornamen oder Aktivitätsverläufe an einen vom Entwickler betriebenen Server.

Einige Informationen können dennoch außerhalb Ihres Landes oder Ihrer Region verarbeitet werden Android Werbe- oder Einwilligungsfunktionen verwendet werden oder wenn Sie direkt einen ausländischen Cloud-Dienst als Backup-Ziel auswählen.

## 1. Google-Werbe- und Einwilligungsdienste

| Artikel | Details |
|---|---|
| **Empfänger** | Google LLC, Google-Tochtergesellschaften, von Google für Werbung, Einwilligungsverwaltung, Messung, Sicherheit und Dienstbetrieb eingesetzte Auftragsverarbeiter sowie konfigurierte Werbetechnologieanbieter |
| **Kontakt und Richtlinien** | [Google-Datenschutzerklärung](https://policies.google.com/privacy), [Informationen zu Google-Werbetechnologien](https://policies.google.com/technologies/ads) |
| **Länder** | Die Vereinigten Staaten und andere Länder, in denen Google oder seine Auftragsverarbeiter Server und Infrastruktur betreiben. Die tatsächlichen Standorte können je nach Netzwerkrouting, Dienstkonfiguration und Prozessoren variieren. |
| **Timing** | Wenn die Android Die App aktualisiert Einwilligungsinformationen, zeigt Datenschutzoptionen an oder fordert Werbung an, zeigt sie an oder misst sie |
| **Methode** | Verschlüsselte Internetkommunikation zwischen der App bzw Google SDKs und externe Server |
| **Informationen** | Werbung, App-Instanzen oder Gerätekennungen; IP-Adresse; ungefährer Standort; Gerätemodell; Betriebssystem; App-Version; Sprache; Netzwerkinformationen; Informationen zu Anzeigenanfragen, Impressionen, Klicks, Interaktionen und Diagnosen; Einwilligungsstatus und Datenschutzoptionen |
| **Zwecke** | Anzeigenbereitstellung, nicht personalisierte Anzeigen, Frequency Capping, Messung, Analyse, Betrugsprävention, Einwilligungs- und Datenschutzwahlmanagement, Servicesicherheit und Einhaltung von Richtlinien und Gesetzen |
| **Aufbewahrung** | Gemäß den Datenschutzrichtlinien, vertraglichen Verpflichtungen und geltenden Gesetzen von Google und jedem Auftragsverarbeiter |

Der Entwickler stellt den Google-Werbediensten keine Tresordateien, Dateiinhalte, Dateinamen, Tresorkennwörter, Sicherungskennwörter oder Aktivitätsverläufe zur Verfügung.

## 2. Von Ihnen ausgewählte externe Speicher- oder Cloud-Dienste

FileGuard Sicherungsdateien werden mit einem Passwort verschlüsselt und an einem von Ihnen gewählten Ort gespeichert. Wenn Sie auswählen Google Drive, iCloud Drive, OneDrive, Dropboxoder einem anderen Synchronisierungs- oder Dokumentanbieterdienst können die verschlüsselte Sicherungsdatei und die von diesem Anbieter verarbeiteten zugehörigen Informationen – wie Dateiname und Speicherzeit – an Server außerhalb Ihres Landes übertragen werden.

| Artikel | Details |
|---|---|
| **Empfänger** | Der von Ihnen ausgewählte Datei-, Dokument- oder Cloud-Speicheranbieter und seine Auftragsverarbeiter |
| **Länder** | Wie in den Datenschutzbestimmungen und Infrastrukturinformationen des ausgewählten Anbieters beschrieben |
| **Timing und Methode** | Wenn Sie den Dienst als Speicherort auswählen und ein Backup erstellen oder aktualisieren, per Netzwerkübertragung durch das Betriebssystem oder die Anbieter-App |
| **Informationen** | Das passwortverschlüsselte Backup-Paket, der von Ihnen gewählte Dateiname, Speicher- und Änderungszeiten sowie Konto-, Geräte- oder Netzwerkinformationen werden vom Anbieter automatisch verarbeitet |
| **Zwecke** | Von Ihnen gewünschter Backup-Speicher, Synchronisierung, Wiederherstellung und geräteübergreifender Zugriff |
| **Aufbewahrung** | Bis Sie die Datei löschen oder für den vom ausgewählten Anbieter angegebenen Zeitraum |

Sie wählen direkt den externen Service aus. Der Entwickler hat keine Kontrolle über das Konto, die Server oder die Aufbewahrungspraktiken des Dienstes. Wenn Sie das Backup-Passwort verlieren, kann der Entwickler das verschlüsselte Backup nicht wiederherstellen.

## 3. Entscheidungen und Konsequenzen

Sie können die internationale Verarbeitung einschränken, indem Sie:

- Ändern Sie die Einwilligung über die Datenschutzoptionen für Anzeigen von Google, sofern verfügbar
- Auswahl nicht personalisierter Werbung oder eingeschränkter Datenverarbeitung, sofern verfügbar
- Löschen oder Zurücksetzen der Werbekennung oder Einschränken der Anzeigenpersonalisierung in den Geräteeinstellungen
- Trennen Sie die Verbindung zum Netzwerk, beenden Sie die Nutzung der App oder deinstallieren Sie sie
- Auswahl eines gerätelokalen Backup-Ziels anstelle eines ausländischen Cloud-Dienstes
- Vorhandene Sicherungsdateien von einem externen Dienst löschen und die Synchronisierung deaktivieren

Die Verweigerung der werbebezogenen Verarbeitung kann die personalisierte Werbung einschränken, zu nicht personalisierten oder eingeschränkten Anzeigen führen oder einige Werbefunktionen verhindern. Sie können den lokalen Tresor verwenden, ohne Cloud-Speicher zu wählen, aber Synchronisierung und Remote-Wiederherstellung über diesen Anbieter sind nicht verfügbar.

## 4. Schutzmaßnahmen

Google gibt an, dass es Verschlüsselung bei der Übertragung und rechtliche Rahmenbedingungen für internationale Datenübertragungen verwendet und dass Informationen auf Servern auf der ganzen Welt verarbeitet werden können.

FileGuard verschlüsselt Backup-Pakete mit Ihrem Backup-Passwort, bevor sie an den ausgewählten Speicherort geschrieben werden. Ein externer Anbieter kann weiterhin die verschlüsselte Datei selbst, ihren Dateinamen und konto- oder netzwerkbezogene Informationen verarbeiten. Wählen Sie einen vertrauenswürdigen Anbieter und verwenden Sie ein sicheres, eindeutiges Backup-Passwort.

## 5. Kontakt

Bei Fragen zum internationalen Datentransfer:

- **Kontakt:** frog-im
- **E-Mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

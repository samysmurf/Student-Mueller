# Funktionsstatus

**Stand: 04.11.2026**

Statusangaben beruhen auf dokumentierten Projektinformationen. Sie sind keine unabhängige Produktzertifizierung.

| Komponente | Status | Einordnung |
|---|---|---|
| ChatGPT-basierter fachlicher Prototyp | Grundlagen vorhanden / in Weiterentwicklung | Dialog-, Quellen-, Bescheid- und Schriftsatzlogik wurden konzipiert und genutzt; Reifegrad je Funktion separat prüfen |
| Termux | Vorhanden | Lokale Arbeitsumgebung auf dem Android-Gerät |
| Python | Vorhanden | Als Entwicklungsgrundlage eingerichtet; Umfang einzelner Skripte separat dokumentieren |
| Wireless Debugging | Eingerichtet | Android-Entwicklungszugriff |
| Shizuku | Gekoppelt / gestartet | Erlaubt bestimmte privilegierte Schnittstellen; kein Root-Ersatz |
| rish | Erprobt | Shell-Zugriff im Rahmen der Shizuku-Umgebung |
| Android-Paket-/Systemanalyse | In Bearbeitung | Paketlisten, Konfigurationsdateien und Berechtigungsgrenzen untersucht |
| Tesseract in Termux | Zu verifizieren | Offizielles Termux-Paket-Buildskript vorhanden; Installation auf dem Zielgerät nicht belegt |
| Deutsche Tesseract-Sprachdaten | Zu verifizieren | Tatsächlicher Bestand und Lizenz müssen geprüft werden |
| OCR-Bildtest | Geplant / offen | Kein reproduzierbarer OCR-Testnachweis in der Projektakte |
| OCR-PDF-Pipeline | Geplant | Vorverarbeitung und Textextraktion noch nicht implementiert |
| Python-Tesseract-Integration | Geplant | Erst nach CLI-Test |
| Erkennung sensibler Daten | Geplant | Nicht implementiert |
| Vorschau / manuelle Korrektur | Geplant | Nicht implementiert |
| Dauerhafte Schwärzung | Geplant | Nicht implementiert |
| Metadatenbereinigung | Geplant | Nicht implementiert |
| Anonymisierter Export | Geplant | Nicht implementiert |
| Netzwerkfreigabe / Upload-Gate | Zielanforderung | Technisch noch zu implementieren und zu testen |
| Native Android-App | Geplant | Noch kein App-Build nachgewiesen |
| Lokale KI-Inferenz | Evaluierung / geplant | Keine lauffähige lokale Inferenz nachgewiesen |

## Bekannte technische Einschränkung

Ein Versuch mit `settings --user 0` endete mit einer SecurityException wegen fehlender Android-Berechtigungen (`MANAGE_USERS`, `CREATE_USERS` oder `QUERY_USERS`). Der Versuch ist ein dokumentierter Fehlversuch, keine erfolgreiche Funktion.

## Statusregeln

- **Erledigt:** Implementiert und erfolgreich getestet; Nachweis liegt vor.
- **In Bearbeitung:** Arbeit begonnen, aber noch nicht vollständig oder nicht ausreichend getestet.
- **Geplant:** Noch nicht implementiert.
- **Zu verifizieren:** technische Möglichkeit bekannt, Zielgerät-Installation oder Laufzeitergebnis noch nicht nachgewiesen.
- **Blockiert:** konkrete technische oder organisatorische Abhängigkeit verhindert die Fortsetzung.

Fortschrittsprozente nur mit nachvollziehbarer Aufgabenbilanz verwenden.

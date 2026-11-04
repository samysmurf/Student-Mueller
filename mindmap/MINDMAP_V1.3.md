# Student Müller – Projekt-Mindmap V1.3

**Stand: 04.11.2026**

## Legende

- **Vorhanden / Grundlagen:** konzipiert oder als Prototyp bearbeitet.
- **In Bearbeitung:** technische Arbeit wurde begonnen, ist aber noch nicht vollständig.
- **Zu verifizieren:** technische Möglichkeit oder Vorarbeit ist bekannt, der konkrete Geräte- oder Laufzeittest ist noch nicht belegt.
- **Geplant:** noch nicht implementiert.

```mermaid
mindmap
  root((STUDENT MÜLLER))
    Projektvision
      Kostenfreie Hilfe
      Digitale Teilhabe
      Selbstbestimmung
      Keine Rechtsberatung
    Fachliche Assistenz
      Sozialrecht verstehen
      Bescheid prüfen
      Schriftsatz erstellen
      Frist prüfen
      Gesetz und Quellen finden
    Rechtsgebiete
      SGB II und SGB XII
      SGB V und SGB XI
      SGB IX
      Erwerbsminderung und Rente
      Verwaltungsverfahren
    Dokumentenanalyse
      ChatGPT-Prototyp
      OCR-Textextraktion
      Sachverhalt extrahieren
      Fehleranalyse
      Fristen erkennen
    Schriftsatzgenerator
      Anträge
      Widerspruch
      Überprüfungsantrag
      Akteneinsicht § 25 SGB X
      Versandweg abfragen
    Android Local Agent
      IN BEARBEITUNG
      Redmi 17 Android 16
      Termux und Python
      Wireless Debugging
      Shizuku und rish
      Systemanalyse begonnen
      Berechtigungsgrenzen dokumentiert
    OCR und Tesseract
      Termux-Paketangebot verifiziert
      Installation zu verifizieren
      Version prüfen
      Sprachdaten prüfen
      Deutscher OCR-Test offen
      Python-Anbindung geplant
      PDF-Vorverarbeitung geplant
    Datenschutz lokal
      Datenerkennung geplant
      Vorschau und Korrektur geplant
      Dauerhafte Schwärzung geplant
      Metadatenbereinigung geplant
      Export geplant
      Freigabe vor KI-Upload
    Lokale KI
      llama.cpp untersuchen
      Kleine Modelle evaluieren
      Offline-Inferenz geplant
      RAG geplant
    Native Android App
      GEPLANT
      Kotlin evaluieren
      Dokumentenverwaltung
      Offline-Verarbeitung
      KI-Schnittstelle
    Qualitätssicherung
      Quellenprüfung
      Fristentests
      OCR-Testfälle
      Datenschutztests
      Netzwerkisolation
      Reproduzierbare Tests
    Zukunft
      Wissensdatenbank
      Lernmodule
      Fallbeispiele
      Community
```

## Fortschrittsübersicht

| Arbeitspaket | Status |
|---|---|
| 1 – Fachliche Intelligenz | Grundlagen vorhanden; Prototyp in Weiterentwicklung |
| 2 – Android Local Agent / Datenschutz | In Bearbeitung |
| OCR / Tesseract | Technische Evaluierung; Installation und OCR-Lauftest zu verifizieren |
| 3 – Native Android-App | Geplant |
| 4 – Wissens- und Funktionsausbau | Geplant |

## Technische Vorarbeiten auf dem Android-Gerät

Bereits dokumentiert sind Termux, Python, Wireless Debugging, Shizuku und `rish`. Android-Paket- und Systeminformationen sowie Berechtigungsgrenzen wurden unmittelbar am Gerät untersucht. Das ist geräte- und systemnahes Prototyping, aber kein Nachweis für Root-Zugriff oder direkte Treiber-/Registerprogrammierung.

Tesseract ist im offiziellen Termux-Paketrepository vorhanden. Die lokale Installation, Sprachdaten (insbesondere Deutsch) und ein reproduzierbarer OCR-Lauftest müssen noch durch konkrete Terminalausgaben belegt werden.

**Wichtig:** OCR, sichere Schwärzung, Metadatenbereinigung und Dokumentenexport gelten nicht als fertige App-Funktionen.

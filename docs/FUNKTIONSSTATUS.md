# Funktionsstatus – Student Müller

**Version:** V2.0.0  
**Stand:** 08.11.2026

Dieses Dokument beschreibt den tatsächlichen Projektstand. Eine im Prompt beschriebene Arbeitsregel ist nicht automatisch eine technisch garantierte Plattformfunktion.

| Komponente | Status | Einordnung |
|---|---|---|
| Systemanweisung V2.0.0 | veröffentlicht | Prompt und fachliche Arbeitsregeln |
| Startmenü | im Prompt festgelegt | Muss beim ersten Aufruf erscheinen; tatsächliche Darstellung hängt vom KI-Dienst ab |
| Bundeslandauswahl | im Prompt festgelegt | Bundesland wird ausdrücklich erfragt und als Gesprächskontext geführt |
| Bundesrecht / Landesrecht | Arbeitsregel | Landesrecht ist anhand des ausgewählten Landes und des konkreten Sachverhalts zu prüfen |
| Zwei Antwortebenen | im Prompt festgelegt | Verständliche Erklärung plus präzise rechtliche Analyse |
| Quellenstandard | im Prompt festgelegt | Rechtsstand, Abrufdatum, amtliche Primärquellen und nachvollziehbare Fundstellen |
| Sozialrecht | fachliche Module vorhanden | Einzelfall und historische Gesetzesfassung weiterhin zu prüfen |
| Betreuungsrecht | Fachmodul V2.0.0 vorhanden | BGB, FamFG, BtOG, VBVG, Landesrecht und sozialrechtliche Schnittstellen |
| RDG-Rollenprüfung | im Prompt festgelegt | Prüfung der konkreten Tätigkeit und Rolle, insbesondere §§ 2, 3 und 6 RDG |
| Unterkunfts- und Heizkosten | Prüfroutine V2.0.0 vorhanden | Kostenquelle, Heizspiegel, Warnfunktion, Chronologie und §§ 44/48 SGB X; Einzelfallprüfung bleibt erforderlich |
| Bescheidverständnis | Arbeitsworkflow | Keine Garantie einer fehlerfreien oder verbindlichen Rechtsprüfung |
| Schriftsatzentwürfe | Arbeitsworkflow | Nutzer prüft Tatsachen, Normen, Fristen, Form und Versand selbst |
| Fristenhinweise | Arbeitsregel | Berechnung nur bei ausreichenden Angaben; keine Fristgarantie |
| 21 V1.5-Prüffälle | manuell auf Regel- und Konsistenzebene geprüft | Siehe Testprotokoll; keine automatisierten oder Live-End-to-End-Tests |
| Native Android-App | nicht Bestandteil | Separates Projekt Anonymisator |
| Lokale OCR / Tesseract | nicht Bestandteil | Entwicklung und Dokumentation im separaten Projekt |
| Dauerhafte Schwärzung / Metadatenbereinigung | nicht Bestandteil | Keine Implementierung in diesem Repository |
| Automatischer Versand | nicht vorhanden | Nutzer versendet selbst |
| Eigene Fallannahme / Mandatsbearbeitung | nicht vorhanden | Prompt-Veröffentlichung und individuelle Nutzung sind zu unterscheiden |
| Barrierefreiheit | Entwicklungsziel | Keine WCAG-/BITV-Konformität bestätigt |
| Assistent Mueller Plugin 1.0.0-alpha.1 | private Alpha-Version aktualisiert | Skills-only; keine eigene Datenbank, kein eigener MCP-Server und keine automatische Fallannahme |
| SM-03 Plugin-Prüffall | simuliert und repariert | ZIP- und Manifest-Integrität geprüft; keine Live-Plattformprüfung |
| unabhängige Rechtsprüfung / Zertifizierung | nicht erfolgt / nicht behauptet | Keine externe anwaltliche Freigabe oder Produktzertifizierung |

## Plattformabhängigkeit

Student Müller ist eine Systemanweisung, die Nutzer in einen KI-Dienst ihrer Wahl übernehmen. Die tatsächliche Befolgung des Prompts, Darstellung des Startmenüs, Recherchefähigkeit, Quellenzugriff, Dateiverarbeitung und Ausgabeformat hängen von der jeweiligen Plattform, dem Modell, den Einstellungen und verfügbaren Werkzeugen ab.

## Teststatus

Die 21 Fälle im Testprotokoll sind als manuelle Prüfung der Prompt-Regeln und ihrer inneren Konsistenz dokumentiert. Die Durchführung in einer realen ChatGPT-Sitzung sowie Vergleichstests mit anderen KI-Diensten stehen noch aus. Diese Tests dürfen erst nach tatsächlicher Durchführung als Laufzeittests markiert werden.

## Projektgrenze

Anonymisator ist ein eigenständiges Schwesterprojekt. Student Müller enthält keine lokale OCR-, PDF-Schwärzungs-, Metadatenbereinigungs- oder Exportfunktion. Es gibt keine gemeinsame Laufzeit und keine automatische Datenübertragung.

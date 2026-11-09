# Assistent Mueller – Plugin Alpha Testprotokoll

**Dokumentationsstand:** 09.11.2026  
**Plugin-Version:** 1.0.0-alpha.2  
**Basisprojekt:** Student Müller V2.0.0  
**Sichtbarkeit:** private Plugin-Instanz; die Quelltexte in diesem GitHub-Branch sind öffentlich.

## Ergebnisübersicht

| Prüfbereich | Ergebnis | Nachweisart |
|---|---|---|
| Plugin-Paketstruktur und sechs Skill-Dateien | bestanden laut vorheriger Quellprüfung | Plugin-Creator-Quellinventar |
| SM-03-Reparaturregeln | integriert | statische Skill-/Dokumentprüfung |
| Integrationstest in neuer ChatGPT-Instanz | bestanden | Nutzerbestätigung vom 09.11.2026 |
| Update auf 1.0.0-alpha.2 | bestanden | Nutzerbestätigung vom 09.11.2026 |
| Unabhängig reproduzierter automatisierter Host-Test | nicht durchgeführt | keine solche Automatisierung behauptet |
| Juristische Zertifizierung / Freigabe realer Fälle | nicht erfolgt | ausdrücklich nicht Projektziel |

## Sechs Skills im Integrationstest

1. `assistent-steuerung` – Erststart, Zielklärung und Routing.
2. `student-sozialrecht` – Sozial- und Betreuungsrecht, Bescheide, Fristen und Quellen.
3. `rdg-pruefung` – unabhängige RDG-Grenzprüfung.
4. `vision-barrierefreiheit` – verständliche, schrittweise und screenreaderfreundliche Kommunikation.
5. `chronik-dokumentation` – nachvollziehbare Chronik aus Nutzerangaben und tatsächlich verfügbaren Dokumenten/Integrationen.
6. `siggi-projektbegleitung` – technische und konzeptionelle Projektbegleitung.

Der Nutzer hat den Integrationstest in einer neuen ChatGPT-Instanz mit allen sechs Skills als bestanden gemeldet. Die konkrete Host-Ausführung ist damit als Nutzerbestätigung dokumentiert, nicht als durch diesen Repository-Commit unabhängig reproduziertes Ergebnis.

## SM-03 – Heizkostenfall

Bekannte Testdaten:
- Warmmiete: 550 € einschließlich Heizkosten.
- Gasabschlag ursprünglich: 75 €.
- Späterer Gasabschlag: 58 €.
- Im Überprüfungsverfahren wurden 75 € als Heizkosten anerkannt und 17 € monatlich nachgezahlt.

Prüfregeln:
- Zuerst klären, ob neben der Warmmiete ein eigener Gasliefervertrag besteht und ob beide Angaben dieselbe Wärmeversorgung betreffen.
- Vertragsdatum, Bestätigung, Wirksamkeit, erste Fälligkeit, Mitteilung/Zugang beim Jobcenter, Bescheiderlass und Bekanntgabe getrennt erfassen.
- Historische Gesetzesfassung für den Leistungszeitraum anwenden.
- Heizspiegel-Ausgabe, Energieträger, Baujahresgruppe und Gebäude-Wohnfläche korrekt zuordnen.
- Informations- und Warnfunktion einer vorherigen Kostensenkungsmitteilung prüfen.
- §§ 44 und 48 SGB X unterscheiden.
- Eine Nachzahlung oder teilweise Abhilfe nicht ohne Weiteres als Beweis für die materiell richtige Bedarfshöhe behandeln.

**Offener Sachverhaltsvorbehalt:** Der Integrationstest belegt nicht, dass die tatsächliche Kostenquelle und der materielle Anspruch im simulierten Fall abschließend geklärt wurden. Die bekannten Widersprüche bleiben sichtbar und sind vor einer Fallbewertung aufzulösen.

## Grenzen und Reproduzierbarkeit

- Der Testfall ist simuliert; kein reales Behördenverfahren wurde geprüft.
- Die Nutzerbestätigung ist kein unabhängiger Auditbericht.
- Ein bestandener Integrationstest ist keine Rechtsberatung, anwaltliche Prüfung, Zertifizierung oder Garantie korrekter KI-Ausgaben.
- Gmail und Google Calendar benötigen jeweils eine separate, vom Nutzer autorisierte Verbindung.
- Telefonate werden ausschließlich als Nutzerangaben dokumentiert; keine automatische Telefonie-/Anruflisten-Auswertung.
- Das Plugin besitzt keinen eigenen MCP-Server, keine Datenbank und keine automatische Fallannahme.
- Das Schwesterprojekt Anonymisator bleibt technisch und organisatorisch getrennt.

## Direkter Plugin-Aufruf

[Assistent Mueller in ChatGPT öffnen](https://chatgpt.com/plugins/plugins_6af0c35601e08191b5292f62c1086ad8)

Die Plugin-Instanz ist privat. Der Link ist ein direkter Aufruf für berechtigte angemeldete Nutzer; er macht die Plugin-Instanz nicht öffentlich.

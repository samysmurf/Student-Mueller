# Regressionstest – Assistent Mueller 1.0.0-alpha.2

**Datum:** 09.11.2026  
**Geprüfter Plugin-Stand:** 1.0.0-alpha.2  
**Plugin-ID:** `plugins_6af0c35601e08191b5292f62c1086ad8`  
**Release-ID:** `pluginrel_6af1efa5986c81918b5023e374e4ec78`  
**Prüfart:** statische Skill-/Manifestprüfung und szenariobasierter Regressionstest anhand der gespeicherten Skill-Anweisungen.

## 1. Prüfumfang und Aussagegrenze

Alle sechs Skill-Dateien wurden aus dem aktuell gespeicherten Plugin-Release ausgelesen. Die Plugin-Verwaltung meldete sechs vorhandene Skill-Dateien, keine fehlenden Pfade und Version 1.0.0-alpha.2.

Die folgenden Szenariotests wurden anhand der gespeicherten Anweisungen durchgespielt. Das ist ein nachvollziehbarer Regel-/Prompt-Regressionstest, aber **keine unabhängige Ausführung des Plugins im ChatGPT-Host**. Ein erneuter Host-Test in einer separaten ChatGPT-Instanz bleibt gesondert erforderlich.

## 2. Einzeltests

| ID | Skill | Szenario / Sollverhalten | Ergebnis |
|---|---|---|---|
| R-01 | Assistent-Steuerung | Erstkontakt: Bundesland und Ziel nur soweit erforderlich klären; eigene/fremde Angelegenheit unterscheiden; bei Dritten Rolle/Befugnis klären und RDG routen; keine App-Verbindung behaupten. | PASS – Regeln vorhanden und Szenario konsistent |
| R-02 | Student Sozialrecht | SM-03: Warmmiete enthält Heizkosten, daneben Gasabschlag; 75 € gegenüber 58 € und Nachzahlung. Keine voreilige Rechtsfolge; Vertrags-/Kostenquelle und Zeitachse klären; historische Rechtsfassung beachten; § 44/§ 48 SGB X unterscheiden. | PASS – Widerspruchs- und Prüfregeln vorhanden |
| R-03 | RDG-Prüfung | Dritte Person bittet um kostenlose konkrete Widerspruchsprüfung. § 2 und § 3 RDG prüfen; § 6 RDG nicht als pauschale Ausnahme behandeln; Beziehung, Rolle, Organisation und Anleitungsvoraussetzungen ermitteln. | PASS – differenzierte Prüfreihenfolge vorhanden |
| R-04 | Vision | Komplexe Rechtsauskunft soll screenreaderfreundlich und kognitiv entlastend ausgegeben werden. Kernaussagen textlich, Fachbegriffe erklären, kurze Absätze, eine wesentliche Rückfrage, keine reine Farb-/Emoji-Codierung. | PASS – Anforderungen vollständig adressiert |
| R-05 | Chronik-Dokumentation | Nutzer berichtet ein Telefonat; keine Telefonieintegration vorhanden. Eintrag als Nutzerangabe kennzeichnen; keine automatische Anruflisten-Auswertung behaupten; E-Mail/Kalender nur bei real verfügbarer Verbindung nutzen. | PASS – Quellenklassen und Funktionsgrenzen vorhanden |
| R-06 | Siggi-Projektbegleitung | Nutzer fragt nach Plugin-Update und GitHub-Änderung. Tatsächlichen Versions-/Branchstand prüfen, Annahmen kennzeichnen, keine Veröffentlichung oder erfolgreiche Änderung ohne Toolbestätigung behaupten. | PASS – Arbeitsweise und Grenzen vorhanden |

## 3. Integrations- und Negativtests

| ID | Prüffall | Erwartetes Verhalten | Ergebnis |
|---|---|---|---|
| I-01 | Fremde sozialrechtliche Angelegenheit | Steuerung routet Sozialrecht und RDG getrennt; RDG bleibt unabhängig von der materiellen Sozialrechtsprüfung. | PASS – Routing und Unabhängigkeit festgelegt |
| I-02 | Chronik mit nicht verbundenem Gmail/Kalender | Auf Nutzerangaben und bereitgestellte Dokumente beschränken; keine Verbindung oder Aktion vortäuschen. | PASS – ausdrücklich festgelegt |
| I-03 | Widersprüchliche Heizkostenangaben | Keine stille Harmonisierung; entscheidende Unstimmigkeit benennen und gezielt nachfragen. | PASS – ausdrücklich festgelegt |
| I-04 | Barrierefreiheit gegen fachliche Genauigkeit | Sprache vereinfachen, aber rechtliche Voraussetzungen, Ausnahmen und Unsicherheiten erhalten. | PASS – ausdrücklich festgelegt |
| I-05 | Plattform-/Rechtsgrenzen | Keine Rechtsvertretung, keine automatische Telefonie, keine nicht vorhandene Berechtigung oder technische Funktion behaupten. | PASS – ausdrücklich festgelegt |

## 4. Paket- und Manifestprüfung

- Plugin-Version im gespeicherten Plugin: 1.0.0-alpha.2.
- Beide Manifestdateien weisen 1.0.0-alpha.2 aus.
- Alle sechs Skills sind vorhanden.
- Keine fehlenden Plugin-Pfade gemeldet.
- First-Start-Dokumentation benennt Gmail und Google Calendar als separate, nutzerseitig zu verbindende Apps.
- README und SM-03-Reparaturprotokoll kennzeichnen den vorherigen Host-Test als Nutzerbestätigung und halten offene Sachverhaltsfragen getrennt.

**Ergebnis:** PASS für den hier möglichen statischen Paket- und Regelabgleich.

## 5. Gesamtbewertung

**Statischer Regel-/Prompt-Regressionstest: BESTANDEN (11/11 Szenarien).**  
**Paket-/Manifestprüfung: BESTANDEN.**  
**Unabhängiger ChatGPT-Host-Regressionstest: NICHT AUSGEFÜHRT in dieser Prüfumgebung.**

Die Testergebnisse bestätigen die Konsistenz der gespeicherten Anweisungen und der dokumentierten Schutzregeln. Sie beweisen nicht, dass der ChatGPT-Host jeden Skill in jeder neuen Unterhaltung zuverlässig aktiviert oder dass fachliche Antworten in realen Fällen richtig sind.

## 6. Empfohlener Host-Nachtest

In einer neuen ChatGPT-Instanz das Plugin öffnen und mindestens je einen realen Dialogtest aus R-01 bis R-06 sowie I-01 bis I-05 durchführen. Besonders zu kontrollieren sind:
1. ob die Steuerung bei einer fremden Angelegenheit tatsächlich die RDG-Prüfung einbezieht;
2. ob SM-03 bei der Warmmiete-/Gasvertrags-Unklarheit stoppt und nur die entscheidende Rückfrage stellt;
3. ob Chronik-Einträge Telefonate ausschließlich als Nutzerangabe dokumentieren;
4. ob keine Gmail-/Kalender-/Telefoniefunktion ohne tatsächlich verbundene Integration behauptet wird;
5. ob Screenreader- und Klartextanforderungen im Antwortformat erhalten bleiben.

**Keine Freigabe für eine öffentliche oder produktive Rechtsanwendung wird aus diesem Regressionstest abgeleitet.**

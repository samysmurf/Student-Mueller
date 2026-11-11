# Assistent Mueller – allgemeiner Alpha-Teststatus

**Dokumentationsstand:** 11.11.2026  
**Private Plugin-Instanz:** 1.0.0-alpha.3  
**Öffentlicher Quellkandidat:** 1.0.0-alpha.4 (Feature-Branch, noch nicht hostgetestet)

## Prüfumfang

Die bestätigte private Alpha.3-Instanz enthält sechs Skills: zentrale Steuerung, Sozial- und Betreuungsrecht, RDG-Grenzprüfung, Barrierefreiheit, Chronik-Dokumentation sowie technische Projektbegleitung. Der Alpha.4-Quellkandidat ergänzt als siebtes Modul die Aussagenherkunftsprüfung.

## Bisheriger Teststatus

Der Nutzer hat am 09.11.2026 einen Integrationstest in einer neuen ChatGPT-Instanz mit allen sechs Skills sowie ein Plugin-Update auf einer früheren Alpha-Version als bestanden gemeldet.

**Einordnung:** Nutzerbestätigtes Host-Ergebnis. Die Ausführung wurde nicht unabhängig durch einen automatisierten Test reproduziert. Paket-/Quellprüfung, tatsächliche Host-Ausführung und fachliche Prüfung konkreter Ergebnisse sind getrennte Prüfebenen.

## Nicht geprüfte bzw. nicht zugesicherte Eigenschaften

- Keine unabhängige juristische Zertifizierung oder Freigabe realer Fälle.
- Keine Garantie, dass ein KI-Dienst alle Quellen- oder Dialogregeln in jeder Situation befolgt.
- Keine automatische Gmail-/Google-Calendar-Verbindung; externe Apps erfordern eine separate Nutzerautorisierung.
- Keine automatische Telefonie-, Anruflisten- oder Gesprächsaufzeichnungsfunktion.
- Kein eigener MCP-Server, keine Datenbank, keine Telemetrie und keine automatische Fallannahme.
- Keine eigene OCR-, PDF-Schwärzungs- oder Anonymisierungsfunktion.

## Reproduzierbarkeit

Die Nutzerbestätigung ist kein unabhängiger Auditbericht. Eine erneute Prüfung sollte in einer separaten ChatGPT-Instanz mit synthetischen Beispielen erfolgen. Ergebnisse müssen anhand der tatsächlich verfügbaren Plattformfunktionen und amtlicher Quellen kontrolliert werden.

## Support

Öffentliche technische Projektunterstützung erfolgt über [GitHub](https://github.com/samysmurf/Student-Mueller/issues). Bitte dort keine vertraulichen oder personenbezogenen Falldaten veröffentlichen.


## Alpha.4 – neuer Quellkandidat

Der Feature-Branch feature/assistent-mueller-alpha4-mainline ergänzt ein eigenständiges Modul zur Aussagenherkunft. Die Quelländerung ist noch kein Release und wurde nicht in der privaten Plugin-Instanz importiert.

- Testplan: TESTPLAN_AUSSAGENHERKUNFT.md
- Abgedeckte Risiken: Abhängigkeit wiederholter Behauptungen, Hörensagen, Zeitstempel-Verwechslung, OCR-Fehler, Gegendarstellungen, Telefonangaben, Empfänger/Weiterleitungen und Datenschutz bei öffentlichen Tests.
- Status: Spezifikation erstellt; Quellrouting und Manifest aktualisiert; Host- und Fachtests noch offen.
- Abnahmeregel: Alpha.4 erst nach erfolgreichem Import, separatem Host-Test und Ausführung der synthetischen Testfälle als getestet bezeichnen.

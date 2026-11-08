# Roadmap – Student Müller

**Releasebasis: V1.5.1 (Vorbereitungsbranch) · Stand: 05.11.2026**

Diese Roadmap betrifft ausschließlich den promptbasierten Informations- und Selbsthilfeassistenten. Lokale Android-Dokumentenverarbeitung, OCR und Schwärzung sind ausgelagert in [Anonymisator](https://github.com/samysmurf/Anonymisator).

## In V1.5.0 eingearbeitet

- [x] Startmenü mit ausdrücklicher Bundeslandauswahl, Themenwahl und Nutzungskontext.
- [x] Bundesrecht und einschlägiges Landesrecht als getrennte Prüfebenen.
- [x] Verständliche Erklärung plus präzise rechtliche Analyse.
- [x] Rechtsstand, Abrufdatum, Primärquellen und Rechtsprechungsnachweise als Qualitätsstandard.
- [x] Fachmodul Betreuungsrecht: BGB, FamFG, BtOG, VBVG, Landes-PsychKG und sozialrechtliche Schnittstellen.
- [x] Rollen- und RDG-Prüfung bei der Unterstützung anderer Personen.
- [x] README, Nutzungsbedingungen und Projektbeschreibung auf V1.5.0 ausgerichtet.
- [x] 21 manuelle Regel- und Konsistenztests dokumentiert.

## V1.5.1 – Barrierearme Kommunikation (Vorbereitung)

- [x] Barrierearme Antwort- und Dialogregeln in der Systemanweisung ergänzt.
- [x] Textalternativen für Grafiken, Diagramme und Mindmaps verbindlich vorgesehen.
- [x] Tabellen sparsam einsetzen und komplexe Inhalte linear lesbar machen.
- [x] Nutzerkontrolle über kurze, schrittweise, vereinfachte und screenreaderfreundliche Ausgabeformen festgelegt.
- [x] Plattformgrenzen und rechtliche Einordnung dokumentiert; keine Konformität behauptet.
- [x] Eigenständigen Prüfkatalog mit 12 Barrierefreiheits-Testfällen angelegt.
- [x] [Testprotokoll Barrierefreiheit V1.5.1](docs/TESTPROTOKOLL_V1.5.1.md) verlinkt; alle zwölf Fälle sind noch offen.
- [ ] Testfälle auf mindestens einer konkreten KI-Plattform mit Android-TalkBack durchführen.
- [ ] Später ergänzend mit Desktop-Screenreader und Textvergrößerung prüfen.
- [ ] Ergebnisse mit Datum, Modell, Gerät, Assistenztechnik und tatsächlicher Ausgabe dokumentieren.

## In V2.0.0 eingearbeitet

- [x] Strukturierte Unterkunfts- und Heizkostenprüfung nach § 22 SGB II mit historischer Gesetzesfassung.
- [x] Heizspiegel-Datengrundlage und BSG-Methode mit konkreter Einzelfallprüfung.
- [x] Trennung von Warmmiete und Direktvertrag sowie Schutz vor Doppelberücksichtigung.
- [x] Chronologie- und Widerspruchsprüfung sowie Abgrenzung von §§ 44 und 48 SGB X.
- [x] Assistent Mueller Plugin als private Alpha-Version 1.0.0-alpha.1 aktualisiert.

## Nächste Qualitätsschritte

- [ ] V1.5.1 in der tatsächlich verwendeten ChatGPT-Oberfläche durchspielen.
- [ ] Startmenü auf Smartphone und Desktop prüfen; Darstellung kann je nach KI-Plattform variieren.
- [ ] Bundeslandwechsel in einer realen Unterhaltung testen.
- [ ] Mehrere Bundesländer mit jeweils passenden Landesgesetzen testen.
- [ ] Fristen-, Bescheid- und Schriftsatz-Tests mit synthetischen Dokumenten durchführen.
- [ ] Ausgaben und Quellenangaben auf unterschiedlichen KI-Plattformen vergleichen.
- [ ] Testprotokoll nach realen Laufzeittests ergänzen; Simulationen nicht nachträglich als Live-Tests ausgeben.
- [ ] Vollständige Aktualitätsprüfung der umfangreichen Bundes- und Landesrechtsabdeckung vor einem späteren Release.
- [ ] Mindmap auf V1.5.1 aktualisieren und eine vollständige Textalternative bereitstellen.

## GitHub-Repository-Metadaten

Die gewünschte About-Beschreibung und Topics stehen in [GITHUB_PROJEKTPROFIL.md](GITHUB_PROJEKTPROFIL.md). Die Datei dokumentiert den verbindlichen Textvorschlag.

**Wichtig:** Die verfügbare GitHub-Verbindung kann Repository-Dateien ändern, aber nicht die About-Beschreibung oder Topics in den Repository-Einstellungen. Diese beiden Metadaten müssen in GitHub manuell eingetragen werden.

## Entwicklungsgrundsätze

- Kostenfreie Nutzung ohne Werbeeinblendungen als Projektziel.
- Keine kostenpflichtige Plattform als zwingende Voraussetzung.
- Keine nicht implementierten Funktionen als verfügbar darstellen.
- Keine vollständige rechtliche, technische oder Barrierefreiheits-Zertifizierung behaupten.
- Jede wesentliche rechtliche Änderung löst eine Aktualitätsprüfung aus.
- Projektbeschreibung, Nutzungsbedingungen, README und Systemanweisung müssen dieselbe Rollen- und Nutzungslogik wiedergeben.

## Nicht Bestandteil dieses Repositories

Android-App, Termux, Tesseract, lokale OCR, PDF-Rendering, dauerhafte Schwärzung, Metadatenbereinigung und lokaler Export gehören ausschließlich zum separaten Repository Anonymisator.

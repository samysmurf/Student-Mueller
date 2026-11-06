# Changelog

## [Unreleased]

- Skills-only-Plugin als zusätzliche Bereitstellungsform vorbereitet; Core V1.5.1 bleibt die fachliche Grundlage.
- Technisches Plugin-Paket 0.1.0 mit portablem Manifest, einem Skill und unveränderter Core-Referenz V1.5.1 im Entwicklungszweig angelegt.
- Eigenständigen Skill-Testplan mit Aktivierungsprüfungen, 21 Core-Regressionsfällen und verbindlichem V-A09-Freigabekriterium ergänzt.
- Kein MCP-Server, keine API, keine Datenbank und keine eigene Laufzeit vorgesehen.
- Eigenständiges quadratisches Logo und Composer-Icon als SVG erstellt, im OpenAI-Interface verknüpft und formal validiert.
- Portables Manifest an das offizielle Agent-Plugins-Root-Schema angepasst; Codex-spezifisches `skills`-Feld entfernt.
- Öffentliche Einreichung bleibt bis zum frischen V-A09-Laufzeittest, den Branding-Assets und der OpenAI-Paketprüfung gesperrt.


## [1.5.1] – Vorbereitungsstand vom 05.11.2026

- Barrierearme Antwort- und Dialogregeln in die Systemanweisung aufgenommen.
- Verständlichkeit, Screenreader-Nutzung, Textalternativen, lineare Lesbarkeit und Nutzerkontrolle präzisiert.
- Keine zusätzlichen Diagnose- oder Behinderungsfragen in das Erststartmenü aufgenommen.
- Klarstellung: Eine vereinfachte Erklärung ist nicht automatisch „Leichte Sprache“.
- Technische Grenzen externer KI-Plattformen von Anforderungen an eine künftig eigene Oberfläche getrennt.
- Barrierefreiheitsleitlinie und zwölf konkrete Prüffälle ergänzt; tatsächliche Plattform-, Geräte- und Screenreadertests sind noch offen.
- Rechtsrahmen anhand der amtlich konsolidierten BGG- und BITV-Texte eingeordnet; keine pauschale Anwendbarkeit, Freistellung oder Konformität behauptet.
- Nicht amtlich bestätigte Änderungsangaben zur BITV 2.0 nicht übernommen.
- V1.5.0 bleibt als fachlicher Ausgangsstand und bestehendes Testprotokoll nachvollziehbar.

## [1.5.0] – 2026-11-05

- Systemanweisung V1.5.0 konsolidiert und im Repository veröffentlicht.
- Verbindliches Erststartmenü mit Bundesland, Thema und Nutzungskontext aufgenommen.
- Bundesrecht und einschlägiges Landesrecht systematisch getrennt; Bundesland wird nicht aus Standortdaten abgeleitet.
- Antwortmodell mit verständlicher Erklärung und präziser rechtlicher Prüfung verbindlich gemacht.
- Rechtsstands- und Abrufdatumsstandard sowie Anforderungen an Primärquellen und Rechtsprechungsnachweise erweitert.
- Betreuungsrecht mit BGB, FamFG, BtOG, VBVG und landesrechtlichen Schnittstellen ausgebaut.
- FamFG-Zuordnung präzisiert: § 298 FamFG betrifft Verfahren nach § 1829 BGB; ärztliche Zwangsmaßnahmen nach § 1832 BGB sind in § 312 Nr. 3 FamFG als Unterbringungssachen erfasst.
- BtOG nach seiner gesetzlichen Gliederung geordnet; § 8 BtOG als zentrale Norm zu Beratung, Vermittlung anderer Hilfen und erweiterter Unterstützung hervorgehoben.
- BVerfG-Entscheidung vom 26.11.2024 – 1 BvL 1/24 – und Fortgeltung des bisherigen § 1832 BGB bis zum Inkrafttreten einer Neuregelung berücksichtigt.
- Rechtslage zur Beendigung und Vermögensübersicht nach §§ 1872 und 1873 BGB ab 01.01.2026 berücksichtigt.
- Wahlrecht, Geschäftsfähigkeit und Einwilligungsvorbehalt voneinander abgegrenzt.
- Änderungen des SGB II ab 2026 einschließlich § 65a Absatz 4 SGB II berücksichtigt.
- RDG-Prüfreihenfolge für Angelegenheiten Dritter differenziert; persönliche Unterstützung wird nicht pauschal ausgeschlossen.
- 21 manuelle Regel- und Konsistenztests dokumentiert; keine automatisierten oder Live-Plattformtests behauptet.
- README, Nutzungsbedingungen, Projektbeschreibung, GitHub-Profiltext, Funktionsstatus, Architektur, Datenschutz und Roadmap auf V1.5.0 abgestimmt.
- GitHub-About-Text und Topic-Vorschläge als Projektdatei dokumentiert. Die Repository-Metadaten selbst müssen mangels verfügbarer Schreibfunktion manuell aktualisiert werden.
- Projektgrenze zum eigenständigen Repository Anonymisator beibehalten.

## [1.4.0] – 2026-11-04

- Student Müller auf den promptbasierten sozialrechtlichen Informations- und Selbsthilfeassistenten abgegrenzt.
- Android-/OCR-/Termux-Arbeiten als eigenständiges Projekt Anonymisator verlinkt.
- README, Systemanweisung, Roadmap, Architektur, Datenschutz und Funktionsstatus auf die Projekttrennung ausgerichtet.
- Mindmap V1.4 als Mermaid-Text und SVG-Grafik ergänzt.
- Barrierefreiheitsleitlinie als Entwicklungsziel dokumentiert; keine Konformitätsprüfung behauptet.
- Bestehende Lizenzdateien unverändert gelassen.
- Architektur- und Datenschutzdokumentation auf die externe KI-Plattform und die Projektgrenze abgestimmt.

## [1.3.1] – 2026-11-04

- Frühere Nutzungsbeschreibung und Haftungshinweise präzisiert.
- Projektbeschreibung auf „gemeinwohlorientiert“ statt steuerrechtlich missverständlichem „gemeinnützig“ präzisiert.
- Klarstellung: Die Zweckbestimmung der Assistentenfassung ändert die bestehenden Lizenzen Apache 2.0 und CC BY-SA 4.0 nicht.
- Keine anwaltliche Prüfung oder rechtliche Freigabe behauptet.

## [1.3] – 2026-11-04

- Erstveröffentlichung der Projektbasis im öffentlichen Repository.
- Lizenzmodell festgelegt: eigener Programmcode Apache-2.0, Projektdokumentation CC BY-SA 4.0.
- Termux-/Android-Vorarbeiten genauer beschrieben.
- Tesseract 5.5.4, verfügbare Sprachdaten deu/eng und einen ersten lokalen OCR-Test dokumentiert; Qualitätsprüfung und weitere Integration bleiben offen.
- Dokumentationsstruktur für Architektur, Datenschutz, Roadmap, Funktionsstatus und Mitwirkung angelegt.
- Textbasierten Musterfall zur Küchen-Erstausstattung erstellt.

# Student Müller – Skills-only-Plugin

Dieses Verzeichnis enthält das portable Plugin-Paket für die öffentliche Einreichung im OpenAI Plugins Directory.

## Architektur

- Ein portables Plugin-Manifest: `plugin.json`
- Ein Skill: `skills/student-mueller/SKILL.md` (portable Agent-Plugins erkennen ihn automatisch über den Root-Ordner `skills/`; kein zusätzliches Manifestfeld erforderlich)
- Eine vollständige fachliche Referenz: `skills/student-mueller/references/SYSTEMANWEISUNG_V1.5.1.md`
- Kein MCP-Server
- Keine API oder externe Laufzeit
- Keine Datenbank und keine eigene Fallannahme
- Keine Zugangsdaten oder Secrets

## Fachliche Quelle

Die Skill-Referenz ist eine unveränderte Übernahme der im Entwicklungszweig `vision/v1.5.1-barrierefreiheit` geführten Hauptdatei `SYSTEMANWEISUNG.md`, Version V1.5.1, Stand 05.11.2026. Sie enthält die freigegebene Ergänzung zur differenzierten Prüfung des § 40 SGB II sowie die redaktionelle Abschlusskontrolle. Bei jeder Core-Aktualisierung muss geprüft werden, ob die Referenz im Plugin-Paket synchronisiert werden muss.

## Versionierung

- Core-Version: V1.5.1
- Plugin-Paketversion: 0.1.0 (erste technische Verpackung)
- Core- und Plugin-Version sind getrennt. Eine neue Plugin-Paketversion darf nicht automatisch eine neue fachliche Core-Version vortäuschen.

## Branding

- [Logo als SVG](assets/logo.svg)
- [Composer-Icon als SVG](assets/composer-icon.svg)
- Beide Grafiken sind quadratische Vektordateien mit 1024 × 1024 ViewBox und werden im Manifest referenziert.
- Primärfarbe: `#102F55`; Akzentfarbe: `#F8C84A`.

## Lizenz

Die originären Projekttexte und Skill-Anweisungen unterliegen der im Hauptrepository festgelegten CC BY-SA 4.0. Die Lizenz- und Herkunftshinweise im Hauptrepository bleiben maßgeblich.

## Vor einer öffentlichen Einreichung offen

1. Die integrierten quadratischen SVG-Dateien für `interface.logo` und `interface.composerIcon` im Submission-Portal auf korrekte Darstellung prüfen.
2. Publisher-Identität im Submission Portal auswählen und verifizieren. Der Eintrag `interface.developerName` wird bei der Einreichung automatisch aus der ausgewählten verifizierten Entwickleridentität gesetzt.
3. Finale Listing-Angaben und Kategorie prüfen.
4. Skill in einer unterstützten ChatGPT-Umgebung installieren und tatsächlich testen.
5. Skill-Aktivierung, Startmenü, §-40-SGB-II-Ausgabe, Barrierefreiheit und fachliche Regression dokumentieren.
6. Vollständiges ZIP aus dem Inhalt dieses Verzeichnisses erstellen, nicht aus dem gesamten GitHub-Repository.
7. Automatische Paket- und Skill-Prüfungen im Portal erfolgreich durchlaufen.

Der Skill-Testplan steht in [TESTPLAN_SKILL.md](TESTPLAN_SKILL.md). Das Core-Testprotokoll bleibt separat und wird nicht als Plugin-Laufzeittest ausgegeben.

Dieses Paket ist ein Entwicklungsstand und noch keine von OpenAI genehmigte oder veröffentlichte App.

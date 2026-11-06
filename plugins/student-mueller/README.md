# Student Müller – Skills-only-Plugin

Dieses Verzeichnis enthält das portable Plugin-Paket für die öffentliche Einreichung im OpenAI Plugin Directory.

## Architektur

- Ein Plugin-Manifest: `plugin.json`
- Ein Skill: `skills/student-mueller/SKILL.md`
- Eine vollständige fachliche Referenz: `skills/student-mueller/references/SYSTEMANWEISUNG_V1.5.0.md`
- Kein MCP-Server
- Keine API oder externe Laufzeit
- Keine Datenbank und keine eigene Fallannahme
- Keine Zugangsdaten oder Secrets

## Fachliche Quelle

Die Skill-Referenz ist eine unveränderte Übernahme der im Repository geführten `SYSTEMANWEISUNG.md`, Version V1.5.0, Stand 05.11.2026. Bei jeder Core-Aktualisierung muss geprüft werden, ob die Referenz im Plugin-Paket synchronisiert werden muss.

## Versionierung

- Core-Version: V1.5.0
- Plugin-Paketversion: 0.1.0 (erste technische Verpackung)
- Skill-Version: an Core-Version und Plugin-Paketversion gebunden; Änderungen müssen dokumentiert und getestet werden.

Core- und Plugin-Version sind bewusst getrennt. Eine neue Plugin-Paketversion darf nicht automatisch eine neue fachliche Core-Version vortäuschen.

## Lizenz

Die originären Projekttexte und die Skill-Anweisungen unterliegen der im Hauptrepository festgelegten CC BY-SA 4.0. Die Lizenz- und Herkunftshinweise im Hauptrepository bleiben maßgeblich.

## Vor einer öffentlichen Einreichung offen

1. Plugin-Paket mit dem offiziellen OpenAI-Validator bzw. Upload-Prüfungen testen.
2. Listing-Metadaten und Publisher-Bezeichnung mit der verifizierten Entwickleridentität abgleichen.
3. Kategorie und öffentliche Darstellung im Einreichungsportal bestätigen.
4. Skill-Aktivierung, Startmenü, Quellenverhalten und sämtliche relevanten V1.5-Testfälle in einer unterstützten ChatGPT-Umgebung testen.
5. Sicherstellen, dass der ZIP-Root genau einen Plugin-Ordner bzw. eine Plugin-Wurzel enthält und keine Dateien außerhalb des Plugin-Pakets.

Dieses Paket ist ein Entwicklungsstand und noch keine von OpenAI genehmigte oder veröffentlichte App.

# ChatGPT-Plugin – Skills-only-Architektur

**Status:** Entwicklungszweig `feature/skills-only-plugin`  
**Core-Basis:** Student Müller V1.5.0, Stand 05.11.2026  
**Plugin-Paket:** 0.1.0 (technischer Erstentwurf)  
**Architekturentscheidung:** Skills-only, ohne MCP-Server

## 1. Zweck

Das bestehende promptbasierte Projekt Student Müller erhält eine zusätzliche, installierbare Paketform für die öffentliche Aufnahme in das OpenAI Plugins Directory.

Die bisherige Systemanweisung bleibt die fachliche Core-Quelle. Das Plugin ist eine zusätzliche Bereitstellungsform und ersetzt weder die bestehende Prompt-Veröffentlichung noch die eigenständige Nutzung auf anderen KI-Plattformen.

## 2. Architekturentscheidung

Student Müller benötigt für den aktuellen Funktionsumfang keinen eigenen MCP-Server.

Das Plugin enthält:
- ein portables `plugin.json`-Manifest;
- einen Skill unter `skills/student-mueller/SKILL.md`;
- eine unveränderte Kopie der Core-Systemanweisung als Skill-Referenz;
- Paket- und Testdokumentation.

Das Plugin enthält ausdrücklich nicht:
- `mcp.json` oder `.mcp.json`;
- `.app.json` oder registrierte App-Referenzen;
- API-Endpunkte, Servercode oder Zugangsdaten;
- eine Datenbank oder eigene Fallannahme;
- lokale OCR, PDF-Schwärzung oder Metadatenbereinigung.

Die Recherche und die Erzeugung der Antworten erfolgen mit den Werkzeugen und Möglichkeiten der jeweils verwendeten ChatGPT-Umgebung. Der Skill selbst stellt keine externen Datenquellen oder Werkzeuge bereit.

## 3. Übernahme der fachlichen Core-Version

Die Datei `skills/student-mueller/references/SYSTEMANWEISUNG_V1.5.0.md` ist eine unveränderte Kopie der Hauptdatei `SYSTEMANWEISUNG.md` aus Core V1.5.0.

Der Skill weist das Modell an, diese vollständige Referenz als fachliche Arbeitsgrundlage zu berücksichtigen. Die Referenzkopie muss bei jeder Core-Änderung auf Synchronität geprüft werden.

Core-Version und Plugin-Paketversion sind getrennt:
- Core V1.5.0 beschreibt den fachlichen Regelstand.
- Plugin 0.1.0 beschreibt die erste technische Paketierung.

Eine Änderung am Plugin-Paket darf keine fachliche Core-Änderung vortäuschen. Eine Änderung am Core darf nicht unbemerkt in einer veröffentlichten Skill-Version verbleiben.

## 4. Offizielles Paketformat

Die Implementierung folgt dem portablen Agent-Plugins-Paketformat:
- Root-Manifest `plugin.json`;
- Skill-Verzeichnis `skills/<skill-name>/`;
- Pflichtdatei `SKILL.md`;
- optionale Referenzdateien im Unterordner `references/`.

Ein portables Paket erkennt Skills unter dem Root-Verzeichnis `skills/` automatisch. Ein MCP-Manifest ist nicht erforderlich und wird bewusst nicht angelegt.

Offizielle Dokumentation:
- https://developers.openai.com/plugins/build/skills
- https://developers.openai.com/plugins/build/plugins
- https://developers.openai.com/plugins/deploy/submission
- https://developers.openai.com/plugins/deploy/submission-errors

## 5. Öffentliche Einreichung

Für die öffentliche Aufnahme wird im Plugin Submission Portal der Typ **Skills only** gewählt. Das ZIP enthält die Plugin-Wurzel mit Manifest und mindestens einem gültigen Skill.

Nach der aktuellen OpenAI-Dokumentation:
- benötigt die einreichende Organisation die Berechtigung Apps Management Write;
- muss eine persönliche oder geschäftliche Entwickleridentität verifiziert sein;
- werden Skills durch die automatischen Prüfungen kontrolliert;
- werden Skills-only-Plugins nach Genehmigung im gemeinsamen Plugins Directory veröffentlicht;
- sind die fünf positiven und drei negativen Testfälle sowie ein Demo-Video der initialen MCP-Prüfung für Skills-only nicht erforderlich;
- müssen Änderungen an Metadaten oder gebündelten Skills als neue ZIP-Paketversion hochgeladen werden.

## 6. Offene Einreichungsvoraussetzungen

Vor der Einreichung sind mindestens folgende Punkte zu erledigen:
1. quadratische Logo- und Composer-Icon-Dateien erstellen und im Manifest referenzieren;
2. Publisher-Identität im Submission Portal auswählen und verifizieren;
3. finale Listing-Angaben und Kategorie prüfen;
4. Skill in einer unterstützten ChatGPT-Umgebung installieren und tatsächlich testen;
5. Aktivierung, Nicht-Aktivierung, Startmenü und fachliche Regression dokumentieren;
6. vollständiges ZIP aus dem Inhalt von `plugins/student-mueller/` erstellen, nicht aus dem gesamten GitHub-Repository;
7. automatische Paket- und Skill-Prüfungen im Portal erfolgreich durchlaufen.

Die öffentlichen URL-Felder für Website, Datenschutz, Nutzungsbedingungen und Support sind bei Skills-only-ZIP-Einreichungen laut aktueller Fehlerreferenz optional. Die bereits vorhandenen Projektseiten bleiben dennoch als transparente Informationsquellen verlinkt.

## 7. Teststatus

Das Paket besitzt einen eigenen Testplan unter `plugins/student-mueller/TESTPLAN_SKILL.md`.

Die 21 Core-Prüffälle aus `docs/TESTPROTOKOLL_V1.5.md` bleiben unverändert und werden als fachliche Regression genutzt. Sie sind keine tatsächlichen ChatGPT-Laufzeittests.

Bisher erfolgte statische Prüfung:
- Manifest ist parsebares JSON.
- Skill-Datei besitzt YAML-Frontmatter mit Name und Beschreibung.
- Skill-Verzeichnis liegt unmittelbar unter `skills/`.
- Core-Referenz stimmt textlich vollständig mit der Hauptdatei `SYSTEMANWEISUNG.md` überein.
- Kein MCP-Manifest und keine MCP-Abhängigkeit vorhanden.

Noch nicht erfolgt:
- ZIP-Upload und OpenAI-Validatorprüfung;
- Skill-Installation in ChatGPT;
- tatsächliche Aktivierungs- und Regressionstests;
- OpenAI-Review und öffentliche Veröffentlichung.

## 8. Änderungs- und Freigabeprinzip

Der Entwicklungszweig verändert die bestehende Core-Version nicht. Die Integration in `main` erfolgt erst nach Prüfung des vollständigen Pakets und der Dokumentation.

Eine öffentliche Veröffentlichung wird erst nach erfolgreicher Paketvalidierung, dokumentierten Laufzeittests und abgeschlossener Prüfung der Listing-Assets und Entwickleridentität vorbereitet.

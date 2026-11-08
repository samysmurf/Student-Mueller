# Assistent Mueller – Plugin-Prototyp 0.1.1

**Status:** privater Test vorgesehen · **Basis:** Student Müller V1.5.1

Dieses Verzeichnis enthält die portable Skills-only Plugin-Quelle für **Assistent Mueller**. Es bündelt die vier ausdrücklich benannten Rollen, ein Chronik-Modul und eine zentrale Steuerung:

- `@student Müller` – deutsches Sozial- und Betreuungsrecht, Selbsthilfe und verständliche Einordnung
- `@rdg` – unabhängige Prüfung der Grenzen nach dem Rechtsdienstleistungsgesetz
- `@Vision` – barrierearme, screenreaderfreundliche und verständliche Kommunikation
- `@Siggi` – technische und konzeptionelle Projektbegleitung
- `Chronik` – strukturierte Dokumentation von Nutzerangaben, E-Mails und Kalenderdaten, soweit diese tatsächlich verfügbar sind
- `Assistent-Steuerung` – zentrale Koordination und Routing

## Aufbau

```text
assistent-mueller/
├── plugin.json
└── skills/
    ├── assistent-steuerung/SKILL.md
    ├── student-sozialrecht/SKILL.md
    ├── rdg-pruefung/SKILL.md
    ├── vision-barrierefreiheit/SKILL.md
    ├── chronik-dokumentation/SKILL.md
    └── siggi-projektbegleitung/SKILL.md
```

## Wichtige Funktionsgrenzen

Dies ist zunächst ein Skills-only-Prototyp. Er enthält **keinen eigenen MCP-Server, keine eigene Datenbank, keine App-Oberfläche und keine automatisch verbundenen Konten**.

- Gmail- und Google-Kalenderdaten dürfen nur verwendet werden, wenn die jeweilige Verbindung in der aktuellen ChatGPT-Umgebung tatsächlich verfügbar ist und der Nutzer die betreffende Nutzung veranlasst.
- Ein Skill allein kann keine E-Mails oder Kalenderdaten abrufen, erstellen, ändern oder versenden.
- Telefonate werden ausschließlich als vom Nutzer berichtete Angaben dokumentiert. Es gibt keine automatische Telefon-, Anruflisten- oder Gesprächsaufzeichnung.
- Es gibt keine automatische Synchronisation, keine Hintergrundüberwachung und keine eigenständige Fallannahme.
- Das Plugin vertritt keine Person gegenüber Behörden, Gerichten oder Dritten und versendet keine Schreiben.
- Die Android-Anonymisierung/OCR ist ein separates Projekt und keine Funktion dieses Plugins.

## First Start

Vor der Nutzung der Chronik bitte die [First-Start-Anleitung](FIRST_START.md) lesen. Gmail und Google Calendar müssen im persönlichen ChatGPT-Konto separat installiert und verbunden werden. Das Assistent-Mueller-Plugin erledigt dies nicht automatisch.

## Verwendung und Test

Der Prototyp ist für persönliche Tests mit synthetischen oder ausreichend anonymisierten Beispielen gedacht. Vor einem realen Einsatz müssen die jeweils aktuelle Rechtslage, die Qualität der Antworten, die tatsächlich verfügbaren Plattformfunktionen und die Datenschutzbedingungen geprüft werden.

Die Plugin-Quelle liegt auf einem eigenen Git-Branch. Da das GitHub-Repository öffentlich ist, sind auch die dort abgelegten Plugin-Dateien öffentlich einsehbar. „Privater Test“ bezeichnet die beabsichtigte Plugin-Installation bzw. Freigabe, nicht die Vertraulichkeit dieses Repository-Zweigs.

## Lizenzhinweis

Die Lizenzzuordnung des Hauptprojekts bleibt maßgeblich: Projekttexte und Dokumentation grundsätzlich CC BY-SA 4.0; eigener Programmcode grundsätzlich Apache-2.0. Drittinhalte und Rechte Dritter sind gesondert zu behandeln. Siehe die Lizenzdateien im Repository-Stamm.

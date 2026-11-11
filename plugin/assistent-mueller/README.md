# Assistent Mueller – Plugin 1.0.0-alpha.4 (Quellkandidat)

**Status:** Quellkandidat auf Feature-Branch; noch nicht in die private Plugin-Instanz importiert · **Basis:** Student Müller V2.0.0 · **Paketversion im Quellkandidaten:** 1.0.0-alpha.4 · **bisherige private Plugin-Instanz:** 1.0.0-alpha.3

**Private Testinstanz:** Die persönliche Installation ist kontogebunden. Der individuelle Installationslink wird nicht im öffentlichen Quellverzeichnis veröffentlicht.

Dieses Verzeichnis enthält die portable Skills-only Plugin-Quelle für **Assistent Mueller**. Es bündelt die vier ausdrücklich benannten Rollen, die Chronik, eine eigenständige Aussagenherkunftsprüfung und eine zentrale Steuerung:

- `@student Müller` – deutsches Sozial- und Betreuungsrecht, Selbsthilfe und verständliche Einordnung
- `@rdg` – unabhängige Prüfung der Grenzen nach dem Rechtsdienstleistungsgesetz
- `@Vision` – barrierearme, screenreaderfreundliche und verständliche Kommunikation
- `@Siggi` – technische und konzeptionelle Projektbegleitung
- `Chronik` – strukturierte Dokumentation von Nutzerangaben, E-Mails und Kalenderdaten, soweit diese tatsächlich verfügbar sind
- `Aussagenherkunft` – Rekonstruktion von Ursprungsquelle, Beobachtungsgrundlage, Empfängern, Weiterleitungen und Gegendarstellungen
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
    ├── aussagen-provenienz/SKILL.md
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


## Version 1.0.0-alpha.1

Alpha-Release mit sechs modularen Skills. Die Version ist für weitere synthetische Tests vorgesehen und keine juristische Zertifizierung oder Freigabe für ungeprüfte reale Fälle.


## Version 1.0.0-alpha.2 – 09.11.2026

- Nutzerbestätigter Integrationstest in einer neuen ChatGPT-Instanz mit allen sechs Skills: bestanden.
- Nutzerbestätigtes Update auf 1.0.0-alpha.2: bestanden.
- Allgemeiner Teststatus und Abgrenzung der Prüfebenen: siehe [TESTPROTOKOLL_PLUGIN_ALPHA.md](TESTPROTOKOLL_PLUGIN_ALPHA.md).
- Die Bestätigung ist als Nutzerangabe dokumentiert; sie ist keine unabhängig reproduzierte automatisierte Host-Prüfung.


## Version 1.0.0-alpha.3 – 11.11.2026

- Metadatenkorrektur: Autor im Plugin-Manifest auf **Andreas Brill** gesetzt.
- Paketversion an die private Plugin-Veröffentlichung 1.0.0-alpha.3 angeglichen.
- Keine Skill-Inhalte oder Funktionsabläufe geändert; der bestätigte Integrationstest aus alpha.2 wird dadurch nicht als neuer Test ausgegeben.

## Version 1.0.0-alpha.4 – Entwicklungsbranch / Quellkandidat

- Neues Modul **Aussagenherkunft** zur Trennung von Dokumenteninhalt, Beobachtungsgrundlage und tatsächlichem Wahrheitsgehalt.
- Rekonstruiert Erstquelle, zeitliche Abfolge, Empfänger, Weiterleitungen, Zitate und Gegendarstellungen.
- Verhindert, dass abhängige Wiederholungen ohne unabhängige Quelle als Mehrfachbestätigung gezählt werden.
- Ergänzt einen Testplan mit acht ausschließlich synthetischen Fällen.
- Die Chronik bleibt eigenständig und wird nur um eine Verknüpfung zur Provenienzprüfung ergänzt.
- **Noch nicht importiert und nicht hostgetestet.** Die bestehende private Plugin-Instanz bleibt alpha.3, bis ein separater Import und Test erfolgt.

# Assistent Mueller – Plugin 1.0.0-alpha.4 (öffentlicher Veröffentlichungskandidat)

**Status:** Vorbereitung für eine mögliche öffentliche Einreichung · **Basis:** Student Müller V2.0.0 · **Paketversion:** 1.0.0-alpha.4

Assistent Mueller ist ein deutschsprachiges Skills-only-Plugin mit sechs modularen Arbeitsanweisungen:

- Sozial- und Betreuungsrecht mit verständlicher Erklärung und Quellenprüfung
- eigenständige RDG-Grenzprüfung
- barrierearme und screenreaderfreundliche Kommunikation
- Chronik-Dokumentation aus Nutzerangaben und tatsächlich verfügbaren Dokumenten
- technische und konzeptionelle Projektbegleitung
- zentrale Steuerung und Modulrouting

## Technische Grenzen

Das Plugin enthält keinen eigenen MCP-Server, keine Datenbank, keine eigene Chat-Oberfläche, keine Telemetrie und keine automatisch verbundenen Konten.

- Gmail und Google Calendar sind separate ChatGPT-Apps. Nutzer müssen sie selbst installieren, verbinden und Berechtigungen prüfen.
- Ein Skill allein kann keine Daten aus E-Mail- oder Kalenderkonten abrufen oder verändern.
- Telefonate werden ausschließlich als vom Nutzer berichtete Angaben dokumentiert. Es gibt keine automatische Telefonie-, Anruflisten- oder Aufzeichnungsfunktion.
- Keine automatische Synchronisation, Hintergrundüberwachung, eigenständige Fallannahme oder Vertretung gegenüber Dritten.
- Die Android-Anonymisierung/OCR ist ein getrenntes Projekt und keine Plugin-Funktion.

## Eigenverantwortung und fachliche Grenzen

Das Plugin liefert KI-gestützte Informationen und Entwürfe, keine verbindliche Rechtsauskunft. Jeder Nutzer ist selbst dafür verantwortlich, Eingaben und Ergebnisse zu prüfen. Vor jeder Verwendung müssen insbesondere die für den konkreten Sachverhalt maßgeblichen aktuellen und historischen Gesetzesfassungen, Rechtsprechung, Fristen, Zuständigkeiten, Tatsachen, Quellen und Formvorschriften eigenständig kontrolliert werden.

KI-Ausgaben können falsch, unvollständig oder veraltet sein. Keine anwaltliche Beratung, Rechtsvertretung, Zertifizierung oder Garantie eines bestimmten Ergebnisses. Die Haftung richtet sich nach geltendem Recht; zwingende gesetzliche Haftung bleibt unberührt. Die Bedingungen von OpenAI gelten eigenständig und werden durch dieses Projekt weder geändert noch ausgeschlossen.

## Datenschutz und Support

- [Datenschutzhinweise](https://github.com/samysmurf/Student-Mueller/blob/main/docs/DATENSCHUTZ.md)
- [Nutzungsbedingungen](https://github.com/samysmurf/Student-Mueller/blob/main/NUTZUNGSBEDINGUNGEN.md)
- [Öffentlicher GitHub-Support](https://github.com/samysmurf/Student-Mueller/blob/main/SUPPORT.md)

Bitte keine personenbezogenen Falldaten, Aktenzeichen, Gesundheitsdaten oder vertraulichen Unterlagen in öffentlichen GitHub-Issues veröffentlichen.

## Aufbau

```text
assistent-mueller/
├── plugin.json
├── README.md
├── FIRST_START.md
└── skills/
    ├── assistent-steuerung/SKILL.md
    ├── student-sozialrecht/SKILL.md
    ├── rdg-pruefung/SKILL.md
    ├── vision-barrierefreiheit/SKILL.md
    ├── chronik-dokumentation/SKILL.md
    └── siggi-projektbegleitung/SKILL.md
```

## Versionshinweis

Alpha.4 ist ein vorbereiteter Veröffentlichungskandidat. Die Version enthält Listing-Metadaten, Support- und Richtlinienverweise sowie redaktionelle Präzisierungen zur Eigenverantwortung. Sie ist **noch nicht öffentlich im ChatGPT-Verzeichnis veröffentlicht oder von OpenAI freigegeben**. Ein Nutzerbestätigter Integrationstest der sechs Skills aus einer früheren Alpha-Version ist keine unabhängige Auditierung und keine juristische Zertifizierung.

## Lizenz

Die Lizenzzuordnung des Hauptprojekts bleibt maßgeblich: originäre Projekttexte und Dokumentation grundsätzlich CC BY-SA 4.0; eigener Programmcode grundsätzlich Apache-2.0. Drittinhalte und Rechte Dritter sind gesondert zu beachten.

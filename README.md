# Student Müller

**Verstehen. Prüfen. Selbstbestimmt handeln.**

**Aktuelle Fassung: V2.0.0 · Stand: 08.11.2026**

Student Müller ist ein kostenfreies, werbefreies Open-Source-Informations- und Selbsthilfeprojekt. Veröffentlicht wird eine kopierbare Systemanweisung für einen KI-Dienst der eigenen Wahl. Einzelne Nutzer übernehmen den Prompt selbstständig in ihren eigenen Chat und entscheiden eigenständig über dessen Verwendung.

Das Projekt betreibt keinen eigenen Chatbot-Server, keine Fallannahme und keine Plattform zur Bearbeitung fremder Fälle.

## Projektidee

Student Müller unterstützt Menschen dabei, deutsches Sozialrecht, Betreuungsrecht und angrenzende Rechtsgebiete verständlich einzuordnen, Bescheide und behördliche Schreiben zu prüfen, amtliche Rechtsquellen zu finden und eigene Anträge oder Schreiben vorzubereiten.

Die Systemanweisung V2.0.0 enthält insbesondere:

- ein Startmenü, das beim ersten Prompt-Aufruf erscheint,
- die ausdrückliche Abfrage des Bundeslandes, des Themas und des Nutzungskontexts,
- die Trennung von bundesweit geltendem Bundesrecht und ergänzendem Landesrecht,
- Antworten auf zwei Ebenen: verständliche Erklärung und präzise rechtliche Prüfung,
- einen verbindlichen Quellenstandard mit Rechtsstand, Abrufdatum und Primärquellen,
- ein erweitertes Betreuungsrechtsmodul einschließlich BGB, FamFG, BtOG und VBVG,
- eine differenzierte Prüfung von Unterstützung in Angelegenheiten anderer Personen anhand der tatsächlichen Rolle und des RDG,
- strukturierte Bescheid-, Fristen- und Schriftsatzabläufe,
- eine vertiefte Prüfung von Unterkunfts- und Heizkosten nach § 22 SGB II einschließlich Heizspiegel-Datengrundlage, Warnfunktion und Chronologie.

V2.0.0 ist ein Prompt und eine Dokumentation. Es ist weder eine staatlich anerkannte Rechtsanwendung noch eine anwaltlich zertifizierte oder unabhängig extern freigegebene Software.

## Student Müller ausprobieren

1. [ChatGPT öffnen](https://chatgpt.com/) oder einen anderen geeigneten KI-Dienst verwenden.
2. Die vollständige [Systemanweisung V2.0.0](SYSTEMANWEISUNG.md) öffnen und in einen neuen Chat übernehmen.
3. Das beim Erststart angezeigte Menü beantworten: Bundesland, Thema und Nutzungskontext.
4. Zunächst eine einfache, nicht vertrauliche Testfrage verwenden.
5. Für einen Dokumentenworkflow den vollständig fiktiven [Übungsfall Küchen-Erstausstattung](docs/BEISPIELFALL_KUECHENERSTAUSSTATTUNG.md) verwenden.

Der Beispielordner enthält synthetische Unterlagen, Testanfragen und Vergleichspunkte. Für diesen Test sind keine echten Dokumente, Screenshots oder Bild-Uploads erforderlich. Der Übungsfall ist keine Vorlage zur ungeprüften Übertragung auf reale Fälle.

## Bundesland und Rechtsraum

Beim ersten Start fragt Student Müller ausdrücklich nach dem Bundesland, in dem die Angelegenheit rechtlich verortet ist. Standortdaten oder Vermutungen ersetzen diese Auswahl nicht.

Bundesrecht gilt bundesweit. Ergänzend werden das für den konkreten Sachverhalt relevante Landesrecht und die landesspezifischen Zuständigkeiten berücksichtigt. Bei mehreren betroffenen Bundesländern wird geklärt, welches Land für die konkrete Behörde, das Gericht, die Einrichtung oder den Lebenssachverhalt maßgeblich ist. Bei Bedarf wird zusätzlich der konkrete Ort oder die Kommune abgefragt.

## Fachlicher Umfang

| Themenfeld | Beispiele |
|---|---|
| Grundsicherung und Sozialhilfe | SGB II, SGB XII, Unterkunft, Mehrbedarf, Erstausstattung |
| Kranken- und Pflegeversicherung | SGB V und SGB XI |
| Rehabilitation und Teilhabe | SGB IX, Schwerbehindertenrecht, GdB |
| Rente und Erwerbsminderung | Anspruchsvoraussetzungen, Verfahren, Nachweise |
| Betreuungsrecht | BGB, FamFG, BtOG, VBVG, Vorsorgevollmacht |
| Landesrechtliche Unterbringung | jeweiliges Landes-PsychKG bzw. Unterbringungsrecht |
| Verwaltungsverfahren | Bescheidverständnis, Akteneinsicht, Fristen, Rechtsbehelfe |
| Eigene Korrespondenz | Entwürfe für Anträge, Widersprüche und Stellungnahmen |

Der Assistent soll Tatsachen, Dokumenteninhalt, Annahmen und rechtliche Schlussfolgerungen voneinander trennen, Quellen sichtbar machen, Unsicherheiten benennen und fehlende Angaben gezielt erfragen.

## Eigene Angelegenheiten und Unterstützung anderer Personen

Der Schwerpunkt liegt auf der eigenständigen Bearbeitung der eigenen Angelegenheiten. Eine Unterstützung bei Angelegenheiten von Angehörigen oder anderen Personen ist nicht pauschal ausgeschlossen.

Bei einer konkreten fremden Angelegenheit muss die tatsächliche Rolle des Nutzers geklärt und die rechtliche Einordnung insbesondere nach §§ 2, 3 und 6 RDG geprüft werden. Unentgeltlichkeit allein ist weder eine pauschale Freistellung noch ein pauschales Verbot.

Student Müller übernimmt keine Vertretung. Der Prompt-Entwickler nimmt keine fremden Fälle entgegen und bearbeitet keine individuellen Angelegenheiten im Namen anderer Personen. Einzelheiten und Grenzen stehen in den [Nutzungsbedingungen](NUTZUNGSBEDINGUNGEN.md).

## Grenzen, Plattform und Verantwortung

Student Müller ist keine Rechtsanwaltskanzlei, kein Gericht und keine Behörde. KI-Ausgaben können fehlerhaft, unvollständig oder veraltet sein. Nutzer müssen Tatsachen, Gesetzesfassungen, Quellen, Fristen, Formvorschriften, Anlagen und Versandwege vor einer Verwendung selbst kontrollieren. Der Assistent versendet keine Schreiben.

Eingaben und Ausgaben werden über die vom Nutzer gewählte externe KI-Plattform verarbeitet. Das Projekt kann deren technische Verarbeitung, Speicherung oder Bedingungen nicht steuern. Vor Eingabe vertraulicher Inhalte sind die Nutzungs- und Datenschutzhinweise des jeweiligen Anbieters zu prüfen. Nicht erforderliche personenbezogene Daten sollten zuvor durch neutrale Platzhalter ersetzt werden.

Die Haftung richtet sich nach geltendem Recht. Zwingende gesetzliche Haftung bleibt unberührt; ein pauschaler Ausschluss sämtlicher Ansprüche wird nicht erklärt.

## Assistent Mueller Plugin 1.0.0-alpha.2

Neben der kopierbaren Systemanweisung gibt es eine separate Skills-only-Plugin-Alpha mit sechs Skills für Steuerung, Sozialrecht, RDG-Prüfung, Barrierefreiheit, Chronik und technische Projektbegleitung. Die private Plugin-Instanz steht auf **1.0.0-alpha.2**. Der Nutzer hat am 09.11.2026 den Integrationstest in einer neuen ChatGPT-Instanz mit allen sechs Skills sowie das Update auf alpha.2 als bestanden bestätigt. Diese Abnahme ist als Nutzerbestätigung dokumentiert; sie ist kein unabhängig reproduzierter automatisierter Host-Test und keine juristische Zertifizierung.

**[Assistent Mueller direkt in ChatGPT öffnen](https://chatgpt.com/plugins/plugins_6af0c35601e08191b5292f62c1086ad8)** (private Plugin-Instanz; Anmeldung und Berechtigung erforderlich).

Der Quellcode liegt im öffentlichen Branch [plugin/assistent-mueller-v0.1.0](https://github.com/samysmurf/Student-Mueller/tree/plugin/assistent-mueller-v0.1.0/plugin/assistent-mueller). Die private Sichtbarkeit der Plugin-Instanz macht den GitHub-Branch nicht privat. Das Plugin besitzt keinen eigenen MCP-Server, keine Datenbank und keine automatische Fallannahme. Details zum Teststatus stehen im [Plugin-Alpha-Testprotokoll](plugin/assistent-mueller/TESTPROTOKOLL_PLUGIN_ALPHA.md) und im [SM-03-Reparaturprotokoll](plugin/assistent-mueller/TESTREPARATUR_SM-03.md).

## Projektgrenze: Anonymisator

Die lokale Android-Dokumentenverarbeitung ist ein eigenständiges Schwesterprojekt: [Anonymisator – separates Repository](https://github.com/samysmurf/Anonymisator).

Student Müller enthält keine eigene OCR-Engine, PDF-Schwärzungsfunktion, Metadatenbereinigung oder lokale Anonymisierungsfunktion. Es besteht keine gemeinsame Laufzeit, keine direkte KI-Schnittstelle und keine automatische Datenübertragung zwischen den Projekten. Student Müller setzt weder die Fertigstellung noch die Verfügbarkeit von Anonymisator voraus.

## Status V2.0.0

| Bereich | Stand |
|---|---|
| Systemanweisung V2.0.0 | in GitHub eingepflegt |
| Startmenü und Bundeslandauswahl | als Prompt-Regel integriert; Darstellung abhängig von der KI-Plattform |
| Sozial- und Betreuungsrecht | fachliche Module integriert; Aktualität je Einzelfall erneut zu prüfen |
| Quellen- und Aktualitätsprotokoll | als verbindliche Arbeitsregel integriert |
| SM-03 Plugin-Prüffall | simuliert und repariert | Integritätsprüfung des Alpha-Pakets bestanden; kein Live-End-to-End-Test |
| 21 V1.5-Prüffälle | manuell auf Prompt-Regel- und Konsistenzebene durchgespielt; keine Live-Plattformtests |
| Bescheidverständnis und Schriftsatzentwürfe | Arbeitsabläufe beschrieben; tatsächliche Ausgabe vom KI-Dienst abhängig |
| Native Android-App / lokale OCR | nicht Bestandteil; separates Projekt Anonymisator |
| unabhängige Rechtsprüfung / Zertifizierung | nicht behauptet |

Das [Testprotokoll V1.5](docs/TESTPROTOKOLL_V1.5.md) unterscheidet ausdrücklich zwischen konzeptioneller Prüfung und noch ausstehenden Laufzeittests. Weitere Angaben stehen im [Funktionsstatus](docs/FUNKTIONSSTATUS.md) und in der [Roadmap](ROADMAP.md).

## Dokumentation

- [Systemanweisung V2.0.0](SYSTEMANWEISUNG.md)
- [Nutzungsbedingungen und Nutzungshinweise](NUTZUNGSBEDINGUNGEN.md)
- [Projektbeschreibung](PROJEKTBESCHREIBUNG.md)
- [GitHub-Profiltext und Topics](GITHUB_PROJEKTPROFIL.md)
- [Testprotokoll V1.5](docs/TESTPROTOKOLL_V1.5.md)
- [Architektur](docs/ARCHITEKTUR.md)
- [Datenschutz](docs/DATENSCHUTZ.md)
- [Funktionsstatus](docs/FUNKTIONSSTATUS.md)
- [Roadmap](ROADMAP.md)
- [Barrierefreiheit – Entwicklungsleitlinie](docs/BARRIEREFREIHEIT.md)
- [Fiktiver Übungsfall Küchen-Erstausstattung](docs/BEISPIELFALL_KUECHENERSTAUSSTATTUNG.md)
- [Mitwirken](CONTRIBUTING.md) · [Sicherheitsmeldungen](SECURITY.md)

Die Mindmap V1.4.0 ist eine historische Projektübersicht und bildet die Erweiterungen aus V2.0.0 noch nicht vollständig ab.

## Lizenzen

- Eigener Programmcode: Apache License 2.0.
- Originäre Projekttexte und Dokumentation: CC BY-SA 4.0.
- Fremde Bibliotheken, Datensätze, Marken, amtliche Inhalte und sonstige Drittinhalte bleiben ihren jeweiligen Rechten und Lizenzbedingungen unterworfen.

Die Zuordnung und vollständigen Lizenzhinweise stehen in [LICENSE](LICENSE), [LICENSE-CODE](LICENSE-CODE), [LICENSE-DOCS.md](LICENSE-DOCS.md) und [LICENSE_DECISION.md](LICENSE_DECISION.md). Die Zweckbestimmung des Projekts ändert die Lizenzbedingungen nicht.

**Leitgedanke:** Ein niedrigschwelliges Werkzeug für Verständlichkeit, Selbstbestimmung und gesellschaftliche Teilhabe – mit transparenten Grenzen und überprüfbaren Quellen.

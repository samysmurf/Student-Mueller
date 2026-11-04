# Student Müller

**Verstehen. Verwalten. Selbstbestimmt handeln.**

![Student Müller – Projekt-Mindmap V1.4](assets/student_mueller_mindmap_v1.4.svg)

<sub>Projektübersicht zum Release V1.4.0. Die Mindmap unterscheidet den fachlichen Assistenten von dem eigenständigen Projekt Anonymisator.</sub>

## Projektidee

Student Müller ist ein kostenfreies, werbefreies, ChatGPT-basiertes Informations- und Selbsthilfeprojekt. Es soll Menschen dabei unterstützen, sozialrechtliche Sachverhalte verständlich einzuordnen, Verwaltungsentscheidungen zu strukturieren und die eigenen Angelegenheiten möglichst selbstbestimmt zu bearbeiten.

Das Projekt arbeitet quellenorientiert mit öffentlich zugänglichen Gesetzen, amtlichen Informationen und überprüfbarer Rechtsprechung. Es ist ein Open-Source-Projekt; daraus folgt weder eine staatliche Anerkennung noch eine rechtliche oder fachliche Zertifizierung.

> **Wichtige Grenze:** Student Müller ist keine Rechtsanwaltskanzlei, übernimmt keine Vertretung und erteilt keine verbindliche Rechtsauskunft. KI-Ausgaben können unvollständig, fehlerhaft oder veraltet sein. Tatsachen, Rechtsgrundlagen, Fristen und Formvorschriften müssen vor einer Verwendung anhand aktueller, verlässlicher Quellen geprüft werden.

## Student Müller ausprobieren

1. [ChatGPT öffnen](https://chatgpt.com/).
2. Die vollständige [Systemanweisung](SYSTEMANWEISUNG.md) öffnen und in einen neuen Chat kopieren.
3. Zunächst eine einfache, nicht vertrauliche Testfrage stellen.
4. Bei einem Dokumentenfall zunächst nur mit dem vollständig fiktiven [Übungsfall Küchen-Erstausstattung](docs/BEISPIELFALL_KUECHENERSTAUSSTATTUNG.md) testen.
5. Ergebnisse mit den Fallunterlagen und den dort angegebenen Prüfpunkten vergleichen.

Der Beispielordner enthält einen fiktiven Antrag, eine Vermieterbestätigung, einen Ablehnungsbescheid, Testanfragen und eine Vergleichsvorlage. Für diesen Test sind weder echte Dokumente noch Screenshots oder Bild-Uploads erforderlich. Der Übungsfall ist keine Vorlage zur ungeprüften Übertragung auf reale Fälle; Rechtslage, Tatsachen und Fristen sind im konkreten Fall gesondert zu prüfen.

**Datenschutz:** Gib keine unredigierten Bescheide, Gutachten, Gesundheitsdaten, Namen, Anschriften, Geburtsdaten, Aktenzeichen, Kontodaten, Zugangsdaten oder sonstige vertrauliche Angaben in einen externen KI-Dienst ein. Beachte die Nutzungs- und Datenschutzbedingungen der jeweils verwendeten Plattform.

## Fachlicher Umfang

| Themenfeld | Beispiele |
|---|---|
| Grundsicherung und Sozialhilfe | SGB II, SGB XII, Unterkunft, Mehrbedarf, Erstausstattung |
| Kranken- und Pflegeversicherung | SGB V und SGB XI |
| Rehabilitation und Teilhabe | SGB IX, Schwerbehindertenrecht, GdB |
| Rente und Erwerbsminderung | Anspruchsvoraussetzungen, Verfahren, Nachweise |
| Verwaltungsverfahren | Bescheidverständnis, Akteneinsicht, Fristen, Rechtsbehelfe |
| Eigene Korrespondenz | Strukturierte Entwürfe für Anträge, Widersprüche und Stellungnahmen |

Der Assistent soll Tatsachen, Dokumenteninhalt, Annahmen und rechtliche Einordnung voneinander trennen, Quellen sichtbar machen, Unsicherheiten benennen und fehlende Angaben gezielt erfragen. Er versendet keine Schreiben und vertritt keine Nutzer gegenüber Behörden oder Gerichten.

## Projektgrenze: Anonymisator

Die lokale Android-Dokumentenverarbeitung ist ein eigenständiges Schwesterprojekt: **[Anonymisator – separates Repository](https://github.com/samysmurf/Anonymisator)**.

Student Müller enthält keine eigene OCR-Engine, PDF-Schwärzungsfunktion, Metadatenbereinigung oder lokale Anonymisierungsfunktion. Es besteht keine gemeinsame Laufzeit, keine direkte KI-Schnittstelle und keine automatische Datenübertragung zwischen den Projekten. Student Müller setzt weder die Fertigstellung noch die Verfügbarkeit von Anonymisator voraus.

## Status V1.4.0

| Bereich | Stand |
|---|---|
| ChatGPT-basierter fachlicher Prototyp | Grundlagen vorhanden; laufende Weiterentwicklung |
| Quellen- und Dokumentenworkflow | als Arbeitsweise beschrieben; Qualität je Funktion zu testen |
| Bescheidverständnis und Schriftsatzentwürfe | Arbeitsabläufe vorhanden; Nutzerprüfung erforderlich |
| Fristenhinweise | Unterstützung bei der Strukturierung; keine Fristgarantie |
| Barrierefreiheit | Entwicklungsziel; keine Konformitätsprüfung behauptet |
| Lokale OCR / Anonymisierung | nicht Bestandteil dieses Repositories; separates Projekt Anonymisator |

Geplante Funktionen werden nicht als implementiert dargestellt. Der jeweilige Stand ist in [Funktionsstatus](docs/FUNKTIONSSTATUS.md) und [Roadmap](ROADMAP.md) dokumentiert.

## Persönliche Nutzung und Verantwortung

Die offizielle Assistentenfassung ist für die eigenständige Bearbeitung der **eigenen persönlichen Angelegenheiten** der jeweils anfragenden Person bestimmt. Sie ist nicht dafür vorgesehen, individuelle fremde Angelegenheiten im Auftrag oder Namen Dritter rechtlich zu prüfen oder Schriftsätze für Dritte zu erstellen.

Allgemeine, nicht auf einen fremden Einzelfall bezogene Informationen zu Gesetzen, Behördenverfahren und öffentlich zugänglichen Rechtsquellen sowie Demonstrationen mit synthetischen Beispieldaten bleiben möglich. Diese projektinterne Zweckbestimmung ist keine gesetzliche Erlaubnis und ersetzt keine gesonderte rechtliche Prüfung des tatsächlichen Angebots und seiner Nutzung.

Nutzer bleiben für Eingaben, Entscheidungen und die Verwendung erzeugter Inhalte verantwortlich. Vor einer Verwendung sind insbesondere Tatsachen, Rechtsgrundlagen, Fristen, Formvorschriften, Anlagen und Versandwege zu prüfen. Die Haftung richtet sich nach geltendem Recht; zwingende gesetzliche Haftung bleibt unberührt. Ein pauschaler Ausschluss sämtlicher Ansprüche wird nicht erklärt.

## Dokumentation und Mitwirkung

- [Systemanweisung](SYSTEMANWEISUNG.md)
- [Projekt-Mindmap als Markdown](mindmap/MINDMAP_V1.4.md)
- [Architektur](docs/ARCHITEKTUR.md) · [Datenschutz](docs/DATENSCHUTZ.md)
- [Funktionsstatus](docs/FUNKTIONSSTATUS.md) · [Roadmap](ROADMAP.md)
- [Barrierefreiheit – @Vision](docs/BARRIEREFREIHEIT.md)
- [Fiktiver Übungsfall](docs/BEISPIELFALL_KUECHENERSTAUSSTATTUNG.md)
- [Mitwirken](CONTRIBUTING.md) · [Sicherheitsmeldungen](SECURITY.md)

## Lizenzen

- Eigener Programmcode: Apache License 2.0.
- Originäre Projekttexte und Dokumentation: CC BY-SA 4.0.
- Fremde Bibliotheken, Datensätze, Marken, amtliche Inhalte und sonstige Drittinhalte bleiben ihren jeweiligen Rechten und Lizenzbedingungen unterworfen.

Die Zuordnung und die vollständigen Lizenzhinweise stehen in [LICENSE](LICENSE). Die persönliche Zweckbestimmung der offiziellen Assistentenfassung ändert die bestehenden Lizenzbedingungen nicht.

**Leitgedanke:** Ein niedrigschwelliges Werkzeug für Verständlichkeit, Selbstbestimmung und gesellschaftliche Teilhabe – mit transparenten Grenzen und überprüfbaren Quellen.

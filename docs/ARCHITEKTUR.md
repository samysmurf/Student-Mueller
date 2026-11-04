# Architektur – Student Müller

**Status: ChatGPT-basierter Informations- und Selbsthilfeassistent; keine eigene Android-App und keine lokale Dokumentenverarbeitungsengine.**

## Systemgrenze

Student Müller wird über ChatGPT bzw. die jeweils genutzte externe KI-Plattform verwendet. Dieses Repository stellt dafür die Systemanweisung, fachliche Arbeitsregeln, Beispieldokumente, Testfälle und Entwicklungsdokumentation bereit. Die eigentliche Verarbeitung von Eingaben und die Erzeugung von Antworten erfolgen innerhalb der externen Plattform und unterliegen deren technischen Eigenschaften sowie Nutzungs- und Datenschutzbedingungen.

## Fachlicher Ablauf

1. **Anliegen klären:** Thema, Ziel und gewünschte Unterstützung erkennen; bei fehlenden entscheidenden Angaben gezielt nachfragen.
2. **Sachverhalt strukturieren:** Nutzerangaben, Dokumenteninhalt, Tatsachen, Annahmen und offene Punkte trennen.
3. **Quellen prüfen:** geltende Rechtsnormen, zeitliche Geltung, amtliche Informationen und überprüfbare Rechtsprechung heranziehen.
4. **Einordnung erstellen:** Anspruchsvoraussetzungen, Unsicherheiten, Fristenrisiken und mögliche Handlungswege verständlich darstellen.
5. **Entwurf erstellen:** Auf Wunsch einen Schriftsatz oder eine andere Behördenkorrespondenz als prüfbaren Entwurf formulieren.
6. **Nutzerprüfung:** Nutzer kontrolliert Tatsachen, Rechtsgrundlagen, Fristen, Anlagen, Formvorschriften und Versandweg selbst.

## Technische Abgrenzung

Nicht Bestandteil von Student Müller sind:

- Android-App oder lokale Android-Shell,
- Termux- und Tesseract-Integration,
- lokale OCR und PDF-Seitenvorverarbeitung,
- Erkennung sensibler Daten auf dem Gerät,
- dauerhafte PDF-Schwärzung und Metadatenbereinigung,
- lokaler Dokumentenexport.

Diese technische Entwicklung liegt ausschließlich im separaten Repository [Anonymisator](https://github.com/samysmurf/Anonymisator). Zwischen beiden Projekten bestehen keine gemeinsame Laufzeit, keine direkte KI-Schnittstelle und keine automatische Datenübertragung. Student Müller setzt Anonymisator nicht voraus.

## Qualitätsprinzipien

Quellen und Aktualität prüfen; Unsicherheiten sichtbar machen; keine Tatsachen oder Rechtsgrundlagen erfinden; keine verbindliche Rechtsprüfung oder Vertretung behaupten; geplante Funktionen nicht als implementiert darstellen. Der Nutzer behält die Kontrolle und Verantwortung für die Verwendung der Ergebnisse.

## Plattformabhängigkeit

Das Projekt kann weder eine lokale Verarbeitung noch Offline-Fähigkeit oder plattformunabhängige Vertraulichkeit garantieren. Verfügbarkeit, Datenverarbeitung, Uploadmöglichkeiten und Nutzungsbedingungen richten sich nach dem jeweils verwendeten externen Dienst.

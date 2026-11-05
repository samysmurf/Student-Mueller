# Architektur – Student Müller

**Version:** V1.5.0 · **Stand:** 05.11.2026

## Systemgrenze

Student Müller ist ein veröffentlichter Systemprompt. Nutzer übernehmen ihn selbstständig in ChatGPT oder einen anderen KI-Dienst ihrer Wahl. Das Repository stellt Systemanweisung, fachliche Arbeitsregeln, Beispieldokumente, Testfälle und Entwicklungsdokumentation bereit.

Die eigentliche Verarbeitung der Eingaben und die Erzeugung von Antworten erfolgen innerhalb der jeweils genutzten externen Plattform. Verfügbarkeit, Modellverhalten, Recherche, Dateiverarbeitung, Datenverarbeitung und Darstellung richten sich nach deren technischen Eigenschaften und Bedingungen.

Der Projektentwickler betreibt keinen eigenen Chatbot-Server, keine eigene Fallannahme und keine Fallbearbeitungsplattform.

## Fachlicher Ablauf

1. **Erststart:** Startmenü mit Bundesland, Thema und Nutzungskontext.
2. **Anliegen klären:** Ziel und gewünschte Unterstützung erkennen; bei fehlenden entscheidenden Angaben gezielt nachfragen.
3. **Rechtsraum bestimmen:** Bundesrecht und das einschlägige Landesrecht trennen; die Region nicht aus Standortdaten erraten.
4. **Sachverhalt strukturieren:** Nutzerangaben, Dokumenteninhalt, Tatsachen, Annahmen und offene Punkte trennen.
5. **Quellen prüfen:** geltende Rechtsnormen, zeitliche Geltung, amtliche Informationen und überprüfbare Rechtsprechung heranziehen.
6. **Zweistufig einordnen:** verständliche Erklärung und präzise rechtliche Analyse liefern.
7. **Entwurf erstellen:** Auf Wunsch einen Schriftsatz oder eine andere Behördenkorrespondenz als prüfbaren Entwurf formulieren.
8. **Nutzerprüfung:** Nutzer kontrolliert Tatsachen, Rechtsgrundlagen, Fristen, Anlagen, Formvorschriften und Versandweg selbst.

## Technische Abgrenzung

Nicht Bestandteil von Student Müller sind:

- Android-App oder lokale Android-Shell,
- Termux- und Tesseract-Integration,
- lokale OCR und PDF-Seitenvorverarbeitung,
- Erkennung sensibler Daten auf dem Gerät,
- dauerhafte PDF-Schwärzung und Metadatenbereinigung,
- lokaler Dokumentenexport,
- automatischer Versand von Schreiben.

Diese technische Entwicklung liegt ausschließlich im separaten Repository [Anonymisator](https://github.com/samysmurf/Anonymisator). Zwischen beiden Projekten bestehen keine gemeinsame Laufzeit, keine direkte KI-Schnittstelle und keine automatische Datenübertragung. Student Müller setzt Anonymisator nicht voraus.

## Qualitätsprinzipien

Quellen und Aktualität prüfen; Unsicherheiten sichtbar machen; keine Tatsachen oder Rechtsgrundlagen erfinden; keine verbindliche Rechtsprüfung oder Vertretung behaupten; geplante Funktionen nicht als implementiert darstellen. Der Nutzer behält die Kontrolle über die Verwendung der Ergebnisse.

## Plattformabhängigkeit

Das Projekt kann weder lokale Verarbeitung noch Offline-Fähigkeit oder plattformunabhängige Vertraulichkeit garantieren. Die tatsächliche Befolgung der Systemanweisung kann je nach KI-Dienst und Modell variieren. Das Startmenü ist im Prompt festgelegt; seine konkrete grafische Darstellung ist keine vom Repository garantierte UI-Funktion.

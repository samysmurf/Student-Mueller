# Skill-Testplan – Student Müller Skills-only-Plugin

**Plugin-Paket:** 0.1.0  
**Fachliche Core-Basis:** V1.5.1, Stand 05.11.2026  
**Status:** Testfälle definiert; Laufzeittests nach der letzten V-A09-Ausgabekontrolländerung noch nicht durchgeführt

## 1. Testziel und Abgrenzung

Geprüft wird die Überführung des bestehenden Student-Müller-Prompts in ein Skills-only-Plugin. Unterschieden werden statische Paketprüfung, Skill-Aktivierung, fachliche Regression und tatsächliche Plattform-Laufzeittests.

Die 21 Prüffälle aus `docs/TESTPROTOKOLL_V1.5.md` bleiben die Core-Regressionsbasis. Sie sind keine Plugin-Laufzeittests. Die V1.5.1-Änderungen und der V-A09-Test werden zusätzlich geprüft.

## 2. Skill-Aktivierung

| ID | Eingabeart | Testidee | Erwartetes Verhalten |
|---|---|---|---|
| SK-A01 | Direkte Aktivierung | „Erkläre mir meinen Bürgergeld-Bescheid.“ | Skill wird aktiviert und wendet die vollständige Core-Referenz an. |
| SK-A02 | Indirekte Aktivierung | „Das Jobcenter hat meine Miete nicht vollständig berücksichtigt.“ | Sozialrechtlicher Kontext wird erkannt; entscheidende Angaben werden schrittweise geklärt. |
| SK-A03 | Betreuungsrecht | „Welche Aufgaben darf mein Betreuer übernehmen?“ | Skill wird aktiviert; Bundesrecht und Landesrecht werden getrennt. |
| SK-A04 | Schriftsatz | „Hilf mir, einen Widerspruch zu formulieren.“ | Skill wird aktiviert; Bescheid, Zugang und Frist werden vor einem Entwurf geklärt. |
| SK-A05 | Unvollständige Angaben | „Ich habe einen Bescheid bekommen.“ | Keine voreilige Rechtsbewertung; gezielte Rückfrage. |
| SK-A06 | Bereits bekannter Kontext | Bundesland und Thema wurden zuvor im Gespräch genannt. | Bekannte Angaben nicht erneut abfragen. |
| SK-A07 | Nicht einschlägige Anfrage | „Schreibe ein Gedicht über den Herbst.“ | Skill soll nicht unnötig aktiviert werden. |
| SK-A08 | Nichtdeutscher Rechtsraum | Allgemeine Frage zu einem ausländischen Rechtssystem. | Deutsches Recht nicht unterstellen; Anwendungsbereich klären. |

## 3. § 40 SGB II – verbindlicher V-A09-Regressionstest

| ID | Test | Erwartetes Verhalten |
|---|---|---|
| V-A09-01 | Widerspruch gegen eine Erklärung zu § 44 SGB X / § 40 SGB II | Vierjahres-, Einjahres- und Absatz-3-Regelungen getrennt darstellen; keine Verkürzung auf eine einzige Frist. |
| V-A09-02 | § 40 Abs. 3 Satz 1 SGB II | Eigenständige Prüfung und Erklärung der gesetzlichen Voraussetzungen und Rechtsfolge. |
| V-A09-03 | § 40 Abs. 3 Satz 2 SGB II | Eigenständige Prüfung der besonderen zeitlichen Regelung; nicht mit Satz 1 oder der Einjahresregel gleichsetzen. |
| V-A09-04 | Sachverhalt ohne erkennbare Anhaltspunkte für Abs. 3 | Fehlende Anhaltspunkte ausdrücklich feststellen, ohne die Norm nur pauschal zu erwähnen. |
| V-A09-05 | Sachverhalt mit möglicher Relevanz des Abs. 3 | Tatsachenlücken gezielt abfragen und beide Sätze getrennt prüfen. |
| V-A09-06 | Ausgabe-Abschlusskontrolle | Vor Abschluss kontrollieren, ob Abs. 3, Satz 1 und Satz 2 ausdrücklich geprüft und im Ergebnis nachvollziehbar dargestellt wurden. Fehlt ein erforderlicher Teil, Antwort vor Ausgabe ergänzen. |

**Freigabesperre:** V-A09 gilt erst dann als bestanden, wenn alle ausdrücklich geforderten Teile in der tatsächlichen Antwort vorhanden sind. Eine bloße Anweisung zur Selbstkontrolle oder ein pauschaler Hinweis „gegebenenfalls zu beachten“ reicht nicht. Die zuletzt freigegebene Ausgabekontrolländerung muss in einem frischen Chat mit einer realen ChatGPT-Ausführung geprüft werden. Bis dahin bleibt der Teststatus offen.

## 4. Weitere Core-Regression

Zusätzlich sind alle 21 Prüffälle aus `docs/TESTPROTOKOLL_V1.5.md` zu wiederholen. Die erwarteten Ergebnisse und bisherigen Einschränkungen bleiben dort dokumentiert.

Die V1.5.1-Barrierefreiheitsregeln sind anhand von `docs/BARRIEREFREIHEIT.md` und den dort definierten Prüffällen in einer unterstützten ChatGPT-Oberfläche zu testen. Keine Screenreader-, Smartphone- oder Plattformkonformität behaupten, bevor diese tatsächlich geprüft wurde.

## 5. Statische Paketprüfung

| ID | Prüfkriterium | Sollzustand |
|---|---|---|
| PK-01 | Root-Manifest | Gültige portable `plugin.json` am Plugin-Root. |
| PK-02 | Plugin-ID | Stabiler Kebab-Case-Name `student-mueller`. |
| PK-03 | Skill-Pfad | `skills/student-mueller/SKILL.md` direkt unter `skills/`. |
| PK-04 | Skill-Frontmatter | YAML mit nichtleerem `name` und `description`. |
| PK-05 | Referenz | Vollständige Core-Referenz liegt unter `references/`. |
| PK-06 | Quellgleichheit | Referenz ist textgleich mit der freigegebenen Core-Datei V1.5.1. |
| PK-07 | MCP-Abwesenheit | Keine MCP-Datei, App-Referenz, Serverabhängigkeit oder Zugangsdaten. |
| PK-08 | Branding | Quadratische SVG-Logo- und Composer-Icon-Dateien vorhanden, valide und im Manifest referenziert. |
| PK-09 | Lizenz | CC BY-SA 4.0 und Herkunftshinweis nachvollziehbar. |
| PK-10 | ZIP-Root | ZIP enthält die Plugin-Wurzel und keine Geschwisterdateien oder das gesamte Repository. |

## 6. Laufzeitprotokoll

Für jeden tatsächlichen ChatGPT-Test dokumentieren:
- Datum und Uhrzeit;
- ChatGPT-Oberfläche und verfügbares Modell;
- installierte Plugin-Paketversion;
- vollständige Testeingabe;
- beobachtete Skill-Aktivierung;
- relevante Ausgabe bzw. anonymisierter Auszug;
- Soll-Ist-Abweichung;
- Bewertung: bestanden, eingeschränkt bestanden oder nicht bestanden.

Nur synthetische oder wirksam anonymisierte Testdaten verwenden. Keine echten personenbezogenen Bescheide oder Gesundheitsdaten in öffentliche Testdateien übernehmen.

## 7. Freigabekriterien

Eine öffentliche Einreichung wird erst vorbereitet, wenn:
1. alle statischen Paketprüfungen bestanden sind;
2. Aktivierung und Nicht-Aktivierung in ChatGPT geprüft wurden;
3. alle 21 Core-Regressionsfälle erneut bewertet wurden;
4. V-A09 nach der letzten genehmigten Ausgabekontrolländerung in einem frischen Chat bestanden ist;
5. Barrierefreiheitsprüfungen entsprechend dem tatsächlichen Testumfang dokumentiert sind;
6. Core-Referenz und Plugin-Skill synchron sind;
7. Branding-Assets und finale Listing-Angaben vorliegen;
8. Nutzungsbedingungen, Datenschutz und Lizenzhinweise mit dem tatsächlichen Funktionsumfang übereinstimmen.

Ein bestandener statischer Test ist keine unabhängige juristische Freigabe und kein Beleg für fehlerfreie Antworten in allen Einzelfällen.

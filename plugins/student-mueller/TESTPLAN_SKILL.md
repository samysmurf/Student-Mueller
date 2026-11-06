# Skill-Testplan – Student Müller Skills-only-Plugin

**Plugin-Paket:** 0.1.0  
**Fachliche Core-Basis:** V1.5.0, Stand 05.11.2026  
**Status:** Testfälle definiert; Laufzeittests noch nicht durchgeführt

## 1. Testziel und Abgrenzung

Dieses Testplan-Dokument prüft die Überführung des bestehenden Student-Müller-Prompts in ein Skills-only-Plugin. Es unterscheidet:

- **statische Paketprüfung:** Manifest, Verzeichnisstruktur, UTF-8, YAML-Frontmatter und Referenzdateien;
- **Skill-Aktivierung:** richtige, indirekte, unvollständige und nicht einschlägige Anfragen;
- **fachliche Regression:** die 21 bereits im Core-Testprotokoll dokumentierten Prüffälle;
- **Plattform-Laufzeittest:** tatsächliche Ausführung des installierten Skills in ChatGPT.

Die 21 Core-Prüffälle aus `docs/TESTPROTOKOLL_V1.5.md` sind keine Plugin-Laufzeittests und werden nicht als solche umetikettiert.

## 2. Skill-Aktivierung

| ID | Eingabeart | Beispiel / Testidee | Erwartetes Verhalten |
|---|---|---|---|
| SK-A01 | Direkte Aktivierung | „Erkläre mir meinen Bürgergeld-Bescheid.“ | Skill wird aktiviert und wendet die Core-Systemanweisung an. |
| SK-A02 | Indirekte Aktivierung | „Das Jobcenter hat meine Miete nicht vollständig berücksichtigt.“ | Sozialrechtlicher Kontext wird erkannt; relevante Angaben werden schrittweise geklärt. |
| SK-A03 | Betreuungsrecht | „Welche Aufgaben darf mein Betreuer übernehmen?“ | Skill wird aktiviert; Bundesrecht und gegebenenfalls Landesrecht werden getrennt. |
| SK-A04 | Schriftsatz | „Hilf mir, einen Widerspruch zu formulieren.“ | Skill wird aktiviert; Frist und Bescheidangaben werden vor einem Entwurf geklärt. |
| SK-A05 | Unvollständige Angaben | „Ich habe einen Bescheid bekommen.“ | Keine voreilige Rechtsbewertung; eine gezielte Rückfrage nach Anliegen bzw. Bescheidart. |
| SK-A06 | Bereits bekannter Kontext | Bundesland und Thema wurden zuvor im Gespräch genannt. | Angaben nicht erneut abfragen; vorhandenen Kontext verwenden. |
| SK-A07 | Nicht einschlägige Anfrage | „Schreibe ein Gedicht über den Herbst.“ | Skill soll nicht unnötig aktiviert werden. |
| SK-A08 | Grenzfall | Allgemeine Frage zu einem nicht-deutschen Rechtssystem. | Nicht deutsches Recht unterstellen; Anwendungsbereich klären oder auf den deutschen Scope begrenzen. |

## 3. Fachliche Regression

Die folgenden Fälle müssen gegen die vollständige Core-Testreihe geprüft werden. Maßgeblich sind Eingabe, erwartetes Verhalten und Bewertungsgrenzen in `docs/TESTPROTOKOLL_V1.5.md`.

1. Erststart ohne Bundesland
2. Auswahl NRW
3. Wechsel NRW zu Bayern
4. Betreuung ohne Einwilligungsvorbehalt
5. Begrenzter Aufgabenkreis
6. Betreuerwunsch der betroffenen Person
7. Konkrete Pflichtverletzung des Betreuers
8. Betreuerwechsel
9. Ärztliche Zwangsmaßnahme
10. PsychKG-Unterbringung gegenüber BGB-Unterbringung
11. Ende der Betreuung ab 2026
12. Wahlrecht bei Betreuung
13. Sozialleistungsbescheid aus 2025
14. Sozialleistungsbescheid ab Juli 2026
15. Fehlerhafte oder fehlende Rechtsbehelfsbelehrung
16. Unterstützung eines Angehörigen
17. Unentgeltliche Hilfe für eine andere Person
18. Noch nicht verabschiedeter Gesetzentwurf
19. Widersprüchliche Dokumente
20. Unklarer Fristbeginn oder fehlender Zugangsnachweis
21. Primärquelle nicht erreichbar

## 4. Paketprüfung

| ID | Prüfkriterium | Sollzustand |
|---|---|---|
| PK-01 | Root-Manifest | Genau eine gültige `plugin.json` am Plugin-Root. |
| PK-02 | Plugin-ID | Stabiler Kebab-Case-Name `student-mueller`. |
| PK-03 | Skill-Pfad | `skills/student-mueller/SKILL.md` direkt unter `skills/`. |
| PK-04 | Skill-Frontmatter | YAML-Frontmatter mit nichtleerem `name` und `description`. |
| PK-05 | Referenz | Vollständige Core-Referenz liegt im Skill-Unterordner `references/`. |
| PK-06 | Quellgleichheit | Referenzdatei ist byte-/textgleich mit der freigegebenen Core-Datei zum dokumentierten Stand. |
| PK-07 | MCP-Abwesenheit | Keine `mcp.json`, `.mcp.json`, `.app.json`, Serverabhängigkeit oder Zugangsdaten. |
| PK-08 | Branding | Quadratische Logo- und Composer-Icon-Dateien werden vor öffentlicher Einreichung ergänzt. |
| PK-09 | Lizenz | CC BY-SA 4.0 und Herkunftshinweis bleiben nachvollziehbar. |
| PK-10 | ZIP-Root | ZIP enthält nur die Plugin-Wurzel, keine Geschwisterdateien und nicht das gesamte Repository. |

## 5. Laufzeitprotokoll

Für jeden tatsächlichen ChatGPT-Test werden mindestens dokumentiert:

- Datum und Uhrzeit;
- ChatGPT-Oberfläche und verfügbares Modell;
- installierte Plugin-Paketversion;
- vollständige Testeingabe;
- beobachtete Skill-Aktivierung;
- relevante Ausgabe bzw. anonymisierter Auszug;
- Soll-Ist-Abweichung;
- Bewertung: bestanden, eingeschränkt bestanden oder nicht bestanden.

Keine echten personenbezogenen Bescheide oder Gesundheitsdaten in öffentliche Testdateien übernehmen. Für Tests ausschließlich synthetische oder wirksam anonymisierte Daten verwenden.

## 6. Freigabekriterien

Eine öffentliche Einreichung wird erst vorbereitet, wenn:

1. alle statischen Paketprüfungen bestanden sind;
2. Skill-Aktivierung und Nicht-Aktivierung in einer unterstützten ChatGPT-Umgebung geprüft wurden;
3. die fachliche Regression dokumentiert ist;
4. Core- und Skill-Referenz nachweislich synchron sind;
5. Branding-Assets und finale Listing-Angaben vorliegen;
6. Nutzungsbedingungen, Datenschutzinformation und Lizenzhinweise mit dem tatsächlichen Funktionsumfang übereinstimmen.

Ein definierter Testfall oder ein bestandenes statisches Prüfkriterium ist kein Beleg für eine unabhängige juristische Freigabe oder für fehlerfreie Antworten in allen Einzelfällen.

# Testprotokoll V1.5.0 – Student Müller

**Stand:** 05.11.2026  
**Prüfumfang:** 21 manuelle Regel- und Konsistenztests  
**Prüfart:** statische Prüfung der Systemanweisung und manuelle gedankliche Durchspielung der definierten Eingabe-/Ausgabefälle  
**Nicht durchgeführt:** automatisierte Tests, echte ChatGPT-Laufzeittests, mobile UI-Tests, externe Modellvergleiche

## 1. Bedeutung der Teststatus

- **Bestanden (Prompt-Logik):** Die Systemanweisung enthält eine hinreichend klare Regel, die das erwartete Verhalten vorgibt, und die Prüfung ergab keinen inneren Widerspruch.
- **Mit Einschränkung bestanden:** Die Regel ist enthalten, aber die tatsächliche Ausführung hängt von einer externen Plattform, einer konkreten Quelle oder noch fehlenden Sachverhaltsangaben ab.
- **Nicht als Live-Test geprüft:** Es wurde keine echte Unterhaltung mit dem Prompt auf einer Zielplattform durchgeführt.

Die Einstufung „Bestanden“ bedeutet daher ausdrücklich nicht, dass ein KI-Modell die Regel in jeder Antwort zuverlässig befolgt. Sie ist kein unabhängiger juristischer Audit und keine Rechtsfreigabe.

## 2. Die 21 Prüffälle

| Nr. | Testfall | Erwartetes Verhalten | Ergebnis der Prompt-Prüfung |
|---:|---|---|---|
| 1 | Erststart ohne Bundesland | Startmenü erscheint zuerst und fragt Bundesland, Thema und Nutzungskontext ab. | **Bestanden – Prompt-Logik.** Startregel ist in Abschnitt 3 verbindlich. Live-Darstellung nicht geprüft. |
| 2 | Auswahl NRW | NRW wird als Arbeitskontext gespeichert; bei PsychKG-Fragen wird amtliches NRW-Landesrecht geprüft. | **Bestanden – mit Quellenvorbehalt.** Landesrechtliche Regel und amtliches Rechtsportal sind vorgegeben. |
| 3 | Wechsel NRW zu Bayern | Der Rechtsraum wird für die neue Angelegenheit umgestellt; NRW-Regeln werden nicht ungeprüft weiterverwendet. | **Bestanden – Prompt-Logik.** Wechsel und Mehrländerfälle sind ausdrücklich geregelt. |
| 4 | Betreuung ohne Einwilligungsvorbehalt | Keine automatische Geschäftsunfähigkeit oder Zustimmungspflicht annehmen; §§ 104 BGB und 1825 BGB getrennt prüfen. | **Bestanden – Prompt-Logik.** Die Rechtsinstitute sind ausdrücklich voneinander abgegrenzt. |
| 5 | Begrenzter Aufgabenkreis | Vertretungsmacht nur innerhalb des gerichtlich angeordneten Aufgabenbereichs prüfen; Sonderbefugnisse nur bei ausdrücklicher Anordnung. | **Bestanden – Prompt-Logik.** §§ 1815 und 1823 BGB sind als Prüfgrundlage enthalten. |
| 6 | Betreuerwunsch der betroffenen Person | Wunsch und Eignung nach § 1816 BGB berücksichtigen; Ablehnung nicht ignorieren. | **Bestanden – Prompt-Logik.** Wünsche und Auswahlkriterien sind ausdrücklich genannt. |
| 7 | Konkrete Pflichtverletzung des Betreuers | Gerichtliche Aufsicht nach § 1862 BGB und mögliche Berichts-/Rechnungsprüfungen prüfen; nicht nur auf Unzufriedenheit abstellen. | **Bestanden – Prompt-Logik.** Aufsicht und Berichtspflichten sind abgebildet. |
| 8 | Betreuerwechsel | § 1868 BGB und § 296 FamFG prüfen; Wünsche, Eignung, wichtiger Grund und Alternativen unterscheiden. | **Bestanden – Prompt-Logik.** Wechsel, Entlassung und Neubestellung sind gesondert geregelt. |
| 9 | Ärztliche Zwangsmaßnahme | § 1832 BGB, BVerfG 1 BvL 1/24, gerichtliche Genehmigung und § 312 Nr. 3 FamFG prüfen; Gesetzesänderung nur bei Verkündung und Inkrafttreten anwenden. | **Bestanden – mit Aktualitätsvorbehalt.** Die Systemregel ist korrekt differenziert; vor jedem realen Fall muss der Gesetzgebungsstand erneut geprüft werden. |
| 10 | PsychKG-Unterbringung gegenüber BGB-Unterbringung | Landes-PsychKG und § 1831 BGB nicht vermischen; zuständiges Landesrecht und FamFG-Verfahren bestimmen. | **Bestanden – mit Landesrechtsvorbehalt.** Trennung ist ausdrücklich vorgegeben; jede Landesfassung muss konkret abgerufen werden. |
| 11 | Ende der Betreuung ab 2026 | §§ 1872 bis 1874 BGB unterscheiden; Herausgabe, Vermögensübersicht, Schlussrechnung bei Betreuerwechsel und Schlussmitteilung nicht vermengen. | **Bestanden – Prompt-Logik.** Die seit 01.01.2026 geltenden Regelungen sind berücksichtigt. |
| 12 | Wahlrecht bei Betreuung | Betreuung allein nicht als Wahlrechtsausschluss behandeln; § 13 BWahlG und bei Landes-/Kommunalwahlen das Landeswahlrecht prüfen. | **Bestanden – Prompt-Logik.** Bundes- und Landeswahlrecht sind ausdrücklich getrennt. |
| 13 | Sozialleistungsbescheid aus 2025 | Historische Gesetzesfassung für den Leistungszeitraum und damaligen Bescheid prüfen; keine rückwirkende Anwendung des neuen Rechts. | **Bestanden – Prompt-Logik.** Rechtsstand und historische Gesetzesfassung sind verbindlicher Prüfstandard. |
| 14 | Sozialleistungsbescheid ab Juli 2026 | Neue SGB-II-Regelungen und gestaffelte Inkrafttretensdaten anwenden; § 65a SGB II berücksichtigen. | **Bestanden – mit Aktualitätsvorbehalt.** Übergangsregel ist ausdrücklich genannt; Normfassung ist im konkreten Fall erneut abzurufen. |
| 15 | Fehlerhafte oder fehlende Rechtsbehelfsbelehrung | § 66 SGG beziehungsweise einschlägige Verfahrensnorm prüfen; Frist nicht schematisch berechnen. | **Bestanden – Prompt-Logik.** Sonderregeln und Fristauslöser sind Teil des Prüfablaufs. |
| 16 | Unterstützung eines Angehörigen | Beziehung, Rolle, Vollmacht und tatsächliche Tätigkeit nur soweit erforderlich klären; private Unterstützung nicht pauschal verbieten. | **Bestanden – Prompt-Logik.** Drittunterstützung ist zugelassen, aber rechtlich zu prüfen. |
| 17 | Unentgeltliche Hilfe für eine andere Person | Zuerst § 2 RDG, dann § 3 und gegebenenfalls § 6 RDG prüfen; Unentgeltlichkeit nicht als automatische Freistellung behandeln. | **Bestanden – Prompt-Logik.** Reihenfolge und Differenzierung sind enthalten. |
| 18 | Noch nicht verabschiedeter Gesetzentwurf | Entwurf als Entwurf kennzeichnen; nicht als geltendes Recht anwenden. | **Bestanden – Prompt-Logik.** Status und Inkrafttreten müssen ausdrücklich unterschieden werden. |
| 19 | Widersprüchliche Dokumente | Widerspruch kenntlich machen, Quellen und Belege gegenüberstellen, keine fehlende Tatsache erfinden. | **Bestanden – Prompt-Logik.** Trennung von Dokumenteninhalt, Angaben und Annahmen ist verbindlich. |
| 20 | Unklarer Fristbeginn oder fehlender Zugangsnachweis | Fehlende Informationen benennen; keine scheinbar sichere Frist errechnen; rechtzeitige fristwahrende Handlung erwägen. | **Bestanden – Prompt-Logik.** Die Fristberechnung ist an ausreichende Tatsachen gebunden. |
| 21 | Primärquelle nicht erreichbar | Keine Aktualitätsprüfung vortäuschen; bekannte Informationen, offene Verifikation und fehlende Quelle klar kennzeichnen. | **Bestanden – Prompt-Logik.** Quellen- und Unsicherheitsregeln decken diesen Fall ab. |

## 3. Fachliche Gegenkontrolle ausgewählter Normzuordnungen

Die folgenden Zuordnungen wurden anhand amtlicher Gesetzestexte und amtlicher Informationen gegengeprüft:

- § 1815 BGB verlangt ausdrücklich angeordnete Aufgabenbereiche für die in Absatz 2 aufgezählten Sonderbefugnisse.
- §§ 1872 und 1873 BGB unterscheiden Herausgabe, Vermögensübersicht, Schlussrechnung beim Betreuerwechsel und Schlussmitteilung.
- § 317 FamFG sieht bei Genehmigung einer Einwilligung in eine ärztliche Zwangsmaßnahme oder deren Anordnung stets einen Verfahrenspfleger vor.
- § 312 Nr. 3 FamFG ordnet ärztliche Zwangsmaßnahmen nach § 1832 BGB den Unterbringungssachen zu; § 298 FamFG betrifft dagegen Fälle des § 1829 BGB.
- § 8 BtOG behandelt Beratung, Unterstützung, Vermittlung geeigneter Hilfen und erweiterte Unterstützung.
- § 65a Abs. 4 SGB II gestattet bis zum 31.12.2026 die Verwendung des Begriffs „Bürgergeld“ durch Behörden für den Begriff „Grundsicherungsgeld“.
- § 13 BWahlG knüpft den Ausschluss vom Wahlrecht an einen Richterspruch, nicht allein an die Bestellung eines Betreuers.
- § 11 PsychKG NRW verlangt eine gegenwärtige erhebliche Gefährdung und dass diese nicht anders abgewendet werden kann; fehlende Behandlungsbereitschaft allein reicht nicht.

## 4. Quellen für die Gegenkontrolle

- [§ 1814 BGB](https://www.gesetze-im-internet.de/bgb/__1814.html)
- [§ 1815 BGB](https://www.gesetze-im-internet.de/bgb/__1815.html)
- [§ 1832 BGB](https://www.gesetze-im-internet.de/bgb/__1832.html)
- [§ 1872 BGB](https://www.gesetze-im-internet.de/bgb/__1872.html)
- [§ 1873 BGB](https://www.gesetze-im-internet.de/bgb/__1873.html)
- [§ 317 FamFG](https://www.gesetze-im-internet.de/famfg/__317.html)
- [§ 312 FamFG](https://www.gesetze-im-internet.de/famfg/__312.html)
- [BtOG](https://www.gesetze-im-internet.de/btog/)
- [§ 65a SGB II](https://www.gesetze-im-internet.de/sgb_2/__65a.html)
- [§ 13 BWahlG](https://www.gesetze-im-internet.de/bwahlg/__13.html)
- [PsychKG NRW, amtliche Fassung](https://recht.nrw.de/lrgv/gesetz/01072025-gesetz-ueber-hilfen-und-schutzmassnahmen-bei-psychischen-krankheiten-psychkg/)
- [BVerfG, Urteil vom 26.11.2024 – 1 BvL 1/24](https://www.bundesverfassungsgericht.de/SharedDocs/Entscheidungen/DE/2024/11/ls20241126_1bvl000124.html)

## 5. Gesamtbewertung

**Ergebnis der manuellen Prompt-Prüfung:** 21 von 21 Prüffällen sind auf Regel- und Konsistenzebene bestanden.

**Nicht nachgewiesen:** tatsächliche Laufzeitzuverlässigkeit in ChatGPT oder anderen KI-Diensten, korrekte grafische Startmenü-Darstellung, zuverlässiger Zugriff auf aktuelle Primärquellen und vollständige juristische Richtigkeit jeder denkbaren Einzelfallantwort.

Vor einer öffentlichen Freigabe als „abschließend getestet“ müssen reale Plattformtests durchgeführt und mit Datum, Plattform, Modell, Eingabe, Ausgabe und Bewertung dokumentiert werden.

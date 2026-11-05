# Testprotokoll Barrierefreiheit V1.5.1 – Student Müller

**Stand:** 05.11.2026  
**Status:** Prüfkatalog vorbereitet; tatsächliche Tests noch nicht durchgeführt.  
**Prüfgegenstand:** barrierearme Antwort- und Dialogregeln der Systemanweisung sowie deren Ausgabe auf konkreten KI-Plattformen.

## 1. Teststatus und Grenzen

Die folgenden Testfälle definieren, was vor einer Aussage über die praktische Zugänglichkeit geprüft werden soll. Sie sind keine bestandenen Tests.

Bisher erfolgte eine statische Prüfung der Systemanweisung und der zugehörigen Dokumentation. Nicht durchgeführt wurden:
- Tests in einer realen ChatGPT- oder anderen KI-Sitzung,
- Tests mit Android TalkBack oder einem Desktop-Screenreader,
- Tests mit Textvergrößerung oder hohem Kontrast,
- Tests mit Menschen mit unterschiedlichen Behinderungen oder Nutzungsvoraussetzungen,
- technische Tests einer eigenen Oberfläche.

Die Systemanweisung steuert die Ausgabeaufforderung, aber nicht die Oberfläche des externen KI-Anbieters. Ein negatives Ergebnis in der Plattformdarstellung ist daher von einem Fehler der Prompt-Regel zu unterscheiden.

## 2. Voraussetzungen für eine reproduzierbare Prüfung

Für jeden tatsächlichen Test sind zu dokumentieren:
- Datum und Uhrzeit,
- KI-Plattform und Modell,
- Gerät, Betriebssystem und Version,
- verwendete Assistenztechnik und deren Einstellungen,
- genaue Testeingabe,
- vollständige tatsächliche Ausgabe,
- beobachtete Barriere oder Abweichung,
- Bewertung: bestanden, teilweise bestanden, nicht bestanden oder nicht prüfbar,
- gegebenenfalls Schritte zur Wiederholung.

Es sind ausschließlich synthetische Testdaten zu verwenden. Keine echten Bescheide oder personenbezogenen Falldaten in öffentliche Testprotokolle übernehmen.

## 3. Testfälle

| ID | Testfall und Eingabeidee | Erwartetes Verhalten | Status |
|---|---|---|---|
| V-A01 | Erststart mit TalkBack durchlaufen | Startmenü wird in sinnvoller Lesereihenfolge ausgegeben; Optionen sind eindeutig unterscheidbar; freie Antwort ist möglich. | **Offen – nicht durchgeführt** |
| V-A02 | Mindmap oder Diagramm anfordern | Die Kernaussagen und Beziehungen werden vollständig in einer strukturierten Textalternative wiedergegeben. | **Offen – nicht durchgeführt** |
| V-A03 | Mehrspaltige Gesetzes-/Vergleichstabelle anfordern | Die Information ist auch linear verständlich; keine wesentliche Bedeutung geht durch Tabellenlayout verloren. | **Offen – nicht durchgeführt** |
| V-A04 | Quellenliste per Screenreader lesen | Linktexte und Quellenbezeichnungen sind ohne visuelle Umgebung eindeutig; die Rechtsquelle ist im Text benannt. | **Offen – nicht durchgeführt** |
| V-A05 | Bescheidprüfung mit zwei Antwortebenen | Verständliche Erklärung und rechtliche Prüfung sind konsistent; Voraussetzungen, Ausnahmen und Unsicherheiten bleiben erhalten. | **Offen – nicht durchgeführt** |
| V-A06 | Ausgabe mit 200-%-Textvergrößerung aufrufen | Kein Informationsverlust oder unzugänglicher Inhalt durch Vergrößerung; plattformabhängige Darstellung wird separat bewertet. | **Offen – nicht durchgeführt** |
| V-A07 | Komplexe Angelegenheit schrittweise klären | Es wird nur die jeweils wichtigste fehlende Angabe gefragt; bereits beantwortete Fragen werden nicht unnötig wiederholt. | **Offen – nicht durchgeführt** |
| V-A08 | Antwort mit Farbcodierung oder Emojis anfordern | Bedeutung bleibt auch ohne Farbe, Emoji oder grafische Hervorhebung vollständig verständlich. | **Offen – nicht durchgeführt** |
| V-A09 | „Bitte einfacher und Schritt für Schritt erklären“ | Sprache wird verständlicher; rechtliche Bedingungen und Vorbehalte bleiben erhalten; vereinfachte Sprache wird nicht fälschlich als zertifizierte Leichte Sprache bezeichnet. | **Offen – nicht durchgeführt** |
| V-A10 | Verlinktes Video oder Audio als Quelle verwenden | Wesentliche Aussagen sind zusätzlich textlich zugänglich; vorhandene Untertitel/Transkripte werden nicht ungeprüft behauptet. | **Offen – nicht durchgeführt** |
| V-A11 | Tastaturbedienung und Fokus in der Plattform testen | Interaktion ist ohne ausschließlich gestenbasierte Bedienung möglich; Fokus bleibt nachvollziehbar. Ergebnis betrifft die Plattform, nicht die Prompt-Regel allein. | **Offen – nicht durchgeführt** |
| V-A12 | Auf einer künftigen eigenen Oberfläche Bedienung mit Touch und Screenreader prüfen | Interaktive Elemente haben zugängliche Namen, ausreichende Ziele, sinnvolle Fokusreihenfolge und funktionieren mit Assistenztechnik. | **Nicht anwendbar – eigene Oberfläche nicht vorhanden** |

## 4. Bewertung und Freigaberegel

Ein Test darf nur dann als bestanden bezeichnet werden, wenn die tatsächliche Ausgabe beziehungsweise Bedienung auf der angegebenen Plattform geprüft wurde. Ein aus der Systemanweisung abgeleitetes erwartetes Verhalten reicht dafür nicht aus.

Ein fehlender oder nicht zugänglicher Plattformmechanismus ist als Plattformgrenze zu dokumentieren. Er darf nicht als bereits behobener Prompt-Fehler dargestellt werden.

Eine Konformitätsaussage nach WCAG 2.2 oder BITV 2.0 setzt eine vollständige Prüfung des jeweils einschlägigen Gegenstands und Anwendungsbereichs voraus. Dieses Testprotokoll ist dafür weder vollständig noch ausreichend.

## 5. Bezugspunkte

- [WCAG 2.2 – W3C Recommendation](https://www.w3.org/TR/WCAG22/)
- [Barrierefreiheit – Entwicklungsleitlinie Student Müller](BARRIEREFREIHEIT.md)
- [Systemanweisung V1.5.1](../SYSTEMANWEISUNG.md)

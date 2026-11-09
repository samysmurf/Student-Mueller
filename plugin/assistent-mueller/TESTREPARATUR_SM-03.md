# SM-03 – Reparaturprotokoll Assistent Mueller 0.1.2

Datum: 08.11.2026
Ausgangspaket: `assistent-mueller.zip` (Plugin-Prototyp 0.1.1, Library-Kopie)
Neuer Stand: 0.1.2

## Ergebnis

Die Nutzerbewertung des simulierten Testfalls SM-03 lautet „passed“. Die nachgelagerte Reparaturprüfung hat jedoch Fehler in der Testführung und Präzisierungsbedarf in den Skills identifiziert. Der Fall war eine Simulation; es wurde kein reales Behördenverfahren geprüft.

## Behobene bzw. abgesicherte Schwachstellen

1. **Historischer Rechtsstand:** Für einen Sachverhalt aus 2025 muss die 2025 geltende Fassung von § 22 SGB II und § 40 SGB II verwendet werden. Die 2026er Rechtslage darf nicht ungeprüft rückübertragen werden.
2. **Sechsmonatsregel:** Die Formulierung „in der Regel jedoch längstens für sechs Monate“ ist keine garantierte Mindestfrist und keine pauschale Karenzzeit. Eine Dreimonatsfrist ist einzelfallbezogen zu beurteilen.
3. **Heizspiegel:** Die Ausgabe 2024 enthält getrennte Tabellen nach Baujahresgruppen. Für Gebäude Baujahr 1995–2001, 251–500 m² Gebäude-Wohnfläche und Erdgas lautet die Kostenkategorie „zu hoch“ ab 23,01 €/m²/Jahr. Andere Baujahresgruppen haben andere Werte. Der Tabellenwert bezieht sich auf Gebäude-Kosten und Gebäude-Fläche, nicht schlicht auf die einzelne Wohnung.
4. **BSG-Methode:** BSG, Urteil vom 28.02.2024 – B 4 AS 18/22 R, Rn. 23: maßgeblich sind die rechte Spalte des Heizspiegels und die abstrakt angemessene Wohnfläche des Haushalts; der Wert ist keine starre Höchstgrenze. Eine konkrete Einzelfallprüfung bleibt erforderlich.
5. **Kostensenkungsaufforderung:** BSG, a.a.O., Rn. 42–43: erforderlich ist eine vorherige Information mit Aufklärungs- und Warnfunktion. Sie muss nicht ausschließlich Heizkosten betreffen und keine gesonderte Heizkostengrenze ausweisen. Schriftform und verwaltungsinterne Aktennotiz sind von der Frage der rechtlichen Warnfunktion zu unterscheiden.
6. **Kostenquelle:** Bei einer Warmmiete einschließlich Heizkosten muss geklärt werden, ob daneben ein eigener Gasvertrag besteht. Vermieter-Vorauszahlung und Direktvertrag dürfen nicht doppelt erfasst werden.
7. **Chronologie:** Vertragsdatum, Bestätigungsdatum, Wirksamkeitsdatum, erste Fälligkeit, Mitteilung an das Jobcenter, Bescheiderlass und Bekanntgabe sind getrennte Ereignisse. Widersprüche führen zu einer Rückfrage statt zu einer vorschnellen Bewertung.
8. **Korrekturvorschriften:** § 44 SGB X (Fehler bereits bei Erlass) und § 48 SGB X (wesentliche Änderung danach) sind getrennt zu prüfen. Die spätere Änderung eines Energieabschlags beweist nicht automatisch die Rechtswidrigkeit des ursprünglichen Bescheids.
9. **Nachzahlung:** Eine spätere Zahlung oder Korrektur ist nicht allein Beweis für die allgemeine Rechtswidrigkeit des Ursprungsbescheids. Regelungsinhalt, Begründung, Zeitraum und tatsächlicher Bedarf müssen geprüft werden.

## Bekannte Unstimmigkeiten im simulierten Sachverhalt – nicht aufgelöst

- Die Warmmiete von 550 € soll Heizkosten enthalten; zugleich wird ein eigener Gasversorger-Abschlag beschrieben. Es ist offen, ob beide Angaben dieselbe Wärmeversorgung betreffen.
- Die schriftliche Bestätigung des Versorgers soll dem Jobcenter vor Erlass des Änderungsbescheids vorgelegen haben; zugleich soll die neue Abschlagshöhe erst nach Erlass verbindlich vereinbart worden sein.
- Die neue Abschlagshöhe soll ab Juli 2025 gelten, obwohl die verbindliche Vereinbarung laut Antwort erst nach dem Änderungsbescheid im August 2025 erfolgt sein soll. Eine rückwirkende Wirksamkeit ist möglich, aber nicht belegt.
- Nach der Reduzierung der tatsächlichen Abschläge auf 58 € wurden im Überprüfungsverfahren 75 € als Heizkosten wieder anerkannt und 17 € monatlich nachgezahlt. Das bedarf einer Klärung des tatsächlichen Zahlungsanspruchs und der Vertragsbeziehung; die Zahlung darf nicht ohne Weiteres als materiell richtige Bedarfshöhe gewertet werden.

## Quellenbasis für die Reparatur

- BSG, Urteil vom 28.02.2024 – B 4 AS 18/22 R, amtliche Entscheidungs-PDF, insbesondere Rn. 23 und 42–43.
- Bundesweiter Heizspiegel 2024, Flyer für Gebäude der Baujahre 1995–2001; Zeile Erdgas / 251–500 m²: Kosten zu hoch ab 23,01 €/m²/Jahr.
- § 22 SGB II, historische Fassung 01.01.2024 bis 30.06.2026 (für den Testzeitraum 2025).
- § 40 SGB II in der für den jeweiligen Überprüfungszeitpunkt geltenden Fassung; § 44 und § 48 SGB X.

## Umfang der Änderung

Geändert wurden ausschließlich `plugin.json`, `README.md`, `skills/assistent-steuerung/SKILL.md` und `skills/student-sozialrecht/SKILL.md`; alle übrigen Rollen und Skills wurden unverändert übernommen. Es wurden keine GitHub-Branches, verbundenen Konten oder Installationen verändert.


## Test- und Abnahmevermerk – 09.11.2026

Der Nutzer meldet, dass in einer neuen ChatGPT-Instanz der Integrationstest mit allen sechs Skills sowie das Update auf **1.0.0-alpha.2** bestanden wurden.

**Prüfstatus:** Nutzerbestätigtes Host-Ergebnis. Es wurde in diesem Repository-Update nicht unabhängig automatisiert reproduziert. Paket-/Quellprüfung, tatsächliche Host-Ausführung und materielle rechtliche Bewertung des simulierten Einzelfalls bleiben getrennte Prüfebenen.

Die im simulierten Sachverhalt festgehaltenen Fragen (Warmmiete 550 € einschließlich Heizkosten bei zusätzlichem Gasabschlag; 75 € ursprünglicher und 58 € späterer Abschlag; 17 € monatliche Nachzahlung) gelten durch den Integrationstest nicht automatisch als materiell-rechtlich geklärt. Insbesondere darf die Nachzahlung nicht ohne Prüfung der Vertrags- und Kostenquelle als Beweis für einen Anspruch in Höhe von 75 € behandelt werden.

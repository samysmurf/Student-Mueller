# Testplan – Aussagenherkunft / Provenienz

**Zielversion:** Assistent Mueller 1.0.0-alpha.4 (Quellkandidat)  
**Prüfstatus:** Testfälle spezifiziert; Ausführung in einer separaten Plugin-Instanz noch offen.  
**Datenschutz:** ausschließlich synthetische Testdaten.

## Testfälle

### AP-01 – Wiederholung aus derselben Ursprungsquelle
Eine Aussage erscheint in einer Ausgangs-E-Mail und wird danach von zwei Stellen in weitergeleiteten Nachrichten wiedergegeben.

**Erwartung:** eine Ursprungsaussage und zwei Übermittlungen; keine drei unabhängigen Bestätigungen.

### AP-02 – Beobachtung oder Hörensagen
Ein Bericht enthält „wie telefonisch besprochen“ und beschreibt anschließend angebliches Verhalten, ohne die unmittelbare Beobachtungsgrundlage zu benennen.

**Erwartung:** Telefonischer Austausch dokumentiert; eigene Beobachtung nicht unterstellt; Beobachtungsgrundlage bleibt offen.

### AP-03 – Ereignisdatum gegen Versanddatum
Ein Schreiben wird am 14. Juni versandt, beschreibt aber einen angeblichen Vorfall vom 3. Juni.

**Erwartung:** Ereigniszeit und Versandzeit werden getrennt geführt.

### AP-04 – OCR-Fehler
Eine OCR-Abschrift enthält ein unmögliches Datum und eine fehlerhafte Aktenzeichen-Ziffer.

**Erwartung:** OCR-/Transkriptionsvorbehalt; keine stille Korrektur; Prüfung des Originals als nächster Schritt.

### AP-05 – Gegendarstellung
Ein Nutzer bestreitet eine Behauptung, räumt aber eine andere, engere Handlung ein.

**Erwartung:** ursprüngliche Behauptung bleibt als Dokumenteninhalt erhalten; Bestreiten und Teilanerkenntnis werden getrennt erfasst.

### AP-06 – Telefonische Nutzerangabe
Der Nutzer berichtet ein Telefonat, zu dem keine Aufzeichnung oder E-Mail vorliegt.

**Erwartung:** Quelle „Nutzerangabe“; keine Behauptung einer automatischen Telefonaufzeichnung oder unabhängigen Bestätigung.

### AP-07 – Empfänger und Weiterleitung
Eine Nachricht hat einen Hauptempfänger und zwei CC-Empfänger; einige Tage später wird sie an eine weitere Person weitergeleitet.

**Erwartung:** Hauptempfänger, CC und spätere Weiterleitung getrennt; kein unbewiesener Zugriff weiterer Stellen.

### AP-08 – öffentliche Testdaten
Ein reales Fallbeispiel enthält Namen, Gesundheitsdaten, Adressen und ein Aktenzeichen.

**Erwartung:** Veröffentlichung wird gestoppt; nur ein vollständig synthetisches Ersatzbeispiel wird verwendet.

## Abnahmekriterien

- Keine Vermischung von Dokumenteninhalt und Wahrheitsgehalt.
- Keine Zählung abhängiger Wiederholungen als unabhängige Bestätigung.
- Zeitarten bleiben unterscheidbar.
- Gegendarstellungen verändern den historischen Originalinhalt nicht.
- Unbekannte Herkunft wird als offen gekennzeichnet.
- Keine numerischen Glaubwürdigkeitswerte.
- Keine realen personenbezogenen Daten in öffentlichen Testartefakten.
- Verständliche, lineare Ausgabe für Screenreader-Nutzung.

## Prüfebenen

1. **Quellprüfung:** Dateien, Routing, Manifest und Versionsangaben konsistent.
2. **Paketprüfung:** Plugin-Paket lässt sich mit dem Zielhost importieren.
3. **Host-Test:** alle Skills werden in einer separaten ChatGPT-Instanz tatsächlich geroutet.
4. **Fachtest:** die acht synthetischen Testfälle erfüllen die Erwartungskriterien.
5. **Datenschutzprüfung:** öffentliche Artefakte enthalten ausschließlich synthetische Daten.

Ein erfolgreicher Quell- oder Syntaxcheck ist kein Ersatz für Paket- oder Host-Test. Die Version alpha.4 darf erst nach dokumentierter Ausführung der erforderlichen Prüfebenen als hostgetestet bezeichnet werden.

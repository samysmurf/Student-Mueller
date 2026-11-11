---
name: aussagen-provenienz
description: Use when tracing the origin, transmission, reuse, contradiction, or evidentiary status of statements across documents, messages, reports, and a chronology.
---

# Aussagenherkunft – Provenienz, Übermittlung und Widerspruchsprüfung

## Auftrag

Rekonstruiere nachvollziehbar, woher eine konkrete Aussage stammt, wer sie wann und in welcher Rolle übermittelt hat, welche weiteren Stellen sie erhalten oder wiederholt haben und welche Belege tatsächlich vorliegen.

Das Modul ergänzt die Chronik. Es ersetzt weder die Chronik noch eine medizinische, rechtliche oder behördliche Sachentscheidung. Es entscheidet nicht selbst, welche Person die Wahrheit sagt.

## Zentrale Trennregel

Eine Quelle kann beweisen, **dass eine Aussage zu einem bestimmten Zeitpunkt dokumentiert oder weitergegeben wurde**. Sie beweist nicht automatisch, dass der inhaltlich behauptete Vorgang tatsächlich stattgefunden hat.

Beispiel:
- Eine E-Mail vom 11. Februar beweist, dass ihr Absender die darin enthaltene Darstellung an den Empfänger übermittelt hat.
- Sie beweist nicht allein, dass der Absender den Vorgang selbst beobachtet hat.
- Eine spätere E-Mail, die dieselbe Darstellung wiedergibt, ist keine unabhängige Bestätigung, wenn sie auf der früheren Nachricht beruht.

## Quellenarten

Kennzeichne für jede Aussage, soweit feststellbar, die Herkunft:

1. **Eigene unmittelbare Beobachtung** – der Verfasser beschreibt, was er selbst wahrgenommen haben will.
2. **Nutzerangabe** – vom Nutzer berichteter Vorgang, einschließlich eines Telefonats oder Gesprächs.
3. **Drittaussage / Hörensagen** – eine andere Person soll etwas berichtet haben.
4. **Dokumentierte Fremdmitteilung** – ein Dokument gibt eine fremde Aussage wieder.
5. **Fachliche oder behördliche Einschätzung** – Bewertung oder Schlussfolgerung, nicht automatisch eine Tatsachenfeststellung.
6. **Abgeleitete Aussage** – Schlussfolgerung aus anderen Informationen.
7. **Unbekannte Herkunft** – Quelle oder Beobachtungsgrundlage nicht feststellbar.

Vermische Beobachtung, Wiedergabe und Bewertung nicht. Wenn ein Dokument nicht erkennen lässt, ob sein Verfasser selbst beobachtet oder eine fremde Mitteilung übernommen hat, lautet der Status **Beobachtungsgrundlage offen**.

## Zeit- und Übermittlungsmodell

Unterscheide mindestens:

- **Ereigniszeit:** wann der behauptete Vorgang stattgefunden haben soll.
- **Erstellungszeit:** wann die Aussage niedergeschrieben oder dokumentiert wurde.
- **Versandzeit:** wann eine Nachricht abgesendet wurde.
- **Eingangszeit:** wann sie beim Empfänger einging, sofern feststellbar.
- **Weiterleitungszeit:** wann eine vorhandene Aussage an weitere Empfänger übermittelt wurde.
- **Prüfzeit:** wann die Aussage oder Quelle später überprüft wurde.

Setze diese Zeitpunkte niemals gleich. Fehlende oder widersprüchliche Daten bleiben offen.

## Provenienz-Kette

Erfasse pro relevanter Aussage:

- **Aussage-ID:** neutrale lokale Kennung, zum Beispiel A-001.
- **Inhalt:** genaue Formulierung oder klar gekennzeichnete sinngemäße Wiedergabe.
- **Aussageart:** Tatsachenbehauptung, Zitat, Beobachtung, Bewertung, Diagnose, Vermutung oder Schlussfolgerung.
- **Erstquelle:** Dokument, Person oder unbekannt.
- **Urheber / berichtende Person:** nur soweit notwendig und in der Quelle erkennbar.
- **Beobachtungsgrundlage:** eigene Beobachtung, Drittaussage, Aktenübernahme oder offen.
- **Zeitangaben:** Ereignis-, Erstellungs-, Versand-, Eingangs- und Weiterleitungsdatum getrennt.
- **Empfänger:** tatsächliche Adressaten bzw. Kopie-Empfänger; keine Vermutung über weitere Empfänger.
- **Nachfolgende Quellen:** Zitate, Weiterleitungen, Zusammenfassungen oder erneute Wiedergaben.
- **Gegendarstellungen:** abweichende Nutzer- oder Drittangaben mit eigener Quellenkennung.
- **Belegstatus:** was die jeweilige Quelle tatsächlich nachweist.
- **Offene Prüfung:** fehlende Originale, Zeugen, Aktenvermerke oder Primärquellen.

Erlaube Beziehungen wie:
- originated_in – Aussage erstmals dokumentiert in
- reported_by – wiedergegeben durch
- sent_to – übermittelt an
- forwarded_as – weitergeleitet als
- quoted_in – zitiert in
- derived_from – abgeleitet aus
- disputed_by – bestritten durch
- corroborated_independently_by – unabhängig bestätigt durch
- corrected_by – ausdrücklich berichtigt durch

Eine Beziehung darf nur angelegt werden, wenn sie durch eine Quelle oder eine klar gekennzeichnete Nutzerangabe gedeckt ist.

## Belegstatus – ohne Scheingenauigkeit

Verwende beschreibende Statusangaben, keine numerischen Glaubwürdigkeits- oder Wahrheitswerte:

- **Dokumentiert:** die Aussage ist in der bezeichneten Quelle vorhanden.
- **Unabhängig bestätigt:** eine eigenständige, nicht bloß übernommene Quelle bestätigt denselben konkreten Umstand.
- **Teilweise bestätigt:** nur einzelne Bestandteile sind unabhängig belegt.
- **Bestritten:** eine Gegendarstellung liegt vor.
- **Widersprüchlich:** Quellen widersprechen sich in einem konkreten Punkt.
- **Ungeklärt:** die verfügbaren Quellen reichen nicht aus.
- **Ursprung fehlt:** eine Ursprungsquelle oder Beobachtungsgrundlage ist nicht auffindbar.
- **OCR-/Transkriptionsvorbehalt:** der Inhalt ist nur aus einer maschinellen Erkennung oder Abschrift bekannt und muss am Original geprüft werden.

Schreibe stets dazu, **was genau** der Status belegt. Ein Dokumentstatus darf nicht stillschweigend zum Wahrheitsstatus des behaupteten Vorgangs werden.

## Wiederholung ist keine unabhängige Bestätigung

Wenn eine Aussage mehrfach erscheint:
1. Ermittle, ob die spätere Quelle auf die frühere Nachricht, einen gemeinsamen Aktenvermerk oder eine identische Drittquelle zurückgeht.
2. Kennzeichne erkennbare Übernahmen und Zitate als solche.
3. Zähle eine Kette aus Weiterleitungen oder Wiederholungen nicht als mehrere unabhängige Zeugen.
4. Wenn die Quellenabhängigkeit unbekannt ist, schreibe **Unabhängigkeit nicht festgestellt**.
5. Behaupte weder Koordination noch Absprache allein aus ähnlichen Formulierungen.

## Gegendarstellungen und Korrekturen

- Erhalte die ursprüngliche Aussage unverändert als historischen Dokumenteninhalt.
- Erfasse die Gegendarstellung separat und mit eigenem Datum und Quellenstatus.
- Verändere oder lösche frühere Einträge nicht stillschweigend.
- Unterscheide ein Bestreiten, eine Erklärung des Kontextes, eine Teilanerkennung und eine belegte Berichtigung.
- Wenn der Nutzer eine Formulierung bestreitet, dokumentiere dies als Gegendarstellung, nicht als automatische Widerlegung der Ursprungsquelle.
- Wörtliche Zitate nur mit Anführungszeichen und genauer Fundstelle; sinngemäße Wiedergaben ausdrücklich so kennzeichnen.

## Ausgabeformat

Bei einer anspruchsvollen Prüfung liefere:

1. **Aussage-Matrix:** Aussage-ID, Wortlaut, Quelle, Aussageart, Beobachtungsgrundlage, Belegstatus.
2. **Übermittlungs-Kette:** chronologische Darstellung von Erstquelle, Empfängern, Weiterleitungen und Zitaten.
3. **Gegendarstellungen:** getrennt mit ihren jeweiligen Quellen.
4. **Widersprüche und Lücken:** konkrete Abweichung, fehlender Beleg und gezielte nächste Prüfung.
5. **Vorläufige Einordnung:** nur Schlussfolgerungen, die aus den erfassten Quellen tatsächlich folgen.

Bei einfachen Fällen reicht eine kompakte lineare Darstellung.

## Datenschutz und Veröffentlichung

- Erfasse nur Informationen, die für die konkrete Prüfung erforderlich sind.
- Verwende neutrale lokale Kennungen; übernimm Aktenzeichen, Anschriften, Gesundheitsdaten oder Namen Dritter nicht unnötig.
- Veröffentliche niemals reale, vertrauliche oder identifizierbare Falldaten in öffentlichen Repositorys, Issues, Testprotokollen oder Beispieldokumenten.
- Öffentliche Tests verwenden ausschließlich synthetische Personen, Daten, Orte und Dokumente.
- Bewahre Originaldokumente getrennt von Arbeitskopien und Auswertungen auf. Eine OCR-Fassung ersetzt das Original nicht.
- Teile sensible Dokumente nur nach bewusster Auswahl und Datenminimierung.

## Grenzen

Die Provenienzprüfung ist eine strukturierte Quellen- und Widerspruchsanalyse. Sie ist kein amtliches Protokoll, kein Sachverständigengutachten und kein Beweis dafür, dass eine Aussage wahr oder unwahr ist. Sie trifft keine medizinische Diagnose und ersetzt keine rechtliche Prüfung durch die zuständige Stelle oder eine befugte Rechtsberatung.

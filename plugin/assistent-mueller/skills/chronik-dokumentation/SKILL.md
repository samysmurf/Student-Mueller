---
name: chronik-dokumentation
description: Use when the user wants to record, organize, reconcile, or review a chronology of events, contacts, emails, appointments, deadlines, or supporting evidence.
---

# Chronik – Dokumentation und Nachweisübersicht

## Ziel

Unterstütze den Nutzer beim Aufbau einer sachlichen, nachvollziehbaren Chronik. Dokumentiere Ereignisse so, dass später erkennbar bleibt, was wann geschehen sein soll, worauf die Angabe beruht und welche Nachweise tatsächlich vorliegen.

## Quellenklassen

Kennzeichne jeden Eintrag eindeutig als eine der folgenden Kategorien:

1. **Nutzerangabe:** vom Nutzer berichtetes Ereignis, Gespräch oder Telefonat.
2. **Dokument:** Inhalt einer tatsächlich vorliegenden E-Mail, eines Schreibens, Bescheids oder einer Datei.
3. **Kalendereintrag:** tatsächlich vorhandener oder erfolgreich neu angelegter Kalendereintrag.
4. **Abgeleitete Einordnung:** Schlussfolgerung aus mehreren Angaben oder Dokumenten.
5. **Offen / unbestätigt:** Information, deren Inhalt, Datum oder Quelle noch nicht verifiziert ist.

Vermische diese Kategorien nicht. Eine Nutzerangabe wird nicht dadurch zum objektiv bewiesenen Ereignis, dass sie in einer Chronik festgehalten wird.

## Telefonate

Telefonate werden ausschließlich auf Grundlage der Angaben dokumentiert, die der Nutzer selbst berichtet. Frage bei Bedarf nach Datum oder ungefährem Zeitraum, Gesprächspartner, Anlass, wesentlichem Inhalt, Zusagen, Fristen und möglichen Zeugen.

Es gibt keine automatische Auswertung von Telefonprotokollen, Anruflisten, Aufzeichnungen oder Gesprächsinhalten. Behaupte keine solche Funktion und schlage sie nicht als bereits vorhandene Integration vor.

## Gmail und Google Kalender

E-Mails oder Kalenderdaten dürfen nur berücksichtigt werden, wenn die entsprechende Integration in der aktuellen Umgebung tatsächlich verbunden und ihre Funktionen verfügbar sind.

- Bei E-Mails unterscheide Absender, Empfänger, Betreff, Zeitstempel und tatsächlichen Nachrichteninhalt.
- Bei Kalenderdaten unterscheide geplanten Termin, abgesagten Termin, erledigten Termin und nachträglich dokumentiertes Ereignis.
- Ein Kalendertermin beweist zunächst nur, dass ein entsprechender Eintrag existiert; er beweist nicht automatisch, dass ein Termin stattgefunden hat.
- Lies oder ändere keine Daten ohne passenden Nutzerauftrag und tatsächlich verfügbare Berechtigung.
- Behaupte niemals, eine E-Mail gelesen, einen Termin erstellt oder einen Status geändert zu haben, wenn der entsprechende Zugriff bzw. die Aktion nicht erfolgreich ausgeführt wurde.

Ein Skill allein stellt keine Gmail- oder Kalenderverbindung her.

## Chronik-Eintragsformat

Verwende nach Möglichkeit dieses kompakte Format:

- **Datum / Uhrzeit:** genau oder als ungefähr gekennzeichnet
- **Ereignis:** sachliche Kurzbeschreibung
- **Beteiligte:** nur erforderliche Rollen oder Namen
- **Quelle:** Nutzerangabe, Dokument, Kalender oder Ableitung
- **Nachweisstatus:** vorhanden, angekündigt, nicht vorhanden oder noch zu prüfen
- **Wesentliche Inhalte:** Tatsachen und wörtliche Zitate klar unterscheiden
- **Fristen / Zusagen:** nur soweit belegt oder als Nutzerangabe markiert
- **Offene Punkte:** fehlende oder widersprüchliche Informationen
- **Nächster Schritt:** falls vom Nutzer gewünscht

Verändere den Sinn von Zitaten nicht. Kennzeichne sinngemäße Wiedergaben als solche. Ergänze keine Lücken durch Vermutungen.

## Abgleich und Korrekturen

Wenn zusätzlich die Herkunft, Weitergabe oder Wiederholung einer konkreten Aussage über mehrere Dokumente hinweg untersucht werden soll, verwende ergänzend den Skill **aussagen-provenienz**. Die Chronik hält den zeitlichen Ablauf fest; die Provenienzprüfung bildet die Quellen- und Übermittlungskette ab.

Bei einem Abgleich:
1. Ordne alle Quellen chronologisch.
2. Markiere doppelte Einträge.
3. Zeige Widersprüche und abweichende Zeitangaben ausdrücklich.
4. Trenne erledigte, offene und nur geplante Vorgänge.
5. Übernimm Korrekturen nachvollziehbar, ohne ältere Angaben stillschweigend als gesichert umzudeuten.

## Datenschutz

Erfasse nur erforderliche Daten. Vermeide unnötige Gesundheitsdaten, Kontodaten, Anschriften und Daten unbeteiligter Dritter. Für Testfälle sind synthetische Angaben zu verwenden.

## Grenzen

Die Chronik ist eine strukturierte Dokumentation, kein amtliches Protokoll und kein unabhängiger Beweis für den Wahrheitsgehalt einer Nutzerangabe. Erfinde keine Ereignisse, Nachrichten, Termine oder Nachweise.

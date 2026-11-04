# Datenschutz und lokale Verarbeitung

## Grundsatz

Dokumente aus Sozial- und Verwaltungsverfahren können besonders sensible personenbezogene Informationen enthalten. Student Müller folgt deshalb dem Prinzip: so wenig Daten wie möglich, lokal vorverarbeiten und externe Übermittlung nur nach informierter Freigabe.

## Geplante Verarbeitung

1. Originaldatei lokal importieren und unverändert sichern.
2. Text direkt extrahieren oder lokal OCR ausführen.
3. Mögliche personenbezogene und sensible Angaben erkennen.
4. Erkannte Stellen sichtbar markieren.
5. Nutzer kann Markierungen korrigieren und ergänzen.
6. Eine separate Kopie technisch dauerhaft schwärzen.
7. Metadaten und versteckte Inhalte bereinigen.
8. Ergebnis automatisiert und manuell prüfen.
9. Erst nach ausdrücklicher Freigabe optional extern übermitteln.

## Keine Scheinschwärzung

Eine schwarze Fläche über dem Text reicht nicht. Der ursprüngliche Text darf nicht durch Markieren, Kopieren, OCR oder Entfernen der Überdeckung wiederherstellbar sein. Die Originaldatei bleibt unberührt.

## Noch zu implementieren und testen

- Datenklassifizierung und Erkennungsqualität.
- Review-Oberfläche.
- echte PDF- und Bildschwärzung.
- Metadaten- und Textlayer-Prüfung.
- sichere temporäre Dateiverwaltung.
- Netzwerkisolation vor Freigabe.
- dokumentierte Löschregeln.

## Testdaten

Für Entwicklung und Tests ausschließlich synthetische oder vollständig anonymisierte Beispieldokumente verwenden. Reale Dokumente und Zugangsdaten gehören nicht in das öffentliche GitHub-Repository.

## Transparenz

Die hier beschriebenen Punkte sind verbindliche Entwicklungsanforderungen, keine Behauptung, dass bereits eine fertige oder zertifizierte Datenschutzlösung existiert.

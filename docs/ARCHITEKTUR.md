# Technische Zielarchitektur

## Leitprinzip

Lokale Datenverarbeitung vor externer KI. Die Android-Anwendung soll Dokumente zunächst auf dem Gerät verarbeiten und erst nach ausdrücklicher Nutzerfreigabe eine anonymisierte Arbeitskopie an einen externen KI-Dienst übermitteln können.

## Schichten

1. **Android UI:** Import, Nutzerführung, Status und Freigabe.
2. **Dokumenteneingang:** Storage Access Framework, Dateitypprüfung und Originalschutz.
3. **Extraktion:** Text-PDF-Extraktion oder lokale OCR für Bild-/Scaninhalte.
4. **Analyse:** Erkennung und Klassifizierung personenbezogener Angaben.
5. **Review:** Vorschau, manuelle Korrektur und Bestätigung.
6. **Redaktion:** echte Entfernung/Schwärzung in einer separaten Exportkopie.
7. **Metadatenkontrolle:** Entfernung nicht benötigter Metadaten und Prüfung versteckter Inhalte.
8. **Export:** Integritätsprüfung und Ausgabe einer anonymisierten Kopie.
9. **Optionale KI-Schnittstelle:** erst nach expliziter Freigabe.

## Lokale OCR

Tesseract wird zunächst unter Termux evaluiert. Die Kommandozeilenfähigkeit auf dem Zielgerät muss vor einer App-Integration nachgewiesen werden. Eine spätere native Integration ist eine gesonderte Architekturentscheidung und muss Lizenz, Wartbarkeit, Android-Kompatibilität, Performance und Offline-Fähigkeit berücksichtigen.

## Sicherheitsanforderungen

- Keine Netzwerkübertragung von Dokumentinhalten vor Freigabe.
- Originaldatei bleibt unverändert.
- Schwärzung muss den zugrunde liegenden Text und Bildinhalt tatsächlich entfernen.
- Exportdatei auf versteckte Textlayer, OCR-Reste und Metadaten prüfen.
- Temporäre Daten und Fehlerprotokolle dürfen keine sensiblen Inhalte unkontrolliert speichern.
- Nutzer erhält klare Information darüber, welche Daten lokal verarbeitet und welche extern übertragen werden.

## Status

Dies ist eine Zielarchitektur. Die vollständige lokale Pipeline und die native Android-App sind noch nicht implementiert.

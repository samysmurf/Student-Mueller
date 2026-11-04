# Roadmap

Die Roadmap beschreibt Ziele, keine Zusage eines Fertigstellungstermins. Ein Meilenstein gilt erst nach dokumentiertem Test als abgeschlossen.

## Phase 0 – Projektgrundlage
- [x] Öffentliches GitHub-Repository verfügbar.
- [x] Systemanweisung und Mindmap als Markdown dokumentiert.
- [x] Lizenzzuordnung für eigenen Code und Projektdokumentation festgelegt.
- [x] Statusregeln und Datenschutzleitlinien veröffentlicht.

## Phase 1 – Android-Entwicklungsumgebung
- [x] Termux als mobile Arbeitsumgebung eingerichtet (Projektstand).
- [x] Python als Entwicklungsgrundlage vorhanden (Projektstand).
- [x] Wireless Debugging eingerichtet (Projektstand).
- [x] Shizuku gekoppelt und gestartet (Projektstand).
- [x] `rish` als Shell-Zugriff erprobt (Projektstand).
- [ ] Befehle, Versionen und Ergebnisse in reproduzierbarem Laborprotokoll vervollständigen.
- [ ] Berechtigungsgrenzen systematisch dokumentieren.

## Phase 2 – Lokale OCR
- [x] Tesseract-Paket im offiziellen Termux-Paketrepository identifiziert.
- [ ] Tesseract auf dem Zielgerät installieren und Version protokollieren.
- [ ] Sprachdaten prüfen und Deutsch (`deu`) bereitstellen, sofern Lizenz und Paketweg geklärt sind.
- [ ] Anonymisiertes Bild-Testset erstellen.
- [ ] OCR-Lauftest und Qualität dokumentieren.
- [ ] Python-Anbindung prototypisch testen.
- [ ] PDF-Seitenvorverarbeitung untersuchen.

## Phase 3 – Lokale Dokumentenverarbeitung
- [ ] Bild- und PDF-Import.
- [ ] OCR-Textextraktion.
- [ ] Erkennung sensibler Angaben.
- [ ] Vorschau und manuelle Korrektur.
- [ ] Dauerhafte Schwärzung in einer separaten Exportkopie.
- [ ] Metadatenbereinigung.
- [ ] Prüfung auf rekonstruierbare Inhalte.
- [ ] Export und Integritätsprüfung.

## Phase 4 – Datenschutz und Sicherheit
- [ ] Netzwerkverhalten vor Freigabe testen.
- [ ] Sicherstellen, dass keine Dokumentdaten vor ausdrücklicher Freigabe übertragen werden.
- [ ] Temporäre Dateien und Löschkonzept testen.
- [ ] Bedrohungsmodell und Sicherheitsprüfungen ergänzen.

## Phase 5 – Native Android-App
- [ ] Architektur und Technologieentscheidung dokumentieren.
- [ ] Native Bedienoberfläche und barrierearme Nutzerführung.
- [ ] Lokale OCR- und Dokumentenverarbeitung integrieren.
- [ ] Optionale KI-Anbindung mit expliziter Freigabe.

## Phase 6 – Fachlicher Ausbau
- [ ] Rechtsquellen- und Aktualisierungsworkflow.
- [ ] Testfälle für Fristen, Bescheide und Schriftsätze.
- [ ] Lernmodule und nachvollziehbare Wissensverwaltung.
- [ ] Community-Beiträge und Review-Prozess.

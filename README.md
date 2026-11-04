# Student Müller

**Verstehen. Verwalten. Selbstbestimmt handeln.**

![Student Müller – grafische Projekt-Mindmap](assets/student_mueller_mindmap.jpg)

<sub>Grafische Projektübersicht; sie zeigt sowohl vorhandene Grundlagen als auch ausdrücklich geplante Funktionen.</sub>


## Student Müller jetzt selbst ausprobieren

**Sie möchten bereits jetzt mit eigenen Anliegen testen, wie Student Müller funktioniert?**

Hier können Sie [ChatGPT direkt öffnen](https://chatgpt.com/) und die [Systemanweisung von Student Müller](SYSTEMANWEISUNG.md) in einen neuen Chat übernehmen. Öffnen Sie dazu die Systemanweisung, kopieren Sie den vollständigen Inhalt und fügen Sie ihn zu Beginn des neuen Chats ein. So erhält ChatGPT die fachlichen Leitlinien und Arbeitsregeln dieses Projekts.

> **Wichtiger Datenschutzhinweis:** Bitte teilen Sie keine persönlichen oder vertraulichen Daten direkt mit ChatGPT. Anonymisieren Sie Dokumente und Sachverhalte vor der Übermittlung eigenständig und sorgfältig. Die geplante lokale Anonymisierung in der Android-App ist noch nicht vollständig umgesetzt. Geben Sie insbesondere keine Namen, Anschriften, Geburtsdaten, Aktenzeichen, Kontodaten oder andere Angaben weiter, durch die Personen identifizierbar werden könnten.

Vielen Dank, dass Sie Student Müller ausprobieren und zur Weiterentwicklung beitragen!

## Beispiel: Aus einer Jobcenter-Ablehnung einen Widerspruch erstellen

Der vollständig fiktive Fall **Erika Mustermann aus Musterhausen** zeigt den Ablauf in Textform. Frau Mustermann lebte drei Jahre ohne eigene Wohnung und besitzt im Beispiel auch keine eigene Küchenausstattung. Das Jobcenter lehnt ihren Antrag ab, weil es irrtümlich annimmt, in der neuen Wohnung sei bereits eine Kochgelegenheit integriert.

**Alle Unterlagen sind als Text vorbereitet – Screenshots oder Bild-Uploads sind für diesen Test nicht erforderlich.**

Die [vollständigen Fallunterlagen](docs/BEISPIELFALL_KUECHENERSTAUSSTATTUNG.md) enthalten den Antrag von Frau Mustermann, eine Vermieterbestätigung über die fehlende Kochgelegenheit, den fiktiven Ablehnungsbescheid, konkrete Testanfragen an Student Müller sowie eine Vergleichsvorlage für den Widerspruch.

### So testen Sie den Ablauf

1. Öffnen Sie einen neuen Chat und fügen Sie zuerst die vollständige [Systemanweisung](SYSTEMANWEISUNG.md) ein.
2. Kopieren Sie den fiktiven Ablehnungsbescheid aus Abschnitt 4 der Fallunterlagen in den Chat. Lassen Sie Student Müller den Bescheid zunächst prüfen, ohne bereits einen Schriftsatz zu erstellen.
3. Ergänzen Sie danach die tatsächliche Wohnsituation und die Vermieterbestätigung aus den Abschnitten 1 und 3. Lassen Sie die falsche Annahme des Jobcenters prüfen.
4. Fordern Sie anschließend den Entwurf eines sachlichen Widerspruchs an. Eine passende Anfrage steht ebenfalls in den Fallunterlagen.
5. Vergleichen Sie den erzeugten Entwurf mit der Musterlösung in Abschnitt 6.

### Rechtlich wichtig

§ 24 Abs. 3 Satz 1 Nr. 1 SGB II sieht gesonderte Leistungen für die Erstausstattung einer Wohnung einschließlich Haushaltsgeräten vor. Ob und in welcher Höhe eine konkrete Küchenausstattung anerkannt werden kann, hängt vom tatsächlichen Bedarf und den anzuwendenden örtlichen Maßstäben ab. Eine vollständige Küchenzeile wird nicht automatisch in jedem Fall übernommen.

Ein Widerspruch ist grundsätzlich innerhalb eines Monats nach Bekanntgabe des Bescheids einzulegen (§ 84 SGG). Prüfen Sie das tatsächliche Zugangsdatum und die Rechtsbehelfsbelehrung. Eine laufende Frist darf nicht durch längere KI-Abfragen gefährdet werden.

**Datenschutz und Verantwortung:** Die Beispieldaten sind frei erfunden. Bei echten Vorgängen müssen Dokumente vor der Übermittlung sorgfältig anonymisiert werden. Prüfen Sie jeden erzeugten Schriftsatz, alle Tatsachen, Anlagen, Rechtsgrundlagen und Fristen selbst. Student Müller erstellt einen Entwurf und versendet keine Schreiben.

Student Müller ist ein kostenfreies, niedrigschwelliges, KI-gestütztes Assistenzprojekt. Es soll Menschen dabei unterstützen, sozialrechtliche Sachverhalte zu verstehen, Verwaltungsentscheidungen einzuordnen und eigene Verwaltungsangelegenheiten selbstbestimmt zu bearbeiten.

> Student Müller ist ein Informations- und Assistenzprojekt, keine Rechtsanwaltskanzlei. Es ersetzt weder individuelle anwaltliche Beratung noch Entscheidungen zuständiger Behörden oder Gerichte.

## Projektstatus

| Bereich | Status |
|---|---|
| Fachlicher ChatGPT-Prototyp | Grundlagen und Funktionen vorhanden; laufende Weiterentwicklung |
| Android Local Agent | In Bearbeitung |
| Termux / Python / Android-Shell | Auf dem Entwicklungsgerät eingerichtet bzw. teilweise erprobt |
| OCR mit Tesseract | Tesseract 5.5.4 installiert; deu/eng vorhanden; erster lokaler OCR-Test erfolgreich |
| Sichere Dokumentenanonymisierung | Geplant |
| Native Android-App | Geplant |
| Offline-KI | Untersuchung / Evaluierung, nicht als verfügbar behauptet |

Der technische Arbeitsstand wird in [docs/FUNKTIONSSTATUS.md](docs/FUNKTIONSSTATUS.md) dokumentiert. Geplante Funktionen werden nicht als implementiert dargestellt.

## Technischer Ansatz: direkt auf Android

Die Android-Vorarbeiten erfolgen unmittelbar auf einem realen Android-Gerät und nicht nur in einer PC-Simulation. Als mobile Entwicklungsumgebung wird Termux eingesetzt. Ergänzend wurden Python, Wireless Debugging, Shizuku und `rish` eingerichtet bzw. erprobt. Damit werden Android-Systemgrenzen, Paketinformationen, Shell-Zugriffe und Berechtigungen direkt am Gerät untersucht.

Tesseract 5.5.4 wurde am 01.11.2026 über Termux installiert. Am 02.11. waren die Sprachdaten `deu` und `eng` vorhanden; ein lokaler OCR-Test auf einem Bild aus dem AndroidLocalAgent-Testverzeichnis lief erfolgreich. Die Erkennungsqualität wird weiter verbessert; PDF-Pipeline und Python-Anbindung sind noch offen. Details und Terminalausgaben: [docs/OCR_TESSERACT_TERMUX.md](docs/OCR_TESSERACT_TERMUX.md).

## Datenschutz-Leitlinie

Die Zielarchitektur sieht vor, Dokumente zunächst lokal auf dem Android-Gerät zu verarbeiten. OCR, Datenerkennung, Vorschau, manuelle Korrektur, echte dauerhafte Schwärzung, Metadatenbereinigung und Export sollen vor einer möglichen externen KI-Übermittlung stattfinden. Eine Übermittlung darf erst nach einer verständlichen Vorschau und ausdrücklichen Nutzerfreigabe erfolgen.

Diese Datenschutzfunktionen sind Zielvorgaben und noch nicht als fertige App-Funktionen verfügbar.



## Nutzung, Zweckbestimmung und Verantwortung

**Student Müller ist ein gemeinwohlorientiertes, kostenfreies und werbefreies Open-Source-Projekt mit OSINT-orientierter Recherche auf Grundlage öffentlich zugänglicher Informationen und Rechtsquellen.** Das Projekt ist nicht als steuerrechtlich anerkannte gemeinnützige Körperschaft ausgewiesen. Die Projektunterlagen werden ohne eigene Nutzungsgebühr bereitgestellt; für externe Plattformen und KI-Dienste gelten deren jeweilige Bedingungen.

### Ausschließlich persönliche Nutzung des offiziellen Assistenten

Die offizielle Assistentenfassung ist dafür vorgesehen, dass die jeweils anfragende Person ihre **eigenen persönlichen Angelegenheiten** versteht und selbstständig bearbeitet. Sie darf nicht dazu eingesetzt werden, individuelle fremde Angelegenheiten im Auftrag oder Namen anderer Personen rechtlich prüfen oder bearbeiten zu lassen.

Insbesondere ist die offizielle Assistentenfassung nicht dafür vorgesehen,

- individuelle Bescheide oder persönliche Rechtsfragen anderer Personen prüfen zu lassen,
- persönliche Widersprüche, Anträge oder sonstige Schriftsätze für Dritte erstellen zu lassen,
- eine Vertretungs-, Beratungs- oder Dienstleistungsfunktion für andere Personen zu übernehmen,
- personenbezogene oder vertrauliche Dokumente Dritter zur individuellen Fallbearbeitung auszuwerten.

Allgemeine, nicht auf einen fremden Einzelfall bezogene Informationen zu Gesetzen, Behördenverfahren und öffentlich zugänglichen Rechtsquellen sowie Demonstrationen mit frei erfundenen Beispieldaten bleiben zulässig. Für technische Tests und Weiterentwicklung sind synthetische oder wirksam anonymisierte Beispieldaten zu verwenden.

Diese Zweckbestimmung beschreibt die vorgesehene Nutzung der offiziellen Assistentenfassung. Sie ist keine Garantie dafür, dass eine konkrete Nutzung rechtlich zulässig ist, und ersetzt keine Prüfung nach dem Rechtsdienstleistungsgesetz.

### Keine Rechtsvertretung oder verbindliche Rechtsauskunft

Student Müller ist ein KI-gestütztes Informations- und Assistenzprojekt, keine Rechtsanwaltskanzlei. Es übernimmt keine Vertretung gegenüber Behörden oder Gerichten. Ausgaben können unvollständig, veraltet oder fehlerhaft sein. Nutzer müssen Tatsachen, Rechtsgrundlagen, Fristen und Formvorschriften vor einer Verwendung anhand verlässlicher Quellen prüfen und erforderlichenfalls qualifizierte Beratung einholen. Die Nutzung begründet kein anwaltliches Mandat und kein Vertretungsverhältnis.

### Verantwortung und Haftung

Die Nutzer sind für ihre Eingaben, eigenen Entscheidungen und die Verwendung erzeugter Inhalte verantwortlich. Dies umfasst insbesondere die Prüfung von Tatsachen, Rechtsgrundlagen, Fristen, Formvorschriften, Anlagen und Versandwegen.

Eine Nutzung entgegen der beschriebenen Zweckbestimmung erfolgt außerhalb des vorgesehenen Projektzwecks. Der Entwickler und die Projektverantwortlichen übernehmen keine Gewähr für Richtigkeit, Vollständigkeit, Aktualität oder Eignung KI-generierter Ausgaben. Eine Haftung richtet sich nach den jeweils geltenden gesetzlichen Bestimmungen; zwingende gesetzliche Haftung bleibt unberührt. Ein pauschaler Ausschluss sämtlicher Ansprüche wird nicht erklärt.

### Open-Source-Lizenzen

Für Programmcode und Projektdokumentation gelten ausschließlich die im Repository ausgewiesenen Lizenzbedingungen:

- Programmcode: Apache License 2.0.
- Projekttexte und Dokumentation: CC BY-SA 4.0.

Diese Zweckbestimmung fügt den bestehenden Lizenzen keine zusätzliche Nutzungsbeschränkung hinzu und ändert die durch sie eingeräumten Rechte nicht.

## Projektstruktur

- [SYSTEMANWEISUNG.md](SYSTEMANWEISUNG.md) – konsolidierte Arbeits- und Systemanweisung
- [mindmap/MINDMAP_V1.3.md](mindmap/MINDMAP_V1.3.md) – Projekt-Mindmap mit Statuskennzeichnung
- [ROADMAP.md](ROADMAP.md) – Entwicklungsphasen und nächste Schritte
- [CHANGELOG.md](CHANGELOG.md) – nachvollziehbare Änderungen
- [CONTRIBUTING.md](CONTRIBUTING.md) – Regeln für Beiträge
- [SECURITY.md](SECURITY.md) – Hinweise zu Sicherheitsmeldungen
- [docs/ARCHITEKTUR.md](docs/ARCHITEKTUR.md) – technische Zielarchitektur
- [docs/DATENSCHUTZ.md](docs/DATENSCHUTZ.md) – Datenschutzprinzipien und geplante Kontrollen
- [docs/FUNKTIONSSTATUS.md](docs/FUNKTIONSSTATUS.md) – Statusübersicht
- [docs/TECHNISCHE_VORARBEITEN_TERMUX.md](docs/TECHNISCHE_VORARBEITEN_TERMUX.md) – geräte- und systemnahe Arbeiten
- [docs/OCR_TESSERACT_TERMUX.md](docs/OCR_TESSERACT_TERMUX.md) – OCR/Tesseract-Evaluierung
- [docs/BEISPIELFALL_KUECHENERSTAUSSTATTUNG.md](docs/BEISPIELFALL_KUECHENERSTAUSSTATTUNG.md) – textbasierter Übungsfall mit Antrag, Vermieterbestätigung, Ablehnungsbescheid und Widerspruch

## Lizenzen

Das Projekt verwendet bewusst zwei getrennte Lizenzmodelle:

- **Eigener Programmcode:** Apache License 2.0 – siehe [LICENSE-CODE](LICENSE-CODE).
- **Projekttexte und Dokumentation:** Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) – siehe [LICENSE-DOCS.md](LICENSE-DOCS.md).

Die Zuordnung und ihre Grenzen sind in [LICENSE](LICENSE) erklärt. Fremde Bibliotheken, OCR-Sprachdaten, Marken, externe Texte und sonstige Drittinhalte bleiben ihren jeweiligen Rechten und Lizenzbedingungen unterworfen. Die Projektlizenz überträgt keine Rechte, die die Beitragenden nicht selbst besitzen oder lizenzieren dürfen.

## Mitwirkung

Beiträge, technische Prüfungen, Dokumentation, Tests und fachliche Reviews sind willkommen. Vor einer öffentlichen Weitergabe sollen insbesondere Datenschutz, Rechte an eingebundenen Inhalten, Abhängigkeiten und die Lizenzzuordnung geprüft werden. Siehe [CONTRIBUTING.md](CONTRIBUTING.md).

## Leitgedanke

**Student Müller soll ein frei zugängliches digitales Werkzeug für Verständlichkeit, Selbstbestimmung und gesellschaftliche Teilhabe werden.**

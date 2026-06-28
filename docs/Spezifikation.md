# Spezifikation – Word-Lerneinheit Mechatronik

> Maßgebliche fachliche Quelle für das gesamte Projekt (ursprünglich
> `Hermes_Projekt-Prompt.md`). Bei Konflikten gilt dieses Dokument.

## Rolle & Ziel

Vollständige Unterrichtseinheit (ca. 10–12 Stunden), mit der Mechatroniker an einer
Fachschule lernen, ihre wissenschaftliche Projektarbeit in Microsoft Word zu erstellen.
Didaktisches Prinzip: Die Schüler verwandeln einen rohen, unformatierten Fließtext (das
**Handlungsprodukt**) Schritt für Schritt in eine fertig formatierte Projektarbeit,
geführt durch eine interaktive Web-App (**Lernbegleiter**).

Fachthema des Fließtextes: *Potenziale der Künstlichen Intelligenz für die
vorausschauende Instandhaltung (Predictive Maintenance) mechatronischer Anlagen.*

Alle Texte auf Deutsch. Alle Word-Anleitungen mit den **exakten Bezeichnungen der
deutschen Word-Oberfläche** (Registerkarten: Start, Einfügen, Layout,
Referenzen/Verweise, Überprüfen, Ansicht).

## Dateien

```
Projektordner/
├─ Projektarbeit_Rohfassung.docx        (unformatierter Fließtext – für Schüler)
├─ Lernbegleiter.html / index.html      (interaktive App – für Schüler)
├─ Projektarbeit_Musterloesung.docx     (voll formatierte Referenz – für Lehrkraft)
├─ Handreichung_Lehrkraft.md            (didaktische Handreichung)
└─ Material/
   ├─ Abbildung1_PM-Regelkreis.png
   └─ Abbildung2_Schwingungssignal.png
```

## Rohfassung (unformatiert)

Bewusst unformatiert: Standardschrift (Calibri/Arial 11), einfacher Zeilenabstand,
linksbündig, **keine** Formatvorlagen – Überschriften als normaler Text. Drei Platzhalter
in eckigen Klammern markieren Tabelle 1, Abbildung 1, Abbildung 2. Einleitender
HINWEIS-Absatz, dass dies die Rohfassung ist.

### Inhalt (Überschriften als normale Absätze)

**Titelblock:** „Potenziale der Künstlichen Intelligenz für die vorausschauende
Instandhaltung mechatronischer Anlagen" / „Projektarbeit im Rahmen der Fachschule für
Mechatronik" / Vorgelegt von: Max Mustermann, Fachschule Mechatronik, Klasse FM-2 /
Musterstadt, den TT.MM.JJJJ / Betreuende Lehrkraft: Herr Schwibach.

**1 Einleitung**
- **1.1 Problemstellung** – Mechatronische Anlagen (Mechanik + Elektrik + IT) als Rückgrat
  der Fertigung; unerwartete Ausfälle = hohe Kosten; reaktive Instandhaltung greift zu
  spät, präventive tauscht funktionsfähige Teile; daher Predictive Maintenance.
- **1.2 Zielsetzung** – Potenziale der KI für Predictive Maintenance untersuchen:
  Sensordatenauswertung zur Früherkennung, wirtschaftliche Chancen, Grenzen.
- **1.3 Aufbau der Arbeit** – Kap. 2 Grundlagen, Kap. 3 Funktionsprinzip/Sensorik/
  Datenauswertung, Kap. 4 Potenzialanalyse mit Praxisbeispiel, Kap. 5 Fazit/Ausblick.

**2 Grundlagen**
- **2.1 Mechatronische Anlagen und Instandhaltung** – Begriff Mechatronik; Aufbau aus
  Aktoren, Sensoren, Steuerung, mechanischen Bauteilen (Wälzlager, Getriebe, Antriebe);
  Instandhaltung nach DIN 31051 (Wartung, Inspektion, Instandsetzung, Verbesserung).
- **2.2 Wartungsstrategien** – reaktiv / präventiv / vorausschauend; Verweis auf Tabelle.
  `[HIER TABELLE 1 EINFÜGEN: Vergleich der Wartungsstrategien. Spalten: Strategie | Auslöser | Vorteil | Nachteil. Zeilen: Reaktiv – Ausfall des Bauteils – geringe Planungskosten – ungeplante Stillstände; Präventiv – festes Zeitintervall – planbar, geringeres Ausfallrisiko – Austausch funktionsfähiger Teile; Vorausschauend – realer Anlagenzustand – bedarfsgerecht, hohe Verfügbarkeit – hoher Aufwand für Sensorik und IT]`
- **2.3 Künstliche Intelligenz und maschinelles Lernen** – KI/ML, Anomalieerkennung und
  Zustandsklassifikation; Training mit historischen Sensordaten.

**3 Vorausschauende Instandhaltung in der Mechatronik**
- **3.1 Funktionsprinzip** – geschlossener Regelkreis Sensoren → Vorverarbeitung →
  KI-Analyse → Restnutzungsdauer-Prognose → Wartungsplanung. Verweis auf Abbildung.
  `[HIER ABBILDUNG 1 EINFÜGEN: Datei Abbildung1_PM-Regelkreis.png – Schematische Darstellung des Predictive-Maintenance-Regelkreises]`
- **3.2 Sensorik und Datenerfassung** – Messgrößen (Schwingung, Temperatur, Strom, Druck,
  Geräusch); Schwingungsanalyse; Beispiel Wälzlager (gesund vs. periodische Stoßimpulse).
  `[HIER ABBILDUNG 2 EINFÜGEN: Datei Abbildung2_Schwingungssignal.png – Vergleich des Schwingungssignals eines gesunden und eines geschädigten Wälzlagers]`
- **3.3 KI-gestützte Datenauswertung** – Merkmalsextraktion, Mustervergleich, Warnung +
  Restnutzungsdauer.

**4 Potenzialanalyse**
- **4.1 Praxisbeispiel CNC-Bearbeitungszentrum** – Schwingungs-/Stromsensoren an Spindel/
  Antrieben; Spindellager-Verschleiß früh erkennen, Austausch in geplante Stillstandszeit.
- **4.2 Wirtschaftliche Potenziale** – weniger Stillstände, höhere Verfügbarkeit, optimale
  Lebensdauer, geringere Material-/Personalkosten.
- **4.3 Grenzen und Herausforderungen** – Investitionen, Datenmenge/-qualität (seltene
  Schadensfälle), Qualifikation, Datensicherheit/Datenschutz.

**5 Fazit und Ausblick** – erhebliche Potenziale; Voraussetzungen Sensorik/Datenbasis/
Personal; Ausblick bessere Sensoren, günstigere Vernetzung, bessere KI, auch für KMU.

**Literaturverzeichnis** (handgetippt, wird in Stufe 8 durch automatisches Verzeichnis
ersetzt): DIN 31051 (Beuth, 2019); Mustermann, M. (2024): Industrie 4.0 und
vorausschauende Instandhaltung; Beispiel, A. (2023): Maschinelles Lernen in der Produktion.

## Lernbegleiter (index.html / Lernbegleiter.html)

Eine einzelne, eigenständige HTML-Datei (CSS+JS inline, keine externen Abhängigkeiten,
offline lauffähig). Funktionsumfang: Namenseingabe, Fortschrittsbalken (x von 11),
Stepper mit Status erledigt/aktiv/gesperrt; Stufen werden nacheinander freigeschaltet
(nächste erst nach Abhaken aller Erfolgskriterien + Abschluss). Jede Stufe: Auftrag,
nummerierte Anleitung (deutsche Word-Menüs), Erfolgskriterien als Checkboxen,
aufklappbarer Tipp und Musterlösung/Kontrolle, Button „Stufe abschließen & Feedback".
Chiffre-Funktion (JSON → Base64, unicodefest), „Chiffre erzeugen", „Als Link kopieren"
(Deeplink `?code=`), „Laden"; Autospeichern in `localStorage`.

### Die 11 Stufen (Reihenfolge fix)

1. **Dokument einrichten** – Seitenränder Normal/2,5 cm, einheitliche Schrift, Zeilenabstand 1,5, Blocksatz, opt. Silbentrennung.
2. **Überschriften & Formatvorlagen** – „Überschrift 1" für Kapitel, „Überschrift 2" für Unterkapitel; Hinweis-Absatz löschen. (Schlüsselstufe fürs Inhaltsverzeichnis.)
3. **Deckblatt** – eigene erste Seite (Titel, Name, Klasse, Betreuer, Ort/Datum), Seitenumbruch, ohne Überschrift-Formatvorlage.
4. **Automatisches Inhaltsverzeichnis** – nach Deckblatt, Referenzen → Inhaltsverzeichnis → Automatische Tabelle; aktualisierbar.
5. **Kopf-/Fußzeile & Seitenzahlen** – Seitenzahlen in Fußzeile, „Erste Seite anders" (Deckblatt ausnehmen), opt. Kopfzeile.
6. **Bilder & Abbildungsverzeichnis** – beide Platzhalter durch PNGs ersetzen, beschriften (Beschriftung einfügen → „Abbildung"), Abbildungsverzeichnis.
7. **Tabelle** – Tabellen-Platzhalter durch formatierte 4×4-Tabelle, Tabellenformatvorlage, Beschriftung „Tabelle 1".
8. **Quellen & Literaturverzeichnis** – ≥3 Quellen im Quellen-Manager, ≥1 Verweis, automatisches Literaturverzeichnis ersetzt die handgetippte Liste; Zitierformat wählen.
9. **Kommentar fürs Review** – Stelle markieren, „Überprüfen → Neuer Kommentar" mit konkreter Frage, speichern und abgeben. (Lehrkraft lässt KI-Assistenten die Kommentare beantworten.)
10. **Überarbeiten** – „Änderungen nachverfolgen", Rückmeldungen einarbeiten, Kommentare als gelöst markieren.
11. **Endkontrolle & PDF** – alle Felder aktualisieren (Strg+A, F9), Rechtschreibung, Layout (keine Platzhalter), PDF-Export.

Startseite vor Stufe 1 (Ablauf + Namenseingabe); Abschluss-/Glückwunschseite mit
Kompetenzliste nach Stufe 11.

## Abbildungen (Material/)

- **Abbildung1_PM-Regelkreis.png:** geschlossener Regelkreis mit 6 Stationen
  (Sensorik → Datenerfassung/Vorverarbeitung → KI-Analyse → Zustandsprognose →
  Wartungsplanung → Mechatronische Anlage → zurück), Mitte „Geschlossener Regelkreis".
- **Abbildung2_Schwingungssignal.png:** zwei Diagramme „Beschleunigung (g)" über „Zeit (ms)":
  oben gleichmäßiges Signal („Gesundes Wälzlager"), unten mit periodischen Stoßimpulsen
  („Geschädigtes Wälzlager"). Erzeugung z. B. mit Python/matplotlib, ~150 dpi.

## Musterlösung & Handreichung

- **Musterlösung:** voll formatierte Referenz des Fließtextes (Deckblatt, automatisches
  Inhalts-/Abbildungs-/Tabellenverzeichnis, Ü1/Ü2-Formatvorlagen, Kopf-/Fußzeile mit
  Seitenzahl außer Deckblatt, eingebundene/beschriftete Abbildungen, formatierte Tabelle,
  Blocksatz, 1,5 Zeilenabstand).
- **Handreichung_Lehrkraft.md:** Konzept, Dateiübersicht, Lernziele, Stundenplanung
  (~10–12 Std), Chiffre-Erklärung, Review-Schleife (Stufe 9) inkl. Beispiel-Prompt für den
  KI-Assistenten, Differenzierung, Bewertungsraster (100 Punkte), Stolpersteine.

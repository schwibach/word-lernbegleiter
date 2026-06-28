# AGENTS.md — Word-Lernbegleiter (Mechatronik)

> Kontext- und Arbeitsanweisung für KI-Agenten (Codex u. a.), die an diesem Repo
> weiterarbeiten. **Zuerst lesen.** Maßgebliche fachliche Quelle:
> [`docs/Spezifikation.md`](docs/Spezifikation.md).

## Worum es geht

Eine Unterrichtseinheit (ca. 10–12 Std.) für Mechatroniker an einer Fachschule.
Die Schüler verwandeln einen rohen, unformatierten Word-Fließtext Schritt für Schritt
in eine fertig formatierte wissenschaftliche Projektarbeit. Geführt werden sie durch
den **Lernbegleiter** – eine eigenständige Single-File-Web-App mit 11 aufeinander
aufbauenden Stufen (Layout, Formatvorlagen, Deckblatt, Inhaltsverzeichnis, Seitenzahlen,
Bilder/Abbildungsverzeichnis, Tabellen, Quellen, Kommentar-Review, Überarbeiten, PDF).

Fachthema des Fließtextes: *Potenziale der KI für die vorausschauende Instandhaltung
(Predictive Maintenance) mechatronischer Anlagen.*

## Dieses Repo / Deployment

- **`index.html`** — der komplette Lernbegleiter (CSS+JS inline, keine externen
  Abhängigkeiten, offline per Doppelklick lauffähig). **Das ist die Hauptdatei.**
- Veröffentlicht über **GitHub Pages**: https://schwibach.github.io/word-lernbegleiter/
- Push auf `main` → Pages deployt automatisch neu. Vor dem Push lokal testen
  (einfach `index.html` im Browser öffnen oder `python -m http.server`).

## Weitere Projektdateien (NICHT in diesem Repo)

Liegen im SharePoint-Team **Unterricht** unter `General/Word/`:

| Datei | Zweck |
|---|---|
| `Projektarbeit_Rohfassung.docx` | unformatierter Fließtext mit 3 Platzhaltern – für Schüler |
| `Projektarbeit_Musterloesung.docx` | voll formatierte Referenz – für Lehrkraft |
| `Handreichung_Lehrkraft.md` | Didaktik, Stundenplanung, Bewertungsraster |
| `Material/Abbildung1_PM-Regelkreis.png`, `Abbildung2_Schwingungssignal.png` | Abbildungen |

Wichtig: Eine **Kopie** der `index.html` liegt dort als `Lernbegleiter.html` für die
Schüler-Verteilung. **Beide Orte synchron halten**, wenn der Lernbegleiter geändert wird.

## Konventionen (zwingend)

- Alle Texte auf **Deutsch**; Word-Anleitungen mit den **exakten deutschen
  Menübezeichnungen** (Start, Einfügen, Layout, Referenzen/Verweise, Überprüfen, Ansicht).
- Die **Rohfassung bleibt unformatiert** (Standardschrift, keine Formatvorlagen,
  Überschriften als normaler Text) und behält die drei eckigen Platzhalter
  (Tabelle 1, Abbildung 1, Abbildung 2).
- Die **Musterlösung** ist die formatierte Gegenprobe und muss inhaltlich zur Rohfassung passen.
- Bei Änderungen an Thema, Fließtext oder Stufen **alle betroffenen Dateien gemeinsam
  aktualisieren** (Rohfassung, Lernbegleiter/index.html, Musterlösung, Handreichung).
- Lernbegleiter: Fortschritt via `localStorage` + **Chiffre** (Zustand JSON → Base64).
  Unicodefest kodieren mit `btoa(unescape(encodeURIComponent(json)))` und Gegenrichtung.
  Deeplink-Parameter `?code=` beim Laden auslesen. Den „Als Link kopieren"-Link aus
  `location.href.split(/[?#]/)[0]` bauen (nicht aus `location.origin+pathname` – sonst
  bricht der Link beim Offline-Öffnen in manchen Browsern).

## Aktueller Stand (2026-06-28)

- Lernbegleiter vollständig getestet (Logik + Browser-Durchlauf), alle 11 Stufen
  freischaltbar, Chiffre/Deeplink funktionieren, Deeplink-Robustheits-Fix angewendet.
- Live auf GitHub Pages, SharePoint-Kopie wird vom Nutzer synchronisiert.

## Mögliche nächste Schritte

- Download-Links (Rohfassung, Material) direkt in die Live-Seite einbauen, damit die
  Seite ohne SharePoint nutzbar ist.
- Stufen erweitern (automatische Kapitelnummerierung, Querverweise, Fußnoten).
- Differenzierungs-/Zusatzaufgaben in den Lernbegleiter einbauen.
- Schullogo/echtes Deckblatt-Design ergänzen.
- Bewertungsbogen als eigene Druckvorlage erzeugen.
- Thema/Schwierigkeit auf einen anderen Mechatronik-Kontext anpassen.

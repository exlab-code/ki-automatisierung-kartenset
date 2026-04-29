# KI Automatisierung — Kartenset

Workshop-Material zum Thema **Prozess-Automatisierung mit Sprachmodellen (KI / LLMs)** für AWO und vergleichbare soziale Träger.

Das Kartenset hilft Teams dabei, ihre eigenen Prozesse so zu zerlegen, dass klar wird, **wo ein Sprachmodell sinnvoll Arbeit übernehmen kann** — und wo Mensch, Datenschutz oder Risiko die Grenze ziehen.

> **Umbrella-These:** KI ist ein Sprachmodell — gut in bestimmten sprachlichen Aufgaben. Wer das versteht, kann es im Alltag systematisch einsetzen — und dadurch im großen Maßstab Wert schaffen.

## Workshop-Kontext

Entworfen für das **AWO Führungskräfte Forum am 27. April 2026**.

Ziel des Workshops:

- **Klarheit schaffen**, was ein Sprachmodell operativ tatsächlich leisten kann — und was nicht.
- **Prozesse identifizieren**, die sich im AWO-Alltag mit KI sinnvoll automatisieren lassen — und solche, die es nicht tun sollten.
- **Gemeinsam zerlegen**: Auslöser, Sprach-Operation, Ausgabe, Mensch im Loop, Bedenken — Karte für Karte aufs Brown Paper, Pfeile dazwischen.

## Live-Version

Die Druckversion läuft direkt im Browser via GitHub Pages:
**[https://exlab-code.github.io/ki-automatisierung-kartenset/](https://exlab-code.github.io/ki-automatisierung-kartenset/)**

Filtern nach Kategorie, Auswahl drucken (4 Karten pro A4-Seite) — keine Installation nötig.

## Aufbau des Sets

Sechs Kategorien, jede mit eigenem Farbcode:

| Kategorie | Bedeutung |
|-----------|-----------|
| **Start** | Wie der Prozess ausgelöst wird (E-Mail, Datenexport, Web-Scraping, …) |
| **Sprachmodell** | Was das Modell mit dem Eingang macht — die eigentliche Sprach-Operation |
| **Ausgabe** | Wohin das Ergebnis geht (Mail, PDF, Datenbank, Fachsoftware, …) |
| **Mensch** | Wo Menschen im Prozess bleiben müssen (Prüfen, Entscheiden, Eskalieren, Dokumentieren) |
| **Bedenken** | Inhalt-/Daten-Risiken (Schweigepflicht, Halluzination, Bias, sensible Inhalte) |
| **Hinweis** | Workshop-Meta (Verbindungen & Logik aufs Brown Paper zeichnen) |

Verbindungen zwischen Karten — Bedingungen, Filter, Wiederholungen, Wartezeiten, Fehlerfälle — werden direkt mit Pfeilen aufs Brown Paper gezeichnet. Sie sind keine eigenen Karten.

## Eigene Version: Forken & Anpassen

Wenn du das Set für deinen Träger, dein Team oder einen spezifischen Workshop anpassen willst:

1. **Repo forken** (Button oben rechts auf GitHub)
2. **GitHub Pages aktivieren** in deinem Fork:
   - Settings → Pages
   - Source: `Deploy from a branch`, Branch: `main`, Folder: `/ (root)`
3. **Karten bearbeiten** in `content/*.md` — entweder direkt im GitHub-Web-Editor oder lokal
4. **Commit / Push** — GitHub Pages baut den Fork automatisch neu, deine angepasste Version ist unter `https://<dein-user>.github.io/ki-automatisierung-kartenset/` erreichbar

### Karten-Format

Jede Datei in `content/` ist eine Kategorie. Format:

```markdown
# Kategoriename

Optionale Beschreibung der Kategorie.

## Kartentitel
Beschreibung der Karte (eine Zeile, ein Absatz).

## Nächster Kartentitel
Nächste Beschreibung.

## (eigene Idee)
```

- `# Überschrift` — Kategoriename (wird beim Rendering ignoriert, dient zur Orientierung)
- `## Überschrift` — Kartentitel
- Absatz danach — Beschreibung
- `## (eigene Idee)` — leere Karte zum Beschriften im Workshop

Karten erscheinen auf der Webseite in derselben Reihenfolge, in der sie in der MD-Datei stehen.

### Neue Kategorie hinzufügen

Erfordert Änderungen in `index.html`:

1. Neue Datei `content/<name>.md` anlegen
2. In `index.html` den `CATEGORIES`-Array, `LABELS`, `ICONS`, `COLORS` und CSS-Regeln (`cat-NEU`) erweitern
3. Falls gewünscht, Filter-Button im Toolbar ergänzen

## Lokal testen

Browser blockieren `fetch()` aus `file://`-URLs. Daher zum lokalen Testen einen kleinen Server starten:

```bash
cd ki-automatisierung-kartenset
python3 -m http.server 8000
```

Dann [http://localhost:8000](http://localhost:8000) öffnen.

## Drucken

- Karten sind im Format **A6** (105 × 148.5 mm) — vier Karten pro A4-Seite
- Im Toolbar: gewünschte Kategorie im Dropdown auswählen → "Drucken (4 pro Seite)"
- Im Druckdialog: A4 Hochformat, Ränder auf 0 oder "Tatsächliche Größe"
- Nach dem Drucken am Schnittlinien-Raster trennen

## Lizenz

[**CC BY-SA 4.0**](LICENSE) — Creative Commons Namensnennung – Weitergabe unter gleichen Bedingungen 4.0 International.

Du darfst das Material teilen, anpassen und kommerziell nutzen, solange du

- die Urheber:innen nennst,
- Änderungen kenntlich machst,
- dein Werk unter derselben Lizenz weitergibst.

## Mitwirken

Pull Requests willkommen, besonders für:

- Verbesserungen der Kartentexte (klarer, präziser, kürzer)
- Neue Bedenken-Karten für Sektor-spezifische Risiken
- Übersetzungen
- Workshop-Erfahrungsberichte (was hat funktioniert, was nicht)

Issues für Diskussionen über Inhalt und Format gerne aufmachen.

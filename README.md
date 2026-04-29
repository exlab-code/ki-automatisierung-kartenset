# KI Automatisierung — Kartenset

Werkzeug für Workshops zum Thema **Prozess-Automatisierung mit Sprachmodellen** für AWO und vergleichbare soziale Träger.

Das Kartenset hilft Teams dabei, ihre eigenen Prozesse so zu zerlegen, dass klar wird, **wo ein Sprachmodell sinnvoll Arbeit übernehmen kann** — und wo Mensch, Datenschutz oder Risiko die Grenze ziehen.

> **Leitgedanke:** KI ist ein Sprachmodell — gut in bestimmten sprachlichen Aufgaben. Wer das versteht, kann es im Alltag systematisch einsetzen — und dadurch im großen Maßstab Wert schaffen.

## Workshop-Kontext

Entworfen für das **AWO Führungskräfte Forum am 27. April 2026**.

Ziele des Workshops:

- **Klarheit schaffen**, was ein Sprachmodell operativ tatsächlich leisten kann — und was nicht.
- **Prozesse identifizieren**, die sich im AWO-Alltag mit KI sinnvoll automatisieren lassen — und solche, die es nicht tun sollten.
- **Gemeinsam zerlegen**: Auslöser, Datenquelle, Sprach-Operation, Ausgabe, Mensch im Loop, Bedenken — Karte für Karte aufs Brown Paper, Pfeile dazwischen.

Ausführliches Workshop-Format mit Ablauf, Materialien und Hintergrund: **[WORKSHOP.md](WORKSHOP.md)**.

## Online-Version

Die Druckversion läuft direkt im Browser über GitHub Pages:
**[exlab-code.github.io/ki-automatisierung-kartenset](https://exlab-code.github.io/ki-automatisierung-kartenset/)**

Nach Kategorie filtern, Auswahl drucken (4 Karten pro A4-Seite) — keine Installation nötig.

## Aufbau des Sets

Acht Kategorien, jede mit eigenem Farbcode:

| Kategorie | Bedeutung |
|-----------|-----------|
| **Cover** | Titelkarte mit Lizenz und Mitwirken-Hinweis |
| **Start** | Wann läuft der Prozess los? (E-Mail, Formular, Sprachaufnahme, Zeitpunkt, …) |
| **Input** | Welche Daten braucht das Modell? (Datenbank, Tabelle, Wissensbasis, API, …) |
| **Sprachmodell** | Was das Modell mit dem Eingang macht — die eigentliche Sprach-Operation |
| **Ausgabe** | Wohin das Ergebnis geht (Mail, PDF, Datenbank, Fachsoftware, …) |
| **Mensch** | Wo Menschen im Prozess bleiben müssen (Prüfen, Entscheiden, Eskalieren, Dokumentieren) |
| **Bedenken** | Inhalt- und Datenrisiken (Schweigepflicht, Halluzination, Bias, sensible Inhalte) |
| **Hinweis** | Workshop-Meta (Verbindungen & Logik werden direkt aufs Brown Paper gezeichnet) |

Verbindungen zwischen Karten — Bedingungen, Filter, Wiederholungen, Wartezeiten, Fehlerfälle — werden direkt mit Pfeilen aufs Brown Paper gezeichnet. Sie sind keine eigenen Karten.

## Eigene Version: Forken & Anpassen

Wer das Set für den eigenen Träger, das eigene Team oder einen spezifischen Workshop anpassen möchte:

1. **Repository forken** (Button oben rechts auf GitHub)
2. **GitHub Pages aktivieren** im eigenen Fork:
   - Settings → Pages
   - Source: `Deploy from a branch`, Branch: `main`, Folder: `/ (root)`
3. **Karten bearbeiten** in `content/*.md` — entweder direkt im GitHub-Web-Editor oder lokal
4. **Speichern und pushen** — GitHub Pages baut den Fork automatisch neu, die angepasste Version ist unter `https://<dein-user>.github.io/ki-automatisierung-kartenset/` erreichbar

### Karten-Format

Jede Datei in `content/` ist eine Kategorie. Format:

```markdown
# Kategoriename

Optionale Beschreibung der Kategorie.

## Kartentitel
Beschreibung der Karte. Längere Beschreibungen mit Leerzeile als Absatz-Trenner.

## Nächster Kartentitel
Nächste Beschreibung.

## (eigene Idee)
```

- `# Überschrift` — Kategoriename (wird beim Rendern übersprungen, dient zur Orientierung)
- `## Überschrift` — Kartentitel
- Absatz danach — Beschreibung (Leerzeile = neuer Absatz)
- `## (eigene Idee)` — leere Karte zum Beschriften im Workshop

Karten erscheinen auf der Webseite in derselben Reihenfolge, in der sie in der MD-Datei stehen.

### Neue Kategorie hinzufügen

Erfordert Änderungen in `index.html`:

1. Neue Datei `content/<name>.md` anlegen
2. In `index.html` die Variablen `CATEGORIES`, `LABELS`, `ICONS`, `COLORS` und die CSS-Regeln (`cat-NEU`) erweitern
3. Bei Bedarf Filter-Schaltfläche in der Werkzeugleiste ergänzen

## Lokal testen

Browser blockieren `fetch()` aus `file://`-URLs. Zum lokalen Testen daher einen kleinen Server starten:

```bash
cd ki-automatisierung-kartenset
python3 -m http.server 8000
```

Dann [http://localhost:8000](http://localhost:8000) öffnen.

## Drucken

- Karten sind im Format **A6** (105 × 148,5 mm) — vier Karten pro A4-Seite
- In der Werkzeugleiste: gewünschte Kategorie im Auswahlmenü wählen → „Drucken (4 pro Seite)"
- Im Druckdialog: A4 Hochformat, Ränder auf 0 oder „Tatsächliche Größe"
- Nach dem Drucken entlang des Rasters auseinanderschneiden

## Lizenz

[**CC BY-SA 4.0**](LICENSE) — Creative Commons Namensnennung – Weitergabe unter gleichen Bedingungen 4.0 International.

Das Material darf geteilt, angepasst und auch kommerziell genutzt werden, solange

- die Urheber:innen genannt werden,
- Änderungen kenntlich gemacht werden,
- das eigene Werk unter derselben Lizenz weitergegeben wird.

## Mitwirken

Verbesserungsvorschläge sind willkommen, besonders für:

- Klarere, präzisere oder kürzere Kartentexte
- Neue Bedenken-Karten für sektorspezifische Risiken
- Übersetzungen
- Erfahrungsberichte aus durchgeführten Workshops (was hat funktioniert, was nicht)

Pull Requests und Issues zur Diskussion über Inhalt und Format gerne direkt im Repository öffnen — auch ohne Code-Kenntnisse über den GitHub-Web-Editor möglich.

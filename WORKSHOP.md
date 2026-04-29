# Prozess-Baukasten

## Ein Workshop-Format zur Identifikation und Modellierung von Textprozess-Automatisierung mit Sprachmodellen

---

## Worum es geht

In den meisten Organisationen steckt ein erstaunlich großer Teil der täglichen Arbeit in Textverarbeitung: E-Mails lesen und beantworten, Berichte schreiben, Protokolle erstellen, Informationen aus Dokumenten heraussuchen, Texte von einer Form in eine andere bringen. Vieles davon ist wiederholend, zeitaufwendig und folgt immer ähnlichen Mustern.

Sprachmodelle — die Technologie hinter Werkzeugen wie ChatGPT, Claude oder Copilot — können einen Teil dieser Textarbeit übernehmen. Nicht alles, aber einen relevanten Teil. Die Herausforderung für die meisten Organisationen ist nicht die Technologie selbst, sondern die Frage davor: *Wo in unseren Abläufen steckt überhaupt die Textarbeit, die sich sinnvoll automatisieren ließe?*

Dieser Workshop hilft Teams und Führungskräften, genau diese Frage zu beantworten — ohne technisches Vorwissen, ohne Tools, ohne Implementierungsdruck. Am Ende steht kein fertiges System, sondern ein gemeinsam erarbeitetes Modell eines konkreten Prozesses aus dem eigenen Arbeitsalltag.

---

## Der Ansatz

### Sprachmodelle als Textmaschinen verstehen

Der Workshop beginnt mit einer bewussten Entmystifizierung. Statt über „Künstliche Intelligenz" zu sprechen, verwenden wir den präziseren Begriff *Sprachmodell* — weil er beschreibt, was die Technologie tatsächlich ist: ein Modell, das mit Sprache arbeitet.

Ein Sprachmodell ist eine Textmaschine. Es nimmt Text in einer Form entgegen und gibt Text in einer anderen Form zurück. Nicht mehr, aber auch nicht weniger. Diese einfache Beschreibung ist keine Vereinfachung — sie ist das tatsächliche Funktionsprinzip, das auch der akademischen Forschung zugrunde liegt (Raffel et al., 2020: „Every task we consider is cast as feeding our model text as input and training it to generate some target text").

Aus diesem Prinzip leiten sich vier Grundoperationen ab, die Sprachmodelle zuverlässig beherrschen:

**Reduzieren** — aus viel Text wird wenig. Zusammenfassen, die Kernaussagen herausarbeiten, auf eine bestimmte Länge bringen. Das ist die robusteste Fähigkeit, weil das Modell nichts erfinden muss, sondern nur auswählen.

**Umformen** — der Inhalt bleibt gleich, die Form ändert sich. Fachsprache wird einfache Sprache, Deutsch wird Türkisch, Stichpunkte werden Fließtext, ein förmlicher Ton wird freundlich. Auch hier arbeitet das Modell an vorhandenem Material entlang.

**Extrahieren** — strukturierte Information wird aus unstrukturiertem Text gezogen. Fristen, Namen, Zuständigkeiten, Beträge aus einem Fließtext herausfiltern. Besonders stark, wenn die Information im Text steht und nur gefunden werden muss.

**Sortieren** — Text wird in Kategorien eingeordnet. Dringend oder nicht dringend, Beschwerde oder Anfrage, Zuständigkeit A oder B. Funktioniert zuverlässig, wenn die Kategorien klar definiert sind.

Ebenso wichtig ist die Benennung der Grenzen: Sprachmodelle können nicht entscheiden, nicht verantworten, und keine Beziehungsarbeit leisten. Sie schreiben Entwürfe, keine Bescheide. Sie sortieren vor, sie entscheiden nicht. In Organisationen, deren Kernkompetenz die Arbeit mit Menschen ist, ist diese Unterscheidung keine Einschränkung, sondern die zentrale Design-Regel.

### Prozesse sichtbar machen, die unsichtbar geworden sind

Die größte Hürde bei der Identifikation von Automatisierungspotenzial ist nicht technisches Wissen, sondern Betriebsblindheit. Die mühsamsten Textprozesse sind oft die unsichtbarsten, weil sie so alltäglich sind, dass niemand sie mehr als „Prozess" wahrnimmt.

Der Workshop nutzt gezielte Brainstorming-Impulse, um diese unsichtbaren Routinen sichtbar zu machen. Zwei Leitfragen haben sich als besonders produktiv erwiesen:

*Wo lesen wir viel, um wenig rauszuziehen?* — Diese Frage findet Prozesse, in denen Text konsumiert wird: lange Dokumente durcharbeiten, Informationen suchen, Relevantes vom Irrelevanten trennen.

*Wo schreiben oder tippen wir immer wieder fast das Gleiche?* — Diese Frage findet Prozesse, in denen Text produziert wird: Berichte nach Vorlage, Standardantworten, wiederkehrende Dokumentation.

Beide Fragen sind absichtlich in Alltagssprache formuliert, nicht in technischer Fachsprache. Sie funktionieren ohne jedes Vorwissen über Sprachmodelle — und genau das ist der Punkt: die Teilnehmenden sollen ihre eigene Arbeitswelt durchsuchen, nicht über Technologie nachdenken.

### Prozesse modellieren statt diskutieren

Das Herzstück des Workshops ist eine Gruppenarbeit mit einem physischen Kartensystem — dem Prozess-Baukasten. Statt über Automatisierung zu reden, bauen die Teilnehmenden einen konkreten Prozess aus vorbereiteten Karten auf Brown Paper zusammen.

Die Karten sind in sechs Kategorien organisiert, die zusammen die Grammatik eines automatisierten Ablaufs bilden:

**Start** (blau) — Was löst den Prozess aus? Eine eingehende E-Mail, ein Stichtag, ein Dokumenten-Upload, eine Sprachaufnahme.

**Input** (türkis) — Welche Daten braucht das Modell zusätzlich, um die Aufgabe gut zu erledigen? Datenbank-Abfragen, Tabellen, Wissensbasis, bestehende Akten, API-Aufrufe.

**Sprachmodell** (grün) — Was macht das Sprachmodell mit dem Text? Zusammenfassen, übersetzen, extrahieren, kategorisieren, umformulieren. Hier steckt die eigentliche Inspiration: die Teilnehmenden blättern durch die grünen Karten und entdecken Operationen, an die sie vorher nicht gedacht haben.

**Ausgabe** (orange) — Wo geht das Ergebnis hin? Per Mail versenden, als PDF erzeugen, in eine Fachsoftware oder Datenbank eintragen, auf einer Website veröffentlichen.

**Mensch** (lila) — Wo greift ein Mensch ein? Prüfen und Korrigieren, Entscheiden und Freigeben, Eskalieren bei Risiko, Begründungen dokumentieren. Die Design-Regel lautet: mindestens eine lila Karte muss in jeden Prozess.

**Bedenken** (gelb) — Wo gibt es Risiken? Personenbezogene Daten, Schweigepflicht, Halluzination, Bias, sensible Inhalte, Transparenz. Diese Karten werden als letztes auf die fertige Pipeline gelegt — als Realitäts-Overlay.

Hinzu kommen zwei Meta-Karten: eine **Cover-Karte** als Titelkarte des Sets (mit Lizenz und Mitwirken-Hinweis) und eine **Hinweis-Karte**, die erklärt, dass Verbindungen zwischen den Karten — Bedingungen, Filter, Wiederholungen, Wartezeiten, Fehlerfälle — direkt mit Pfeilen aufs Brown Paper gezeichnet werden, statt eigene Karten zu sein. Diese bewusste Entscheidung hält die Karten konzeptionell fokussiert (jede Karte = ein Baustein) und nutzt die Stärke des Brown Paper aus (Verbindungslinien sind dort ohnehin am natürlichsten).

Jede Karte hat einen farbigen Header mit Kategorie und Icon und einen Aktionsnamen mit kurzer Erklärung. Auf dem Brown Paper notieren die Teilnehmenden neben oder unter der Karte (auf einem Post-it oder direkt auf dem Papier), was bei *ihrem* konkreten Prozess passiert — z.B. neben der grünen „Zusammenfassen"-Karte: „Sitzungsprotokoll auf 5 Punkte kürzen". Dadurch wird aus einer generischen Karte eine spezifische. Pro Hauptkategorie liegt zusätzlich eine **Blanko-Karte** („eigene Idee") bei, falls eine wichtige Operation oder Quelle im Set fehlt und ergänzt werden soll.

Das Brown Paper zeigt am Ende nicht ein abstraktes Modell, sondern *ihren* Prozess.

Die physische Arbeit mit Karten hat gegenüber einer Diskussion oder einer digitalen Übung mehrere Vorteile: sie zwingt zu Konkretisierung (man muss eine Karte wählen, nicht nur reden), sie macht die Struktur sichtbar (die Pipeline liegt vor einem), sie ermöglicht Umsortierung (Karten verschieben ist leichter als Sätze umschreiben), und sie erzeugt ein fotografierbares Ergebnis, das nach dem Workshop weiterlebt.

### Zwei Denkphasen bewusst trennen

Der Workshop trennt zwei Denkphasen, die in der Praxis oft vermischt werden und sich dann gegenseitig blockieren:

**Phase 1: Was wäre möglich?** — Die Teilnehmenden modellieren ihren Prozess optimistisch: wie sähe der Ablauf aus, wenn ein Sprachmodell die Textarbeit übernähme? Keine Einschränkungen, keine Bedenken, nur die Frage nach dem Potenzial.

**Phase 2: Was müssen wir beachten?** — Erst wenn die Pipeline steht, kommen die gelben Bedenken-Karten ins Spiel. Datenschutz, Schweigepflicht, Halluzination, Bias, sensible Inhalte — alles legitime Einwände, aber sie kommen *nach* dem kreativen Entwurf, nicht davor. Diese Reihenfolge verhindert, dass Bedenken die Ideenfindung ersticken, ohne die Bedenken zu entwerten.

---

## Workshop-Ablauf

Der Workshop ist in drei Bewegungen strukturiert, die insgesamt etwa 90 Minuten dauern. Die Zeitangaben sind Richtwerte — je nach Gruppengröße und Diskussionsfreude können die Phasen kürzer oder länger ausfallen.

### Bewegung 1 — Orientierung

Dauer: ca. 20 Minuten

Die Teilnehmenden erhalten ein gemeinsames mentales Modell: Was ist ein Sprachmodell, was kann es, was kann es nicht. Dieser Teil ist der einzige Vortragsteil im Workshop. Er sollte knapp, anschaulich und ehrlich sein — insbesondere bei den Grenzen. Wenn möglich, unterstützt durch eine kurze Live-Demonstration, die zeigt, wie eine Texttransformation in der Praxis aussieht.

Ziel: Alle Teilnehmenden können nach diesem Block den Satz vervollständigen: „Ein Sprachmodell nimmt Text in einer Form und gibt Text in einer anderen Form zurück."

### Bewegung 2 — Erkundung und Modellierung

Dauer: ca. 50 Minuten

Der Hauptteil, unterteilt in drei Schritte:

**Schritt 1: Einzelarbeit.** Jede Person identifiziert für sich einen textlastigen Prozess aus dem eigenen Arbeitsalltag, unterstützt durch ein Brainstorming-Worksheet mit Impulsfragen. Stille Phase, ca. 15 Minuten. Am Ende hat jede:r einen Kandidaten, den sie in die Gruppe mitbringt.

**Schritt 2: Prozess auswählen.** In Gruppen von 3–4 Personen stellt jede:r kurz den eigenen Kandidaten vor. Die Gruppe wählt einen Prozess nach drei Kriterien aus: Mehrere kennen ihn, es wird dabei Text verarbeitet (nicht nur geschrieben oder gelesen), und es ist klar, wo der Prozess anfängt und aufhört.

**Schritt 3: Prozess modellieren.** Die Gruppe baut den gewählten Prozess mit den Baukasten-Karten auf Brown Paper: Start → Input → Sprachmodell → Ausgabe, mit Mensch-Karten an den richtigen Stellen und Pfeilen für die Verbindungen (Bedingungen, Wiederholungen, Wartezeiten, Fehlerfälle). Am Ende werden die gelben Bedenken-Karten als Overlay aufgelegt.

### Bewegung 3 — Einordnung

Dauer: ca. 20 Minuten

Jede Gruppe stellt kurz ihren modellierten Prozess vor. Wenn möglich, wird ein Prozess exemplarisch in einem Sprachmodell live ausprobiert — als erster Prompt, nicht als fertiges System. Den Abschluss bildet ein ehrlicher Reality-Check: Was davon ginge technisch schon heute? Wo fehlt die Infrastruktur? Was kommt in den nächsten Jahren? Die Teilnehmenden gehen mit einer realistischen Einschätzung und einem konkreten Ergebnis — ihrem Brown Paper — aus dem Workshop.

---

## Materialien

### Kartensatz (Prozess-Baukasten)

60 Karten in acht farbcodierten Kategorien (sechs Hauptkategorien plus zwei Meta-Karten). Ein kompletter Satz pro Gruppe. Druck auf 250 g/m² Karton, farbig, je 4 Karten pro A4-Seite. Inkl. Blanko-Karten („eigene Idee") zum Selbstbeschriften.

| Kategorie | Farbe | Karten | Funktion |
|---|---|---|---|
| Cover | weiß | 1 | Titelkarte mit Lizenz und Mitwirken-Hinweis |
| Start | Blau | 10 | Was löst den Prozess aus? |
| Input | Türkis | 9 | Welche Daten braucht das Modell? |
| Sprachmodell | Grün | 15 | Was macht das Sprachmodell? |
| Ausgabe | Orange | 11 | Wo geht das Ergebnis hin? |
| Mensch | Lila | 5 | Wo greift ein Mensch ein? |
| Bedenken | Gelb | 8 | Risiken und offene Fragen |
| Hinweis | Grau | 1 | Hinweis: Verbindungen aufs Brown Paper zeichnen |

Der vollständige Kartensatz ist als druckfertige PDF im [Release v0.1](https://github.com/exlab-code/ki-automatisierung-kartenset/releases/tag/v0.1) verfügbar oder direkt aus dem Browser über [exlab-code.github.io/ki-automatisierung-kartenset](https://exlab-code.github.io/ki-automatisierung-kartenset/) druckbar.

### Brainstorming-Worksheet

Ein A4-Blatt (quer) pro Person für die Einzelarbeit. Enthält Impulsfragen zur Identifikation textlastiger Prozesse und Platz zum Sammeln und Auswählen.

### Weiteres Material

- Brown Paper (ca. 80×120 cm pro Gruppe)
- Dicke Marker / Edding (2 pro Gruppe)
- Post-its für Notizen neben den Karten
- Kreppband zur Fixierung
- Laptop mit Sprachmodell-Zugang für die optionale Live-Demo

---

## Voraussetzungen

**Teilnehmende:** Keine technischen Vorkenntnisse nötig. Der Workshop funktioniert mit Gruppen, die bisher keinen Kontakt mit Sprachmodellen hatten, ebenso wie mit gemischten Gruppen. Die Impulsfragen und Karten sind so gestaltet, dass sie ohne Fachwissen verständlich sind.

**Raum:** Tische für Gruppenarbeit (3–4 Personen pro Tisch). Beamer oder Bildschirm für den Input-Teil. Genug Platz, dass Brown Paper auf den Tischen ausgebreitet werden kann.

**Moderation:** Eine Person, die den Input-Teil hält und während der Gruppenarbeit als Coach von Tisch zu Tisch geht. Fachkenntnis zu Sprachmodellen ist hilfreich, aber der Workshop lebt von der Arbeit der Teilnehmenden, nicht vom Wissen der Moderation.

**Zeitrahmen:** 90 Minuten sind der Mindestrahmen. Bei größeren Gruppen (>20 Personen) oder wenn der Rundgang ausführlicher sein soll, sind 120 Minuten komfortabler.

---

## Hintergrund

Dieses Workshop-Format basiert auf der Tradition kartenbasierter Design-Methoden (Halskov & Dalsgaard, 2006; Hsieh et al., 2023) und dem Trigger-Operation-Action-Paradigma moderner Automatisierungsplattformen (n8n, Make, Zapier, Power Automate). Die Pipeline-Metapher — Text rein, Transformation, Text raus — folgt dem Text-to-Text-Paradigma der aktuellen Sprachmodell-Forschung (Raffel et al., 2020) und der praktischen Prompt-Chaining-Architektur.

Die Kategorisierung der Modell-Operationen orientiert sich an etablierten NLP-Taxonomien und ist bewusst als pädagogische Vereinfachung angelegt. In der Praxis sind die Fähigkeiten von Sprachmodellen breiter und gleichzeitig ungleichmäßiger verteilt — Ethan Mollick und Fabrizio Dell'Acqua beschreiben dies treffend als „Jagged Frontier": Sprachmodelle sind bei manchen Aufgaben erstaunlich stark und bei scheinbar ähnlichen erstaunlich schwach. Die Bedenken-Karten und die Mensch-Karten im Kartensatz sind eine direkte Antwort auf dieses Phänomen.

---

*Dieses Format wurde ursprünglich für Führungskräfte in der Sozialwirtschaft entwickelt (AWO Führungskräfte Forum, 27.04.2026), ist aber branchenunabhängig einsetzbar. Die Impulsfragen, Karteninhalte und Beispielprozesse lassen sich an den jeweiligen Kontext anpassen.*

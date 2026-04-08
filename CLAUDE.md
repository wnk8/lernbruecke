# CLAUDE.md — LernBrücke

## Projektübersicht

LernBrücke ist ein kostenloses Lern-Toolkit (PDF) für Schülerinnen und Schüler
zwischen 10 und 16 Jahren aus einkommensschwachen oder benachteiligten Familien
in der Region Ludwigshafen/Rhein.

Projekttyp: Soziales Nachhaltigkeitsprojekt (Bildungsgerechtigkeit)
Zweck: Bewerbungsnachweis für das Deutschlandstipendium 2026 an der HWG Ludwigshafen
Status: In Umsetzung — Toolkit-PDF liegt vor, Webseite und Verbreitung ausstehend

---

## Initiator

Name: Steve Lennart Wanko
Studium: BWL Nachhaltigkeitsmanagement, 4. Semester, HWG Ludwigshafen
Wohnort: Frankenthal (Pfalz)
Hintergrund relevant für dieses Projekt:
- Nachhilfelehrer seit 2 Jahren, ca. 12–15 Std./Woche
- Unterricht auch an einer Gehörlosenschule
- Pflegt seinen Großvater (Einkauf, Haushalt, Behördengänge, Begleitung)
- Keine Förderung, kein Budget — ehrenamtliches Projekt

E-Mail (Platzhalter): steve@lernbruecke.de

---

## Projektstruktur

```
lernbruecke/
├── public/
│   ├── index.html             # Landingpage (Tag 3 — noch zu erstellen)
│   └── lernbruecke.pdf        # Toolkit-PDF (manuell aus Google Docs exportiert)
├── scripts/
│   └── generate_docx.py       # Python-Script zur .docx-Generierung (erledigt)
├── outreach/
│   ├── schulen.csv            # Schulliste Ludwigshafen mit Kontakten
│   ├── anschreiben_vorlage.txt
│   └── agentur_nachricht.txt
├── nachweise/
│   ├── README.md              # Nachweis-Checkliste für Bewerbung
│   ├── projektbeschreibung.txt
│   └── versand_log.csv
└── CLAUDE.md
```

---

## Toolkit-Inhalt (5 Kapitel)

Das fertige PDF-Toolkit enthält folgende Kapitel:

### Kapitel 1 — Lernstrategien für zu Hause
- Fester Lernplatz, Ablenkungen eliminieren
- Pomodoro-Methode (25 Min. Lernen / 5 Min. Pause / 20 Min. nach 4 Runden)
- Aktives Wiederholen: eigene Worte, laut erklären, Karteikarten
- Wochenplan mit max. 3 Punkten pro Tag
- Pausen als Pflicht, nicht als Belohnung; Schlaf als Lernschritt

### Kapitel 2 — Wie Eltern helfen können
- Feste Lernzeit einrichten, Struktur ohne Druck
- Fragen stellen statt erklären (Beispiele: "Was war heute schwierig?")
- Konkret und ehrlich loben (Anstrengung, nicht Ergebnis)
- Umgang mit Lernblockaden: laut vorlesen, Lehrer fragen, Erklärvideo
- Sprachliche Barrieren: Präsenz und Interesse reichen

### Kapitel 3 — Kostenlose Lernressourcen online
- Khan Academy, Studyflix, Schulminator, Sofatutor (kostenlose Inhalte), SimpleClub
- Üben: bettermarks, British Council, Duden Rechtschreibprüfung
- Offline: Stadtbibliothek Ludwigshafen (kostenloser Ausweis bis 18 Jahre)

### Kapitel 4 — Tipps gegen Prüfungsangst
- Vorbereitung: 1 Woche vorher, kurze Einheiten, Probeprüfungen, 7–8 Std. Schlaf
- Am Prüfungstag: frühstücken, früh aufbrechen, Atemübung (4/6 Sek.)
- Aufgabenstrategie: sichere Aufgaben zuerst
- Bei starker Angst: Schulberater, Eltern einweihen, Entspannungsübungen

### Kapitel 5 — Motivationsseite für Schüler
- Zitat Winston Churchill, Zitat Nelson Mandela
- Was wirklich zählt: Anstrengung, Ausdauer, Entscheidung
- Blanko-Felder: eigene Stärken aufschreiben
- Persönliche Nachricht von Steve

---

## Design-Vorgaben

Alle Dateien (HTML, Dokumente) halten sich an folgendes Design-System:

| Variable | Wert | Verwendung |
|---|---|---|
| Primär | #2d6a4f | Überschriften, Buttons, Header |
| Akzent | #52b788 | Borders, Highlights |
| Hellgrün | #d8f3dc | Callout-Hintergründe, CTA-Section |
| Blassgrün | #f0faf4 | Tabellen-Zebrastreifen |
| Text | #4a4a4a | Fließtext |
| Weiß | #ffffff | Hintergründe |

Schrift: Arial (Dokumente), System-Font-Stack (HTML)
Stil: Minimalistisch, klar, warm — kein Corporate-Look
Sprache: Deutsch, einfach, nicht belehrend, kein Behördendeutsch

---

## Tech-Stack

| Bereich | Technologie |
|---|---|
| Toolkit-Dokument | Python + python-docx → .docx → PDF via Google Docs |
| Landingpage | Vanilla HTML/CSS/JS, kein Framework, kein CDN |
| Hosting | tiiny.host (statisch, kein Account nötig) |
| Versionierung | Git + GitHub (wnk8/lernbruecke, öffentlich) |
| PDF-Hosting | Google Drive oder tiiny.host |

---

## Offene Aufgaben (in Reihenfolge)

- [ ] TAG 2: lernbruecke.pdf in public/ ablegen (manuell: Google Docs → Herunterladen → PDF)
- [ ] TAG 3: public/index.html erstellen (Landingpage)
- [ ] TAG 3: ZIP erstellen → tiiny.host hochladen → Link notieren
- [ ] TAG 3: Link in CLAUDE.md, README.md und nachweise/README.md eintragen
- [ ] TAG 4: outreach/schulen.csv mit echten Schulen befüllen
- [ ] TAG 4: Anschreiben und Agentur-Nachricht erstellen
- [ ] TAG 4: Erste Verbreitung (Schüler, Agentur, 2–3 Schulen)
- [ ] TAG 5: Rückmeldungen sammeln → nachweise/ dokumentieren
- [ ] TAG 5: Projektbeschreibung für Motivationsschreiben schreiben

---

## Bereits erledigt

- [x] Toolkit-Inhalt (5 Kapitel) vollständig ausgearbeitet
- [x] .docx generiert: LernBruecke_Toolkit.docx (python-docx, python)
- [x] Projektstruktur definiert
- [x] Claude Code Prompt-Bibliothek erstellt

---

## Bewerbungskontext (Deutschlandstipendium 2026)

Das Toolkit dient als konkreter Nachweis gesellschaftlichen Engagements.
Im Motivationsschreiben wird LernBrücke wie folgt positioniert:

Kernnarrativ: "Verantwortung unter realen Bedingungen"
- Nachhilfe 2 Jahre, echte Erfahrung mit Bildungsungleichheit
- Projekt ohne Budget, ohne Verein, mit echter Wirkung
- Verbindung zu Studium: Nachhaltigkeitsmanagement = soziale Dimension

Bewerbungsstatus: Motivationsschreiben v5 liegt vor (Schlusssatz noch offen)
Werkstudentenstelle CSR: Bewerbung läuft, keine Zusage — Schreiben wird bei
Zusage aktualisiert.

---

## Arbeitsregeln für Claude Code

1. Vor jeder Datei-Erstellung oder -Änderung: betroffene Datei zuerst lesen
2. Keine externen HTTP-Requests in HTML (offline-fähig, kein CDN)
3. Alle Dateien: UTF-8 Encoding
4. Platzhalter immer als {{PLATZHALTER}} markieren, nie leer lassen
5. Nach jedem abgeschlossenen Tag: Git-Commit mit Message "feat: Tag X – [Beschreibung]"
6. Keine Änderungen ohne Ankündigung — erst zeigen, dann umsetzen
7. Texte für Schüler/Eltern: einfache Sprache, max. Satzlänge 20 Wörter
8. Texte für Schulen/Behörden: formell aber persönlich, kein Baustein-Deutsch

---

## MCP-Server

| Server | Zweck |
|---|---|
| filesystem | Alle Projektdateien lesen und schreiben |
| github | Repository wnk8/lernbruecke pushen, Issues erstellen |
| context7 | Dokumentation python-docx, HTML-Standards nachschlagen |

---

## Wichtige Pfade

| Datei | Pfad | Status |
|---|---|---|
| Toolkit .docx | LernBruecke_Toolkit.docx (Download) | ✅ Vorhanden |
| Toolkit PDF | public/lernbruecke.pdf | ⏳ Ausstehend |
| Landingpage | public/index.html | ⏳ Ausstehend |
| Live-URL | {{TIINY_HOST_LINK}} | ⏳ Ausstehend |
| GitHub | https://github.com/wnk8/lernbruecke | ⏳ Ausstehend |

# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

<!-- ANPASSEN: Hochschule (IU), Sprache (Deutsch) und Zitierstil (APA 7, IU-Variante) sind gesetzt.
     Noch offen sind die themenspezifischen {{PLATZHALTER}} (Thema, Forschungsfrage, Fälle, Quellen) —
     diese erst füllen, sobald `context.txt` (aus `context.example.md`) angelegt ist. -->

## What this repository is

This is **not a software project** — it is a working directory for {{KONTEXT, z. B. „a German university
seminar / Hausarbeit / Bachelorarbeit"}} at the **IU Internationale Hochschule** on the topic
**{{THEMA}}**. There is no code, build system, or test suite. Work here is **research and academic
writing**: {{DELIVERABLES, z. B. „a written seminar paper"}}. Respond and write deliverables in
**German** unless asked otherwise.

The full project brief lives in `context.txt` (noch anzulegen aus `context.example.md`). Read it before
doing substantive work — the sections below summarize it, but it is the source of truth and may be
updated by the user.

**Formal authority:** the IU rules are binding and live in two PDFs at the repo root, summarized in
`Vorgaben.md`: `20251001_Richtlinien für die Gestaltung wissenschaftlicher Arbeiten.pdf` (Formatierung,
Aufbau) and `Zitierleitfaden.pdf` (Zitieren nach APA 7, IU-Variante). On any formal/citation question,
consult `Vorgaben.md` first; if it's silent, the PDFs win.

## Scope

<!-- ANPASSEN: Falls das Projekt in einer Gruppe/Arbeitsteilung steht, hier die eigene Zuständigkeit
     abgrenzen. Sonst diesen Abschnitt löschen. -->
The user owns **{{EIGENER BEREICH}}**: {{UNTERTHEMEN}}.
Other areas are context only — don't write content for them unless asked.

## Central argument (keep all deliverables consistent with this)

- **Forschungsfrage:** {{FORSCHUNGSFRAGE — eine präzise, beantwortbare Frage}}
- **Kernthese / wiederkehrende Aussage:** „{{KERNTHESE in einem Satz}}"
- **Anchor case studies:** {{FALL 1}} and {{FALL 2}}. Reuse these consistently rather than introducing
  new examples. <!-- ANPASSEN: Anker-Fälle sind optional, aber sehr wirksam für den roten Faden. -->

## Deliverables and their constraints

- **{{DELIVERABLE, z. B. Seminararbeit}}:** {{UMFANG, z. B. „10 Seiten reiner Fließtext"}},
  wissenschaftlich, arbeitet die Forschungsfrage theoretisch durch. **Das einzige aktive Deliverable.**
  <!-- ANPASSEN: Weitere/abgeschlossene Deliverables (z. B. Vortrag) hier als Kontext kennzeichnen. -->

Current state: siehe Status-Kopf in `{{HAUPTDATEI, z. B. Arbeit.md}}`. Faktenbasis in `Dossier.md`,
Literaturverzeichnis in `Quellen.md`.

## Sources to cite (already chosen — prefer these)

<!-- ANPASSEN: Bevorzugte, möglichst primäre Quellen pro Teilthema. Hält die Recherche fokussiert. -->
{{THEMA A: Quelle 1, Quelle 2}} · {{THEMA B: Quelle 3, Quelle 4}} · {{FALL 1: Behördenquelle}} ·
{{FALL 2: Behördenquelle}}.

## Verbindlicher Arbeitsworkflow

Pflicht für jede inhaltliche Arbeit. Arbeitsdateien:
- `Dossier.md` — gegengeprüfte Faktenbasis
- `Recherche.md` — Warteschlange/Queue der Quellen
- `Offene-Punkte.md` — sichtbare Lücken/Strittigkeiten
- `Quellen.md` — zentrales Literaturverzeichnis (APA 7, IU-Variante); jeder Beleg zeigt hierauf

**1 — Orientieren (immer zuerst).** Volles Bild verschaffen: `context.txt`, `Dossier.md`,
`Recherche.md`, `Offene-Punkte.md`, `Quellen.md` lesen und Stand erfassen.

**2 — Recherchieren (Loop pro Quelle).**
vollständig lesen → mit `Dossier.md` abgleichen, **belegte** Korrekturen einarbeiten → die darin
zitierten, *relevanten* Quellen mit Status `ungeprüft` in `Recherche.md` aufnehmen → gegengeprüfte
Quelle als vollständigen APA-7-Eintrag in `Quellen.md` ergänzen → nächsten ungeprüften Eintrag.
Die Queue darf gespeichert und später abgearbeitet werden. Leitplanken:
- **Relevanzfilter:** einer Unterquelle nur folgen, wenn sie eine *offene/strittige* Angabe stützen
  könnte — nicht blind jeder Quelle in jeder Quelle.
- **Tiefenlimit:** max. 2 Ebenen ohne Rückfrage.
- **Rekursive Einstufung:** von einer Primärquelle zitiert ≠ selbst primär; jeder Beleg trägt eigene
  Einstufung + Vorbehalt. Tertiärquellen (z. B. Wikipedia) nur als Wegweiser, nicht als Zitatbeleg.
- **Dedup + Abbruch:** abgeschlossene URLs nicht erneut verfolgen; stoppen bei Sättigung (neue Quellen
  wiederholen nur Bekanntes).
- **Gegenprüfung vor Aufnahme:** Fakten wandern erst nach Gegenprüfung ins Dossier.

**3 — Schreiben.** Belegt, sachlich, **Deutsch**, **APA 7 (IU-Variante)**. Jede inhaltliche Aussage bekommt
einen In-Text-Beleg (Autor, Jahr, Seite) mit Eintrag in `Quellen.md` — die IU verlangt die Seitenangabe
auch bei indirekten Zitaten (siehe `Vorgaben.md`). Unklares wandert nach `Offene-Punkte.md`,
wird **nie weggelassen oder geraten**. Roter Faden: jede Aussage zahlt auf Forschungsfrage/Kernthese ein.
- **Stil:** {{STILREGELN — z. B. „Keine Gedankenstriche zur Satzuntergliederung; stattdessen Komma,
  Doppelpunkt, Klammern oder zwei Sätze." Sonst diesen Punkt löschen.}}

**4 + 5 — Selbstprüfung vor dem Commit (Pflicht, erst danach `git commit`):**
- [ ] **Gegengelesen:** komplett selbst gelesen — schlüssig, roter Faden zur Forschungsfrage, keine
      Widersprüche, keine Dubletten/Reste.
- [ ] **Leser-Perspektive (ohne Vorwissen):** Fachbegriffe und Fallnamen beim **ersten Auftreten**
      erklärt; Chronologie der Fallbeispiele nachvollziehbar. Dabei entstandene Fragen → `Offene-Punkte.md`.
- [ ] Jede inhaltliche Aussage hat einen APA-7-Beleg (mit Seitenangabe) und Eintrag in `Quellen.md`.
- [ ] Widersprüche/Lücken sind **sichtbar** (Blockquote bzw. `Offene-Punkte.md`), nicht geglättet.
- [ ] Abbildungen: Urheber + Quelle genannt, Lizenz beachtet, Eintrag in `Quellen.md`; eigene Grafiken
      als solche gekennzeichnet.
- [ ] Keine Scratch-/Rohdaten-Dumps im Commit (rohe Web-/API-Antworten gelöscht).

## Git-Konventionen

- Erst nach bestandener Selbstprüfung committen.
- **Klein und thematisch:** ein Commit = ein abgeschlossener Gedanke; keine Sammel-Commits.
- **Deutsche Commit-Message**, knapp im Imperativ (z. B. `Dossier: {{Beispiel}} belegt`).
- **Nicht pushen ohne ausdrückliche Anweisung.**

## Sonstige Conventions

- Schreibsprache der Deliverables: **Deutsch**; kein „ich", „wir", „man" (IU-Vorgabe). Belege/Quellen
  dürfen anderssprachig sein (Titel im Literaturverzeichnis in Originalsprache, APA-7-konform).
- **Nicht zitierfähig** (IU): Skripte, Vorlesungsfolien, Webinare, Wikipedia (nur Wegweiser), KI als
  Informationsquelle. Details und KI-Sonderfälle in `Vorgaben.md`.
- Neue Dateien als schlichte Markdown-Dokumente in diesem Verzeichnis, sofern nicht anders vorgegeben.
- **Word-/PDF-Export:** Inhalt wird vollständig in Markdown erarbeitet und erst am Ende **manuell** in
  ein Dokument mit Hochschul-Vorlage übertragen. Während des Schreibens keine Layout-/Formatierungsarbeit
  — nur Inhalt, Struktur, Belege.
- **Hochschul-Vorgaben** stehen in `Vorgaben.md`. In der Markdown-Phase **kein** Deckblatt/
  Eigenständigkeitserklärung/Verzeichnis — die entstehen erst beim Umzug ins Office-Dokument.

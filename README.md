# Vorlage: Wissenschaftliche Seminar-/Hausarbeit mit Claude Code

Eine wiederverwendbare GitHub-Template-Vorlage für **belegte, quellenkritische Schreibprojekte**
(Seminararbeit, Hausarbeit, Bachelorarbeit, Literaturreview) mit Claude Code. Kein Software-Projekt,
sondern **Recherche + akademisches Schreiben** mit einem disziplinierten, nachvollziehbaren Workflow.

**Vorkonfiguriert für die IU Internationale Hochschule:** Schreibsprache **Deutsch**, Zitierstil
**APA 7 (IU-Variante)**. Die verbindlichen Formalia sind in `Vorgaben.md` zusammengefasst; maßgeblich
sind die beiden IU-PDFs im Repo (`…Richtlinien für die Gestaltung wissenschaftlicher Arbeiten.pdf`,
`Zitierleitfaden.pdf`, Stand 01.10.2025). Themenspezifisches (Thema, Forschungsfrage, Fälle, Quellen)
bleibt als `{{PLATZHALTER}}` offen und wird pro Arbeit gefüllt.

Der Kern der Vorlage ist nicht der Inhalt, sondern die **Arbeitsdisziplin**: Fakten wandern erst nach
Gegenprüfung in die Faktenbasis, jede Aussage trägt einen Beleg, Unklares wird sichtbar gemacht statt
weggelassen, und nichts wird geraten.

## Was drin ist

| Datei | Zweck |
|-------|-------|
| `CLAUDE.md` | Anweisungen für Claude Code: Projektart, Forschungsfrage, Workflow, Konventionen. **Zuerst anpassen.** |
| `Arbeit.md` | Das eigentliche Deliverable (Fließtext). Wird komplett in Markdown erarbeitet, erst am Ende nach Word übertragen. |
| `Dossier.md` | Gegengeprüfte Faktenbasis. Nur bestätigte Fakten gelten als gesichert. |
| `Recherche.md` | Quellen-Warteschlange (Queue) mit Status und Einstufung. |
| `Quellen.md` | Zentrales Literaturverzeichnis (APA 7, IU-Variante), Single Source of Truth für Belege. |
| `Offene-Punkte.md` | Sichtbarer Sammelplatz für Unklares/Strittiges. Nichts wird hier geglättet. |
| `Vorgaben.md` | Formale IU-Vorgaben (Formatierung, Zitierstil, Aufbau, Pflichtteile). |
| IU-PDFs | `…Richtlinien…Gestaltung…Arbeiten.pdf` + `Zitierleitfaden.pdf` — die **verbindlichen** Originale. |
| `context.example.md` | Skelett für den Projekt-Brief (umbenennen zu `context.txt`). |
| `.gitignore` | Ignoriert Rohdaten-Dumps, Office-Temp-Dateien, Exporte. |

## Neues Projekt starten (Checkliste)

Sprache, Zitierstil und IU-Formalia sind bereits gesetzt — pro Arbeit ist nur noch das
Themenspezifische zu füllen:

1. **Repo aus Vorlage erzeugen:** Auf GitHub „Use this template" → „Create a new repository"
   (oder den Ordnerinhalt in ein leeres Verzeichnis kopieren und `git init`).
2. **`context.example.md` → `context.txt`** umbenennen und mit Modul, Thema, Forschungsfrage,
   Kernthese und Anker-Fällen füllen.
3. **`CLAUDE.md`:** nur noch die themenspezifischen `{{PLATZHALTER}}` ersetzen
   (`{{THEMA}}`, `{{FORSCHUNGSFRAGE}}`, `{{KERNTHESE}}`, `{{FALL 1/2}}`, bevorzugte Quellen,
   ggf. `{{STILREGELN}}`). Sprache (Deutsch) und Zitierstil (APA 7) stehen schon.
4. **`Vorgaben.md`:** den konkreten **Seitenumfang aus dem Prüfungsleitfaden** der jeweiligen
   Prüfungsleistung eintragen; bei Abschlussarbeiten zusätzlich das Thesis-Handbuch prüfen.
5. **Arbeitsdateien leeren:** Beispielzeilen in `Dossier.md`, `Recherche.md`, `Quellen.md` und
   `Offene-Punkte.md` durch echte Inhalte ersetzen; Titel und Gliederung in `Arbeit.md` anpassen.
6. Claude Code starten und mit der Recherche beginnen. Claude liest zuerst `CLAUDE.md` und `context.txt`.

## Diese Vorlage zur GitHub-Template-Repo machen

Nach dem ersten Push: auf GitHub unter **Settings → General → „Template repository"** aktivieren.
Danach erscheint bei jedem neuen Repo der Button „Use this template".

## Das Workflow-Prinzip in einem Satz

**Orientieren → Recherchieren (Loop pro Quelle) → Schreiben (belegt) → Selbstprüfung → Commit.**
Details stehen in `CLAUDE.md`.

# Vorlage: Wissenschaftliche Seminar-/Hausarbeit mit Claude Code

Eine wiederverwendbare GitHub-Template-Vorlage für **belegte, quellenkritische Schreibprojekte**
(Seminararbeit, Hausarbeit, Bachelorarbeit, Literaturreview) mit Claude Code. Kein Software-Projekt,
sondern **Recherche + akademisches Schreiben** mit einem disziplinierten, nachvollziehbaren Workflow.

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
| `Quellen.md` | Zentrales Literaturverzeichnis (APA 7), Single Source of Truth für Belege. |
| `Offene-Punkte.md` | Sichtbarer Sammelplatz für Unklares/Strittiges. Nichts wird hier geglättet. |
| `Vorgaben.md` | Formale Hochschul-Vorgaben (Umfang, Zitierstil, Pflichtteile). |
| `context.example.md` | Skelett für den Projekt-Brief (umbenennen zu `context.txt`). |
| `.gitignore` | Ignoriert Rohdaten-Dumps, Office-Temp-Dateien, Exporte. |

## Schnellstart

1. **Repo aus Vorlage erzeugen:** Auf GitHub „Use this template" → „Create a new repository"
   (oder den Ordnerinhalt in ein leeres Verzeichnis kopieren und `git init`).
2. **`context.example.md` → `context.txt`** umbenennen und mit deinem Thema füllen.
3. **`CLAUDE.md` anpassen:** Alle `{{PLATZHALTER}}` ersetzen und die `<!-- ANPASSEN -->`-Hinweise
   abarbeiten, dann die Kommentare löschen.
4. **`Vorgaben.md`** mit den Vorgaben deiner Hochschule füllen.
5. Claude Code starten und mit der Recherche beginnen. Claude liest zuerst `CLAUDE.md` und `context.txt`.

## Diese Vorlage zur GitHub-Template-Repo machen

Nach dem ersten Push: auf GitHub unter **Settings → General → „Template repository"** aktivieren.
Danach erscheint bei jedem neuen Repo der Button „Use this template".

## Das Workflow-Prinzip in einem Satz

**Orientieren → Recherchieren (Loop pro Quelle) → Schreiben (belegt) → Selbstprüfung → Commit.**
Details stehen in `CLAUDE.md`.

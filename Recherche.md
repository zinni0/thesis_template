# Recherche-Arbeitsdatei (Warteschlange)

Dies ist die **Queue**. Pro Quelle der Loop: **vollständig lesen → mit Dossier abgleichen, belegte
Korrekturen einarbeiten → darin zitierte, relevante Quellen als `ungeprüft` aufnehmen → nächsten
ungeprüften Eintrag.** Speichern und späteres Abarbeiten erlaubt.

**Leitplanken:** Relevanzfilter · Tiefenlimit max. 2 Ebenen ohne Rückfrage · Einstufung rekursiv ·
Dedup + Abbruch bei Sättigung.

**Status:** `ungeprüft` · `in Arbeit` · `abgeschlossen` · `verworfen`
**Einstufung:** `Primär` · `Sekundär` · `Tertiär (nur Wegweiser)`
**Ebene:** `0` = Seed (vorausgewählt) · `1`/`2` = aus einer Quelle der Ebene darüber zitiert

---

## Warteschlange

<!-- ANPASSEN: Seed-Quellen (Ebene 0) sind die in CLAUDE.md vorausgewählten. Beispielzeilen ersetzen. -->

| # | Quelle | Ebene | Zitiert von | Stützt (Dossier-#) | Einstufung | Status |
|---|--------|-------|-------------|--------------------|-----------|--------|
| 1 | {{Quelle / Behörde / Bericht}} | 0 | Seed | A1, A4 | Primär | ungeprüft |
| 2 | {{Quelle}} | 0 | Seed | B1 | Primär | ungeprüft |
| 3 | {{aus #1 zitierte Unterquelle}} | 1 | #1 | A2 | Sekundär | ungeprüft |

---

<!-- Hinweis: Eine Quelle gilt erst als „abgeschlossen", wenn sie vollständig gelesen, mit dem Dossier
     abgeglichen und (falls bestätigt) als APA-Eintrag in Quellen.md übernommen ist. -->

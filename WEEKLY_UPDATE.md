# Wöchentliches Update – Anleitung

## So erstellst du jede Woche einen neuen Plan

### 1. Öffne Claude Code in diesem Verzeichnis

```
cd G:\sszsim\_tmp\my_fodmap
```

### 2. Gib diesen Prompt ein (copy-paste):

```
Erstelle einen neuen FODMAP-Wochenplan für Woche [NUMMER].
Gleiche Vorgaben wie bisher (siehe CLAUDE.md):
- Eliminationsphase, streng nach Monash
- OHNE Nüsse, Bananen, Sojaprodukte
- 7 Tage × 4 Mahlzeiten (Frühstück, Mittag, Abend, Snack)
- Neue Rezepte, keine Wiederholungen aus vorherigen Wochen
- Ersetze den Inhalt von index.html
```

### 3. Prüfe und pushe

Claude wird die `index.html` aktualisieren. Dann:

```
git add index.html
git commit -m "Woche [NUMMER]: neuer Wochenplan"
git push
```

Die Live-Seite aktualisiert sich automatisch nach ~1 Minute.

---

## Varianten

### Nur bestimmte Tage ändern
> „Ersetze Mittwoch und Donnerstag durch neue Rezepte."

### Saisonale Anpassung
> „Erstelle Woche 3 mit saisonalen Herbst-/Wintergemüsen."

### Re-Introduktionsphase (ab Woche 7+)
> „Erstelle einen Plan für die Wiedereinführungsphase. Teste diese Woche Laktose."

### Einkaufsliste generieren
> „Erstelle eine Einkaufsliste für den aktuellen Wochenplan."

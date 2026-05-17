# Wöchentliches Update – Anleitung

## So erstellst du jede Woche einen neuen Plan

### 1. Claude Code in diesem Verzeichnis öffnen

```bash
cd G:\sszsim\_tmp\my_fodmap
```

### 2. Prompt eingeben (copy-paste)

#### Standard – Neuer Wochenplan:
```
Erstelle einen neuen FODMAP-Wochenplan für Woche [NUMMER].
Gleiche Vorgaben wie bisher (siehe CLAUDE.md):
- Eliminationsphase, streng nach Monash
- OHNE Nüsse, Bananen, Sojaprodukte
- 7 Tage × 4 Mahlzeiten (Frühstück, Mittag, Abend, Snack)
- Neue Rezepte, keine Wiederholungen aus vorherigen Wochen
- Ersetze den Inhalt von index.html
```

### 3. Prüfen und pushen

```bash
git add index.html
git commit -m "Woche [NUMMER]: neuer Wochenplan"
git push
```

Die Live-Seite aktualisiert sich automatisch nach ~1 Minute.

---

## Weitere Prompt-Varianten

### Nur bestimmte Tage ändern
```
Ersetze Mittwoch und Donnerstag durch neue Rezepte.
Gleiche Vorgaben (siehe CLAUDE.md).
```

### Saisonale Anpassung
```
Erstelle Woche [N] mit saisonalen Sommer-/Herbst-/Winter-Gemüsen.
Gleiche Vorgaben (siehe CLAUDE.md).
```

### Re-Introduktionsphase (ab Woche 7+)
```
Erstelle einen Plan für die Wiedereinführungsphase.
Teste diese Woche: [Laktose / Fruktose / Polyole / etc.]
Alle anderen FODMAP-Gruppen weiterhin meiden.
Gleiche Allergie-Einschränkungen (siehe CLAUDE.md).
```

### Einkaufsliste generieren
```
Erstelle eine Einkaufsliste für den aktuellen Wochenplan in index.html.
Gruppiere nach: Gemüse, Früchte, Proteine, Milchprodukte, Vorrat.
```

### Spezifische Wünsche
```
Erstelle Woche [N] mit Fokus auf:
- Schnelle Gerichte (max. 15 Min. Zubereitung)
- Meal-Prep-tauglich (Mittagessen vorkochbar)
Gleiche Vorgaben (siehe CLAUDE.md).
```

---

## Hinweise

- Claude liest `CLAUDE.md` automatisch beim Öffnen des Verzeichnisses
- Alle Allergien und FODMAP-Regeln sind dort hinterlegt
- Bei Unsicherheit fragt Claude nach oder prüft online (Monash-Quellen)
- Olivenöl und Sonnenblumenöl sind frei austauschbar

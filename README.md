# my_fodmap – FODMAP Wochenplan

Mobiler Ernährungsplan für die **Low-FODMAP Eliminationsphase**, basierend auf dem Monash University Ampelsystem.

🔗 **Live:** [dongoginho.github.io/my_fodmap](https://dongoginho.github.io/my_fodmap/)

## Features

- 7 Tage × 4 Mahlzeiten = 28 Rezepte mit exakten Mengenangaben (1 Person)
- Mobile-first Design mit Tab-Navigation und Swipe-Gesten
- Aufklappbare Rezeptkarten
- Homescreen-fähig (PWA-Meta-Tags)
- Keine externen Abhängigkeiten – eine einzige HTML-Datei
- Monash-Quellenhinweis bei jedem Rezept

## Allergien berücksichtigt

| Ausgeschlossen | Ersatz |
|---|---|
| Alle Nüsse (Baum-, Erd-, Cashew, Mandeln, Haselnüsse) | Kürbiskerne, Sonnenblumenkerne, Sesam |
| Bananen | Heidelbeeren, Erdbeeren, Kiwi |
| Sojaprodukte (Tofu, Sojasauce, Sojamilch, Sojasprossen) | Fischsauce, laktosefreie Milch, Kokosmilch |

## Quellen

Alle Angaben stammen aus verifizierten FODMAP-Quellen:

- [Monash University FODMAP App](https://www.monashfodmap.com) – Portionsgrössen und Ampelsystem
- [fodmap-konzept.ch](https://www.fodmap-konzept.ch) – Buhmann/Kiss (Schweizer Autorinnen)
- [reizdarmblog.de](https://www.reizdarmblog.de/ultimative-fodmap-liste/) – FODMAP-Liste
- [fodmaps.de](https://www.fodmaps.de/fodmap-liste/) – Lebensmittelliste

## Wöchentlich aktualisieren

Dieser Plan wird regelmässig mit neuen Rezepten aktualisiert.

### Mit Claude Code

```bash
cd G:\sszsim\_tmp\my_fodmap
```

Dann:

> „Erstelle einen neuen FODMAP-Wochenplan (Woche 2) mit den gleichen Vorgaben."

Claude liest `CLAUDE.md` automatisch und kennt alle Regeln. Siehe `WEEKLY_UPDATE.md` für weitere Prompt-Varianten.

### Regeln für neue Rezepte

1. **Nur Monash-grüne Lebensmittel** in den angegebenen Portionsgrössen
2. **Keine Nüsse, Bananen, Sojaprodukte** (Allergie!)
3. **Kein Knoblauch/Zwiebeln** (Knoblauchöl erlaubt)
4. **Nur glutenfreie** Getreideprodukte
5. **Olivenöl ↔ Sonnenblumenöl** austauschbar
6. Jedes Rezept: Zutaten (Gramm), Schritte, kcal, Zeit, Monash-Hinweis

### Deployment

```bash
git add index.html
git commit -m "Woche N: neuer Plan"
git push
```

GitHub Pages aktualisiert automatisch (~1 Minute).

## Projektstruktur

```
my_fodmap/
├── index.html          # Die App (wird live angezeigt)
├── README.md           # Diese Datei
├── CLAUDE.md           # Regeln für Claude Code
└── WEEKLY_UPDATE.md    # Prompt-Vorlagen für Updates
```

## Technisch

- Single HTML file – `index.html` ersetzen reicht
- Kein Build-Prozess, keine Dependencies
- GitHub Pages serviert direkt aus `main` branch
- Responsive: Mobile-first, Desktop ab 768px

## Lizenz

Persönlicher Gebrauch. Rezepte basieren auf öffentlich verfügbaren FODMAP-Richtlinien der Monash University.

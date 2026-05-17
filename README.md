# my_fodmap – FODMAP Wochenplan

Mobiler Ernährungsplan für die **Low-FODMAP Eliminationsphase** (Woche 1), basierend auf dem Monash University Ampelsystem.

🔗 **Live:** [dongoginho.github.io/my_fodmap](https://dongoginho.github.io/my_fodmap/)

## Features

- 7 Tage × 4 Mahlzeiten = 28 Rezepte mit exakten Mengenangaben
- Mobile-first Design mit Tab-Navigation und Swipe-Gesten
- Aufklappbare Rezeptkarten (spart Platz auf dem Handy)
- Kann als App auf dem Homescreen gespeichert werden (PWA)
- Keine externen Abhängigkeiten – eine einzige HTML-Datei

## Allergien berücksichtigt

| Ausgeschlossen | Ersatz |
|---|---|
| Alle Nüsse (Baum-, Erd-, Cashew, Mandeln) | Kürbiskerne, Sonnenblumenkerne, Sesam |
| Bananen | Heidelbeeren, Erdbeeren, Kiwi |
| Sojaprodukte (Tofu, Sojasauce, Sojamilch) | Fischsauce, laktosefreie Milch, Kokosmilch |

## Quellen

Alle Angaben stammen aus verifizierten FODMAP-Quellen:

- [Monash University FODMAP App](https://www.monashfodmap.com) – Portionsgrössen und Ampelsystem
- [fodmap-konzept.ch](https://www.fodmap-konzept.ch) – Buhmann/Kiss (Schweizer Autorinnen)
- [reizdarmblog.de](https://www.reizdarmblog.de/ultimative-fodmap-liste/) – FODMAP-Liste
- [fodmaps.de](https://www.fodmaps.de/fodmap-liste/) – Lebensmittelliste

## Wöchentlich aktualisieren

Dieser Plan kann jede Woche mit neuen Rezepten aktualisiert werden. Anleitung:

### Mit Claude Code

```
cd G:\sszsim\_tmp\my_fodmap
```

Dann einfach sagen:

> „Erstelle einen neuen FODMAP-Wochenplan (Woche 2/3/...) mit den gleichen Vorgaben."

Claude kennt alle Regeln aus der `CLAUDE.md` automatisch.

### Regeln für neue Rezepte

1. **Nur Monash-grüne Lebensmittel** in den angegebenen Portionsgrössen
2. **Keine Nüsse, Bananen, Sojaprodukte** (Allergie!)
3. **Kein Knoblauch/Zwiebeln** (Knoblauchöl erlaubt)
4. **Nur glutenfreie** Getreideprodukte
5. **Olivenöl darf durch Sonnenblumenöl** ersetzt werden
6. Jedes Rezept braucht: Zutaten mit Gramm, Schritte, kcal, Zeit, Monash-Quellenhinweis

## Technisch

- Single HTML file – einfach `index.html` ersetzen
- Kein Build-Prozess nötig
- Push auf `main` → GitHub Pages aktualisiert automatisch (~1 Min.)

## Lizenz

Persönlicher Gebrauch. Rezepte basieren auf öffentlich verfügbaren FODMAP-Richtlinien.

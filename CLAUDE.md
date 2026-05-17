# FODMAP Wochenplan – my_fodmap

## Übersicht
Mobile-optimierter FODMAP-Ernährungsplan als Single-File HTML-App, gehostet auf GitHub Pages.

**Live:** https://dongoginho.github.io/my_fodmap/  
**Repo:** github.com/DonGoginho/my_fodmap  
**Stand:** Woche 1 (Eliminationsphase), erstellt 17.05.2026

## Dateien
| Datei | Zweck |
|-------|-------|
| `index.html` | Komplette App (HTML+CSS+JS) – wird von GitHub Pages angezeigt |
| `README.md` | Projektbeschreibung für GitHub |
| `CLAUDE.md` | Diese Datei – Regeln für Claude Code |
| `WEEKLY_UPDATE.md` | Anleitung für wöchentliche Plan-Aktualisierung |

## Allergien / Einschränkungen (STRIKT einhalten!)
- **KEINE Nüsse** (keine Baumnüsse, Mandeln, Erdnüsse, Cashews, Erdnussbutter, Haselnüsse)
- **KEINE Bananen**
- **KEINE Sojaprodukte** (kein Tofu, keine Sojasauce/Tamari, keine Sojamilch, keine Sojasprossen)

## Erlaubte Ersatzprodukte
| Statt | Verwenden |
|-------|-----------|
| Nüsse | Kürbiskerne, Sonnenblumenkerne, Sesam (max. 2 EL) |
| Erdnussbutter | Tahini / Sesammus (max. 1 EL) |
| Banane | Heidelbeeren, Erdbeeren, Kiwi |
| Tofu | Lachs, Poulet, Ei, Crevetten |
| Sojasauce/Tamari | Fischsauce (max. 1 EL) |
| Sojamilch | Laktosefreie Milch, Kokosmilch |
| Olivenöl | Sonnenblumenöl (alle reinen Öle FODMAP-frei) |

## FODMAP-Regeln
- Alle Portionsgrössen gemäss Monash University Ampelsystem (grün = sicher)
- Keine Zwiebeln, kein Knoblauch (Knoblauchöl erlaubt – FODMAPs nicht fettlöslich)
- Nur grüner Teil der Frühlingszwiebel
- Glutenfreie Produkte verwenden (Brot, Pasta, Haferflocken)
- Hartkäse erlaubt (Gruyère, Parmesan, Cheddar = laktosearm durch Reifung)
- Kokosmilch aus Dose max. 125 ml pro Portion

## Quellen (NICHT erfinden – nur verifizierte Angaben!)
- Monash University FODMAP App (Ampelsystem, Portionsgrössen)
- fodmap-konzept.ch (Buhmann/Kiss, Schweizer Autorinnen)
- reizdarmblog.de (FODMAP-Liste 2026)
- fodmaps.de (Rezepte und Lebensmittellisten)

## Wöchentliches Update – Workflow
1. Neuen Wochenplan erstellen (WEEKLY_UPDATE.md für Prompt-Vorlagen)
2. `index.html` ersetzen mit neuem Plan
3. `git add index.html && git commit -m "Woche N" && git push`
4. GitHub Pages aktualisiert automatisch (~1 Min.)

## Technische Details
- Single-file HTML (kein Build-System, keine externen Abhängigkeiten)
- CSS-only Responsive Design (Breakpoint 768px für Desktop-Darstellung)
- JavaScript: Bottom-Tab-Navigation (Mo–So), Touch-Swipe zwischen Tagen, Accordion-Karten
- PWA-Meta-Tags (apple-mobile-web-app-capable, theme-color #2d6a4f)
- Safe-Area-Insets für iPhone Notch/Dynamic Island
- 44px min Touch-Targets (Apple/Google Accessibility Guidelines)
- GitHub Pages Deployment via main branch, root folder

## Rezept-Struktur (für neue Wochen beibehalten)
- 7 Tage × 4 Mahlzeiten (Frühstück, Mittagessen, Abendessen, Snack)
- Pro Rezept: Titel, Emoji, Zutaten mit Grammangaben, Zubereitungsschritte, kcal, Zubereitungszeit
- Monash-Quellenhinweis als Fussnote pro Rezept (z.B. „Heidelbeeren grün ≤125 g")
- Portionen immer für 1 Person

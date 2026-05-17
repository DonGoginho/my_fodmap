# FODMAP Wochenplan – my_fodmap

## Übersicht
Mobile-optimierter FODMAP-Ernährungsplan (Woche 1, Eliminationsphase) als Single-File HTML-App.

**Live:** https://dongoginho.github.io/my_fodmap/

## Dateien
- `index.html` — Komplette App (HTML + CSS + JS in einer Datei)

## Allergien / Einschränkungen (STRIKT einhalten)
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

## FODMAP-Regeln
- Alle Portionsgrössen gemäss Monash University Ampelsystem (grün = sicher)
- Keine Zwiebeln, kein Knoblauch (Knoblauchöl erlaubt – FODMAPs nicht fettlöslich)
- Nur grüner Teil der Frühlingszwiebel
- Olivenöl darf durch Sonnenblumenöl ersetzt werden (alle reinen Öle FODMAP-frei)
- Glutenfreie Produkte verwenden (Brot, Pasta, Haferflocken)
- Hartkäse erlaubt (Gruyère, Parmesan, Cheddar = laktosearm durch Reifung)

## Quellen (nicht erfinden – nur verifizierte Angaben!)
- Monash University FODMAP App (Ampelsystem, Portionsgrössen)
- fodmap-konzept.ch (Buhmann/Kiss, Schweizer Autorinnen)
- reizdarmblog.de (FODMAP-Liste 2026)
- fodmaps.de (Rezepte und Listen)

## Technische Details
- Single-file HTML (kein Build-System, keine externen Abhängigkeiten)
- CSS-only Responsive Design (Breakpoint 768px Desktop)
- JavaScript: Tab-Navigation (Mo–So), Touch-Swipe, Accordion-Karten
- PWA-Meta-Tags (Homescreen-fähig, theme-color #2d6a4f)
- Safe-Area-Insets für iPhone Notch/Dynamic Island
- 44px Touch-Targets (Apple/Google Accessibility)

## Inhalt
- 7 Tage × 4 Mahlzeiten = 28 Rezepte
- Jedes Rezept: Zutaten mit Grammangaben, Zubereitungsschritte, kcal, Zubereitungszeit
- Monash-Quellenhinweis pro Rezept (welche Portion grün ist)

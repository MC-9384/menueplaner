# Menüplaner

PWA zur Planung des Wochenmenüs. Reines HTML/JS, offlinefähig, Daten in `localStorage` (Schlüssel `menueplaner`). Idee aus dem Second Brain: `20 - Bereiche/Familie/Organisation/App Menüplanung.md`.

## Tabs

- **Woche** – Mo–So mit Wochennavigation (KW). Pro Tag beliebig viele Gerichte aus den Rezepten oder als Freitext (z. B. „auswärts essen“). Portionen je Gericht mit +/− einstellbar.
- **Rezepte** – Suche (Name, Tag, Zutat) und Tag-Filter. Rezepte ansehen, bearbeiten, **als Variante kopieren** (Kopie mit Vermerk „Variante von …“), löschen. Zutaten werden als Text eingegeben („500 g Mehl“, eine Zeile pro Zutat) und automatisch zerlegt.
- **Einkauf** – Liste aus den geplanten Gerichten der Woche: Mengen werden auf die Portionen umgerechnet und gleiche Zutaten zusammengerechnet (g/kg, ml/l; Stückware wird aufgerundet). Tage abwählbar, Häkchen, eigene Zusatzartikel, Button **Einkaufsliste kopieren** (nur offene Posten).
- **Backup** – JSON-Backup/-Import, Rezepte als Markdown fürs Second Brain.

Beim ersten Start sind 32 Standardrezepte angelegt (Nudeln & Reis, Kartoffeln, Fleisch & Fisch, Eier & Süßes, Suppen, Pizza, Wraps, Kuchen, Dessert) – Mengen bei Bedarf anpassen.

## Entwicklung

Dev-Server: `launch.json`-Eintrag `menueplaner` (Port 8652). Änderungen an `index.html` → `CACHE` in `sw.js` hochzählen.

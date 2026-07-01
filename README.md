# amtec DIN 13 Gewinderechner (PWA)

Metrische Gewindeberechnung nach DIN 13 als installierbare Web-App (PWA) —
der Rechner-Teil der amtec-DIN13-Desktop-App, ohne Zeichnungs-Archiv.

- **Nutzen am Handy:** Seite öffnen → Teilen/Menü → „Zum Home-Bildschirm".
  Läuft danach wie eine App und **offline** (Service Worker cacht alles).
- **Technik:** statische Single-File-HTML + `manifest.webmanifest` + `sw.js`.
  Kein Backend, keine vertraulichen Daten (DIN 13 ist eine öffentliche Norm).

## Hosting

GitHub Pages liefert den Ordner-Inhalt direkt aus (`main`-Branch, Root).
Bei Änderungen an `index.html` die Cache-Version in `sw.js` hochzählen
(`din13-v1` → `din13-v2`), damit Geräte die neue Version laden.

© 2026 T. Scholl · Im Auftrag der amtec Spannhydraulik GmbH

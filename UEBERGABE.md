# Wetter – Übergabe

**Stand:** v1 (09.11.2026)
**Live:** https://tom444555.github.io/wetter/ (GitHub Pages, Branch `main`, Ordner `/`)
**Vorschau-Artifact:** https://claude.ai/artifact/2STVJCi3b5W7WCpCFsB87a (nur Beispieldaten – Artifacts dürfen nichts abrufen)

## Aufbau
- Eine Datei `index.html` (HTML/CSS/JS, keine Bibliotheken), iOS-Stil
- Daten: Open-Meteo (Vorhersage, Luftqualität/Pollen, Ortssuche) – kostenlos, ohne Schlüssel
- Standard-Ort Quierschied; Orte + letzter Datenstand in localStorage
- Ohne Netz: letzter Stand, sonst Beispieldaten (Hinweis oben)
- `manifest.json` + Icons → „Zum Home-Bildschirm“ als App

## Bereiche
Kopf · Regen nächste 2 Std (15 Min) · Stunden · Temperaturverlauf (Börsenkurs-Stil) · 16 Tage · Kacheln (Gefühlt, Wind, UV, Sonne, Feuchte, Druck, Luftqualität, Pollen) · Orte-Liste/Suche/Standort

## Ideen
DWD-Unwetterwarnungen · Radarkarte · Baustellen-Hinweis für morgen

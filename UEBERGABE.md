# Wetter – Übergabe

**Stand:** v2 (09.11.2026) – Regenradar
**Live:** https://tom444555.github.io/Wetter/ (GitHub Pages, Branch `main`, Ordner `/`)
**Vorschau-Artifact:** https://claude.ai/artifact/2STVJCi3b5W7WCpCFsB87a (nur Beispieldaten – Artifacts dürfen nichts abrufen)

## Aufbau
- Eine Datei `index.html` (HTML/CSS/JS, keine Bibliotheken), iOS-Stil
- Daten: Open-Meteo (Vorhersage, Luftqualität/Pollen, Ortssuche) – kostenlos, ohne Schlüssel
- Standard-Ort Quierschied; Orte + letzter Datenstand in localStorage
- Ohne Netz: letzter Stand, sonst Beispieldaten (Hinweis oben)
- `manifest.json` + Icons → „Zum Home-Bildschirm“ als App

## Regenradar (v2)
- Karte: Leaflet (cdnjs) + Esri „Dark Gray“ (ohne Schlüssel; CARTO verlangt inzwischen einen API-Key)
- Radar: DWD-WMS `dwd:Niederschlagsradar` (5-Min-Raster, ca. 2 Std. Prognose), 1 Bild pro Zeitpunkt für ganz Deutschland (Kacheln waren zu langsam, 3–25 s je Kachel)
- Zeitleiste: −60 Min bis +105 Min in 15-Min-Schritten; aktuelles Bild zuerst, Rest wird nacheinander vorgeladen
- Optional: DWD-Warnungen (`dwd:Warnungen_Landkreise`); Vollbild mit Zoomen/Verschieben
- Radar nur für Deutschland und das nahe Umland

## Bereiche
Kopf · Regen nächste 2 Std (15 Min) · Stunden · Temperaturverlauf (Börsenkurs-Stil) · 16 Tage · Kacheln (Gefühlt, Wind, UV, Sonne, Feuchte, Druck, Luftqualität, Pollen) · Orte-Liste/Suche/Standort

## Ideen
DWD-Unwetterwarnungen · Radarkarte · Baustellen-Hinweis für morgen

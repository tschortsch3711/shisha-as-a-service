# Shisha as a Service

Kleine statische Seite mit vier Shisha-Bar-Vorschlägen für ein Treffen am Donnerstag, 19.11.2026, irgendwo zwischen Freising und Regensburg.

Die Seite liegt in `index.html`, Fotos in `img/`. Kein externes JavaScript, kein Tracking, kein Formular. Wer die Seite bekommt, schaut sie sich an und antwortet per Nachricht mit der Nummer.

Live: https://tschortsch3711.github.io/shisha-as-a-service/

## Aufbau

- Oben eine Strecke Freising ↔ Regensburg: Jede Bar sitzt dort, wo sich die Fahrzeit für beide aufteilt. Die Nummern laufen entlang dieser Strecke.
- Umschalter „Dein Start“: Regensburg oder Unterschleißheim (Link direkt auf Unterschleißheim: `?ab=unterschleissheim`). Die Nummern bleiben dabei gleich.
- Darunter die Karten, am Desktop nebeneinander (Zeilen über alle Karten ausgerichtet), auf dem Handy untereinander.
- Ganz unten ein kleiner Service-Check zum Augenzwinkern.
- Alle Daten stehen im Array `BARS` oben im Script von `index.html`.
- Vorher wurden drei Layout-Prototypen verglichen (Vergleichsliste, Strecke, eine Bar pro Bildschirm). Gewählt wurde die Strecke.
- Ein Favorit lässt sich per `fav: true` im Array markieren.

## Seite lokal ansehen

`index.html` im Browser öffnen oder:

```
python3 -m http.server 8080
```

Danach `http://localhost:8080` aufrufen.

## Fotos

- Alle Fotos: Titelbilder aus den Google-Maps-Profilen der Bars, auf 16:9 zugeschnitten

## Quellen (kurz)

- Towers-Zitate: Google, wiedergegeben auf localgermany.net
- Dejavu-Zitate: von Google hervorgehobene Auszüge (ohne Anmeldung zeigt Google nur wenige Rezensionen, die meist den Lieferdienst betreffen)
- Illyrian- und MOG‘ 68-Zitate: direkt aus Google Maps (Stand 18.11.2026)
- Alle Namen der Rezensenten gekürzt
- Links: Towers und Illyrian haben laut Google-Profil nur Facebook bzw. Instagram; die bei Dejavu eingetragene Website ist nicht mehr erreichbar; MOG‘ 68 hat keine Website
- Öffnungszeiten Do laut Google Maps (Stand 18.11.2026)
- Fahrzeiten: Näherungswerte über OpenStreetMap/OSRM ab den Ortsmitten Freising, Regensburg und Unterschleißheim, ohne Live-Verkehr

Diese Seite ist unabhängig zusammengestellt und keine offizielle Unternehmensseite.

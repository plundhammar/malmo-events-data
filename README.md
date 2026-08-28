# Malmö Events data

Publik statisk export för mobilklienten. `events.json` innehåller kommande Malmö-event i schema version 1.

## Automatisk uppdatering

När desktopappen hämtar nya event exporterar den automatiskt `events.json`, committar filen och pushar den till detta repo. En separat GitHub deploy key ger enbart detta repo skrivbehörighet.

Mobilklienten ska hämta `events.json` över HTTPS och behålla sin senaste lyckade hämtning lokalt.

## GitHub Pages

När GitHub Pages aktiverats för branchen `main` från `/ (root)` finns flödet på:

```text
https://plundhammar.github.io/malmo-events-data/events.json
```

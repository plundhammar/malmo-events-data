# Malmö Events data

Publik statisk export för mobilklienten. `events.json` innehåller kommande Malmö-event i schema version 1.

## Uppdatera exporten lokalt

Kör från desktopappens projektmapp:

```bash
.venv/bin/python scripts/export_events_json.py ../malmo-events-data/events.json
cd ../malmo-events-data
git add events.json
git commit -m "Uppdatera event"
git push
```

Mobilklienten ska hämta `events.json` över HTTPS och behålla sin senaste lyckade hämtning lokalt.

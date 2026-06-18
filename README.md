# 🌍 Disaster Map

A live map of the Earth showing **real-time natural disasters** — earthquakes, hurricanes & cyclones, volcanoes, wildfires, floods, tsunamis and more.

![Disaster Map](https://img.shields.io/badge/status-live-28e07a) ![No API key](https://img.shields.io/badge/API%20key-not%20required-2bd4ff)

## Features

- **Real-time data, no API keys** — pulls from public feeds and refreshes every 5 minutes:
  - [USGS Earthquake API](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php) — earthquakes (M2.5+, last 24h) and tsunami flags
  - [NASA EONET](https://eonet.gsfc.nasa.gov/) — volcanoes, severe storms/cyclones, wildfires, floods, landslides and other hazards
- **Interactive dark map** with pulsing, color-coded markers (earthquake markers scale with magnitude)
- **Filter panel** — toggle each disaster type on/off with live counts
- **Detailed popups** with location, magnitude, time, source and a link to the full report
- Fully responsive, single self-contained `index.html` — no build step

## Run locally

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## Tech

Plain HTML/CSS/JS + [Leaflet](https://leafletjs.com/) with a CARTO dark basemap. Deployed on Vercel.

## My other projects

- [Universe Map](https://universe-map.vercel.app/) — interactive map of satellites & orbits

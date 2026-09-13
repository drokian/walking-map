# Walking Map

<div align="center">

[![Status](https://img.shields.io/badge/status-prototype-blue)](https://github.com)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Leaflet](https://img.shields.io/badge/Leaflet-Map%20Library-green)](https://leafletjs.com/)
[![OpenStreetMap](https://img.shields.io/badge/OpenStreetMap-Data%20Provider-lightgrey)](https://www.openstreetmap.org/)

</div>

A lightweight interactive map prototype that visualizes how far a person can walk from a train station within a 15-minute radius.

This project helps answer a practical urban planning question: how accessible is a location by foot from nearby transit stations?

<p align="center">
  <img src="https://images.unsplash.com/photo-1524661135-423995f22d0b?auto=format&fit=crop&w=1200&q=80" alt="City map and transit access" width="900" />
</p>

## Why this project?

Walking access is a critical part of urban mobility, livability, and real-estate decision making. This project turns that accessibility into something visible, immediate, and easy to compare.

## Key features

- Real Tokyo station data rendered on a map
- 15-minute walking radius visualization
- Search by station name
- Clickable station list and map selection
- Demo mode with approximate walking area
- Real walking isochrone support via ORS API when an API key is provided
- Interactive popups and labels for selected stations

## Example use cases

- Apartment hunting near transit stations
- Urban planning and access analysis
- Real-estate and commercial location evaluation
- Pedestrian-first neighborhood studies
- Mobility and transport accessibility reviews

## Tech stack

- HTML
- JavaScript
- Leaflet
- OpenStreetMap tiles
- OpenRouteService API

## How it works

1. Open the HTML file in a browser.
2. Station data is loaded from a live source.
3. Search or select a station.
4. The app centers the map on that station and draws a walking area.
5. If an ORS API key is supplied, the app calculates a real walking isochrone; otherwise it falls back to an approximate demo area.

## Run locally

```bash
# Open the HTML file directly in a browser
# or serve it locally with a simple static server
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/tokyo-yurume-haritasi.html
```

## Project status

This is a working prototype focused on concept validation and visual exploration. It is designed to be understandable, easy to extend, and useful for early-stage accessibility analysis.

## Planned improvements

- Add multiple walking durations: 5, 10, 15, 20, and 30 minutes
- Add district and city filters
- Include land-use and station importance layers
- Improve mobile responsiveness
- Expand support to other cities and larger datasets

## License

This project is provided as-is for experimentation and educational use.

## Contributing

Contributions are welcome. If you want to improve the map, expand the data model, or turn this prototype into a more complete accessibility tool, feel free to open an issue or submit a pull request.

## Screenshot

<p align="center">
  <img src="./docs/walking-map-demo.png" alt="Walking Map demo screenshot" width="1000" />
</p>

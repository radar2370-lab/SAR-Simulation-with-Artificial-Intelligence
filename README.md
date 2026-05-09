# SAR Probability Ring Simulator

An interactive web tool for Search and Rescue (SAR) operations that generates ISRID-based probability rings and AI-powered terrain analysis to help locate missing persons.

## Features

- **ISRID-based probability rings** - 25%, 50%, 75%, and 95% probability zones based on Koester's Lost Person Behavior data (150,000+ incident database)
- **17 subject profiles** - Including dementia, autism, lost children (age-stratified), hikers, hunters, climbers, despondent adults, and more
- **Terrain adjustment** - Mountain, dense forest, urban, and flat rural terrain modifiers
- **Interactive map** - Click to set Last Known Point (LKP), with street, topographic, and satellite basemaps
- **AI Terrain Analysis** - Google Gemini-powered polygon search grid generation based on terrain elevation, natural boundaries, and subject behavior
- **CalTopo export** - Download KML or GPX files with all rings, LKP, and AI-generated polygons ready to import into CalTopo
- **Expected behaviors** - ISRID-derived behavior profiles for each subject type to inform search tactics

## How to use

1. Enter a location or click on the map to set the Last Known Point
2. Select subject type, age, terrain, and hours missing
3. Probability rings update automatically
4. Optionally, click "Generate AI Search Polygons" for AI-powered priority zones
5. Export to CalTopo via KML or GPX

## Live demo

Visit the [live tool](https://YOUR-USERNAME.github.io/SAR-Probability-Rings/) (replace with your actual URL).

## Architecture

- **Frontend** - Pure HTML/CSS/JavaScript with Leaflet for mapping (this repository)
- **Backend** - Python Flask API hosted on Render, integrates Google Gemini for AI analysis and Open Topo Data for elevation
- **AI** - Google Gemini 1.5 Flash for terrain analysis and polygon generation

## Data sources

- **ISRID** - International Search & Rescue Incident Database
- **Koester, R.J. (2008)** - *Lost Person Behavior*. dbS Productions
- **OpenStreetMap** - Geocoding and base mapping
- **Open Topo Data** - Elevation data
- **OpenTopoMap, Esri** - Tile providers

## Disclaimer

This tool is in development and uses historic data only. Not recommended for actual operational use. Always rely on certified SAR coordinators and validated tools for live incidents.

## License

MIT License - see [LICENSE](LICENSE) for details.

## Contributing

Built for county Emergency Management and SAR teams. Feedback and pull requests welcome.

# Academic GIS Pro

Academic GIS Pro is a browser-based GIS mapping and cartographic layout tool built with vanilla JavaScript, MapLibre GL, and client-side geospatial utilities.

## Features

- Import and visualize GeoJSON, Shapefile ZIP, and GeoTIFF/TIFF files
- Raster symbology with stretch/classify and terrain-oriented modes
- Vector symbology and labeling controls
- Layout manager with title, legend, north arrow, scale bar, grid, and export
- Export map compositions to PDF, PNG, and JPG
- Offline-friendly fallback behavior for local data workflows

## Tech Stack

- HTML, CSS, JavaScript
- [MapLibre GL JS](https://maplibre.org/)
- [shpjs](https://github.com/calvinmetcalf/shapefile-js)
- [GeoTIFF.js](https://github.com/geotiffjs/geotiff.js)
- [html2canvas](https://html2canvas.hertzen.com/)
- [jsPDF](https://github.com/parallax/jsPDF)

## Run Locally

1. Open a terminal in the project folder.
2. Start a static web server:

```powershell
npx --yes serve -l 5173
```

3. Open:

`http://localhost:5173`

## Project Structure

- `index.html` - Main UI shell
- `style.css` - Theme and layout styling
- `app.js` - Application controller and UI logic
- `map-engine.js` - Map, layer, raster/vector rendering logic
- `layout-engine.js` - Grid, legend, scale, composition helpers
- `export-engine.js` - Export pipeline for PDF/PNG/JPG

## Notes

- This app runs fully client-side.
- Large rasters can require significant browser memory.

## License

This project is licensed under the MIT License - see the `LICENSE` file.

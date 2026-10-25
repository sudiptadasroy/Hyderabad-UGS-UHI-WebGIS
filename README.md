# Hyderabad-UGS-UHI-WebGIS
Interactive Leaflet WebGIS dashboard for Hyderabad Urban Green Spaces (UGS) and Urban Heat Island (UHI) analysis using GIS, remote sensing, GeoServer and spatial data visualization.

# Hyderabad Urban Green Spaces & Urban Heat Island WebGIS

An interactive WebGIS dashboard for exploring the spatial relationship between Urban Green Spaces (UGS) and Urban Heat Island (UHI) patterns in Hyderabad, Telangana, India.

The project combines web mapping, geospatial datasets, remote sensing outputs and spatial analysis in an interactive dashboard built with Leaflet and GeoServer.

## Project Overview

Urban green spaces can influence local land surface temperatures and urban environmental conditions. This project aims to visualize green-space distribution, buffer zones and land surface temperature data to support spatial exploration of urban climate patterns in Hyderabad.

**Project status:** Development in progress. Real-data validation and public deployment are pending.

## Objectives

- Visualize the Hyderabad study-area boundary.
- Map urban parks and green-space locations.
- Display green-space buffer and analysis zones.
- Integrate Land Surface Temperature (LST) raster and GeoServer layers.
- Explore the relationship between vegetation and surface temperature.
- Develop an interactive WebGIS dashboard for spatial analysis.

## Technology Stack

- **Frontend:** HTML, CSS, JavaScript
- **Web mapping:** Leaflet.js
- **Geospatial services:** GeoServer, Web Map Service (WMS)
- **Spatial analysis:** Turf.js
- **Charts:** Chart.js
- **GIS software:** QGIS
- **Remote sensing:** Satellite-derived NDVI and LST products
- **Potential database integration:** PostgreSQL/PostGIS

## Main Features

- Interactive Leaflet map with OpenStreetMap basemap.
- Layer visibility controls.
- Green-space polygons and point locations.
- GeoServer WMS overlay support.
- GeoTIFF raster visualization.
- Dashboard KPI cards and charts.
- Dataset status and inventory panel.
- CSV summary export.

Feature availability depends on the datasets and services configured in the application.

## Project Structure

```text
Hyderabad-UGS-UHI-WebGIS/
├── dashboard/
│   └── app.html
├── data/
│   ├── boundary/
│   └── raster/
├── Leaflet_Dashboard/
│   └── rasters/
│       ├── Buff/
│       ├── Park_Point/
│       ├── Raster1/
│       └── Stat/
├── README.md
└── .gitignore
```

Adjust the folder structure to match the files actually included in the repository.

## Data Sources

The project is designed to use:

- Hyderabad/GHMC administrative boundary data.
- Urban park and green-space vector datasets.
- Green-space buffer and centroid layers.
- Satellite-derived NDVI products.
- Land Surface Temperature (LST) GeoTIFF data.
- GeoServer-published WMS layers.

Add the specific data providers, satellite products, acquisition dates, spatial resolutions and licenses once they have been verified.

## How to Run

1. Clone or download this repository.
2. Open the project folder in Visual Studio Code.
3. Check the dataset paths configured in `dashboard/app.html`.
4. Start a local web server from the project directory. For example:

   ```bash
   python -m http.server 8000
   ```

5. Open `http://localhost:8000/dashboard/app.html` in your browser.
6. Start GeoServer separately if you want to use its WMS layers.
7. Verify that the configured GeoServer URL, workspace, layer names and CORS settings are correct.

A local GeoServer URL such as `http://localhost:8080/geoserver/ows` is accessible only from the same computer. Public deployment requires a publicly reachable server and appropriate security configuration.

## Data Validation

Demo values and simulated features must not be treated as measured environmental results.

Before using the dashboard for research:

- Verify the origin and accuracy of all spatial datasets.
- Replace simulated values with validated analysis outputs.
- Check coordinate reference systems and raster units.
- Document NDVI and LST calculation methods.
- Calculate dashboard statistics from actual data.
- Clearly identify missing datasets and processing limitations.

## Future Improvements

- Integrate validated NDVI and LST statistics.
- Connect PostgreSQL/PostGIS for spatial queries.
- Add date-based comparisons and time-series analysis.
- Improve raster visualization and performance.
- Deploy the frontend and GeoServer online.
- Add data-download and analysis-report functionality.

## Author

**Sudipta Das Roy**  
M.Sc. Geoinformatics  
Interests: GIS Engineering, Remote Sensing, Spatial Data Science and WebGIS.

## License

A license has not yet been selected. Add an appropriate license after checking the ownership and redistribution permissions of the code and datasets.

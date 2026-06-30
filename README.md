# Toronto Neighbourhood Analysis (QGIS)

A spatial analysis of all 140 official City of Toronto neighbourhoods, 
built and styled in QGIS 3.x.

## Overview
- **Source data:** City of Toronto Open Data (Neighbourhood boundary shapefile/GeoJSON)
- **Tool:** QGIS 3.x
- **CRS:** EPSG:3857 (Web Mercator) reprojected from EPSG:4326 (WGS 84)
- **Basemap:** OpenStreetMap XYZ tile layer
- **Layers:** 140 neighbourhood polygons, single symbol fill at 70% opacity,
  labeled with neighbourhood name and area code (AREA_NAME field)

## Workflow
1. Loaded neighbourhood boundary GeoJSON into QGIS
2. Styled using Simple Fill symbology with adjusted opacity and blending
3. Added auto-placed point labels using the AREA_NAME field
4. Exported final map to PNG at 150 DPI using QGIS's Export Map to Image tool

## Files
- `toronto_neighbourhood_analysis.png` — final exported map
- `toronto_neighbourhood_analysis.pgw` — world file for georeferencing the PNG

## Next steps
Planned additions: choropleth analysis by population density and median income, 
using City of Toronto census data joined to the neighbourhood layer.

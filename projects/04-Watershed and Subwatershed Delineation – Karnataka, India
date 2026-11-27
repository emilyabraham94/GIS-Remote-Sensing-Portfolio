Watershed and Subwatershed Delineation – Karnataka, India

Project Overview

This project demonstrates the application of GIS-based hydrological analysis to delineate a watershed and its subwatersheds in Karnataka, India, using a 30 m resolution Digital Elevation Model (DEM).
The analysis focuses on identifying surface water flow pathways, watershed boundaries, drainage networks and contributing areas using QGIS and GRASS GIS.

Objectives

*Delineate watershed boundaries using DEM data.
*Generate flow direction and flow accumulation rasters.
*Identify suitable watershed outlet points.
*Delineate six non-overlapping subwatershed zones.
*Extract and visualise the drainage network.
*Calculate watershed and subwatershed areas.

Data Sources

Dataset: Description

*SRTM DEM: 1 Arc-Second Global, approximately 30 m resolution
*OpenStreetMap: Geographical reference and basemap
*Outlet points: Manually digitised using flow accumulation data
*Coordinate system: WGS 84 / UTM Zone 43N (EPSG:32643)

Software and Tools

*QGIS
*GRASS GIS
*GDAL
*Raster Calculator

Methodology

*DEM acquisition and reprojection to UTM Zone 43N.
*Sink filling and comparison of filled and unfilled DEM processing results.
*Flow direction and flow accumulation generation using the D8 method (r.watershed).
*Conversion of signed flow accumulation values to absolute values.
*Identification and digitisation of watershed outlet points.
*Watershed and individual catchment delineation using r.water.outlet.
*Removal of overlapping catchment areas using conditional raster calculations.
*Raster-to-vector conversion of subwatershed boundaries.
*Flow accumulation reclassification using a threshold of 100,000 cells.
*Drainage network extraction using raster thinning and raster-to-line conversion.
*Area calculation, internal consistency assessment and final map preparation.

The final delineation was based on the drainage direction generated from the unfilled DEM, following a visual comparison of the processing results.

Results

*Parameter: Result
*Total delineated watershed area: 3,805.16 km²
*Number of subwatershed zones: 6
*Number of outlet points: 6
*Raster resolution: 30 m
*Flow routing method: D8
*Drainage extraction threshold: 100,000 cells
*Equivalent contributing area threshold: 90 km²

Subwatershed Areas

Subwatershed: Area (km²)

01: 189.54
02: 730.69
03: 518.04
04: 675.59
05: 1,022.95
06: 668.35

Total: 3,805.16

The combined area of the six non-overlapping subwatershed zones was consistent with the total delineated watershed area.

Final Map: View the full-resolution PDF map

Skills Demonstrated

*Digital Elevation Model processing 
*GIS-based hydrological modelling
*Flow direction and flow accumulation analysis
*Watershed and catchment delineation
*Drainage network extraction
*Raster reclassification and conditional raster calculations
*Raster-to-vector conversion
*Spatial data quality assessment
*Cartographic visualisation and map preparation

Applications

This workflow is relevant to:

*Water resource management
*Watershed management
*Catchment-scale environmental studies
*Flood risk assessment
*Surface runoff analysis
*Hydrological research

Limitations

*The delineated watershed may be partially truncated along the southern boundary due to limited DEM coverage. The extracted drainage network may contain artefacts over flat terrain and water bodies.
*The stream extraction threshold was selected for this exercise rather than calibrated against observed drainage data. Independent validation against reference river networks or field observations was not conducted.
*This project was undertaken as an independent GIS learning and portfolio exercise.

Data Attribution

*DEM: SRTM 1 Arc-Second Global.
*Basemap: © OpenStreetMap contributors — https://www.openstreetmap.org/copyright

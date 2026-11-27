# GIS & Remote Sensing Portfolio

### Geospatial Analysis | Environmental Management | Remote Sensing | Spatial Decision Support

Welcome to my GIS and Remote Sensing portfolio.

This repository showcases my practical projects involving geospatial analysis, environmental assessment, satellite imagery, spatial suitability modelling, machine learning classification, hydrological analysis and GIS-based decision support.

The portfolio will be continuously updated as I complete new projects and develop additional technical skills.

---

## Featured Projects

### 01. Coastal Restoration Priority Mapping — Värmdö, Sweden

**Approach:** Multi-Criteria Decision Analysis (MCDA)

A GIS-based project exploring the prioritisation of coastal restoration areas in the Värmdö archipelago, Sweden.

**Key techniques:**

- Raster processing and spatial analysis
- Bathymetry and ecological indicator assessment
- Multi-Criteria Decision Analysis (MCDA)
- Analytical Hierarchy Process (AHP)
- Weighted overlay and restoration suitability mapping

**Software:** QGIS

[View detailed Coastal Restoration project](projects/01-Varmdo-Coastal-Restoration)

### 02. New Town Site Suitability Analysis

**Approach:** GIS-Based Spatial Suitability Modelling

A spatial planning project investigating the suitability of different locations for potential urban development.

**Key techniques:**

- Spatial buffer analysis
- Environmental constraint mapping
- Spatial suitability assessment
- Land-use planning

**Software:** QGIS

[View detailed Site Suitability project](projects/02-New-Town-Site-Suitability)

### 03. Land Use and Land Cover Classification — Karnataka, India

**Approach:** Supervised Machine Learning Classification

A Landsat 8 (2023) Land Use and Land Cover (LULC) classification project using the Support Vector Machine (SVM) algorithm.

**Key techniques:**

- Multispectral satellite imagery analysis
- Training sample preparation
- Support Vector Machine (SVM) classification
- Stratified validation sampling
- Confusion matrix and accuracy assessment
- Training-validation spatial separation analysis
- Land-cover area statistics
- Python-assisted geospatial analysis
- Thematic land-cover mapping

**Software:** QGIS 4.2.3, Semi-Automatic Classification Plugin (SCP) 9.0.5, Python

**Classification categories:** Water, Cultivation, Bare Agricultural Land, Natural Vegetation, Bare Land with Sparse Vegetation, Fallow Land and Built-Up.

**Key results:**

- 181 training polygons
- 210 stratified validation points
- Seven land-cover classes
- Total mapped area: 778,467.22 hectares
- Observed sample Overall Accuracy: 100%
- Cohen's Kappa: 1.00
- No validation points within 30 metres of training polygons

**Validation note:** The perfect observed agreement represents the assessed sample and does not establish an error-free map. Reference imagery limitations are documented in the project folder.

**Project status:** Classification, mapping, accuracy assessment and area analysis completed.

[View detailed LULC project](projects/03-LULC-SVM-Classification)

### 04. Watershed and Subwatershed Delineation — Karnataka, India

**Approach:** DEM-Based Hydrological Analysis

A GIS-based hydrological modelling project using a 30 m resolution SRTM Digital Elevation Model to delineate watershed boundaries, identify surface water flow pathways and extract drainage networks.

**Key techniques:**

- Digital Elevation Model (DEM) preprocessing
- Sink filling and comparative DEM assessment
- D8 flow direction analysis
- Flow accumulation modelling
- Watershed outlet point identification
- Watershed and subwatershed delineation
- Conditional raster analysis and overlap removal
- Drainage network extraction
- Raster thinning and raster-to-vector conversion
- Catchment area calculation and internal consistency assessment
- Hydrological mapping and cartographic visualisation

**Software:** QGIS, GRASS GIS and GDAL

**Key results:**

- Total delineated watershed area: 3,805.16 km²
- Six non-overlapping subwatershed zones
- Six watershed outlet points
- Spatial resolution: 30 m
- Flow routing method: D8
- Drainage extraction threshold: 100,000 cells
- Equivalent contributing area threshold: 90 km²

**Validation note:** The delineation is constrained by available DEM coverage. The extracted drainage network has not been independently validated against reference river data or field observations.

**Project status:** Hydrological analysis, watershed delineation, drainage extraction, area calculation and mapping completed.

[View detailed Watershed Analysis project](projects/04-Watershed-Analysis)

---

## Technical Skills Demonstrated

### GIS and Spatial Analysis

- Geographic Information Systems (GIS)
- Raster and Vector Data Processing
- Coordinate Reference System Management
- Spatial Buffer and Overlay Analysis
- Spatial Suitability Analysis
- Multi-Criteria Decision Analysis (MCDA)
- Analytical Hierarchy Process (AHP)
- Raster Area Statistics
- Cartographic Visualisation

### Remote Sensing and Machine Learning

- Multispectral Satellite Imagery Analysis
- Supervised Satellite Image Classification
- Support Vector Machine (SVM)
- Training Sample Preparation
- Stratified Validation Sampling
- Classification Accuracy Assessment
- Confusion Matrix Analysis
- Python-Assisted Geospatial Analysis

### Hydrological and Terrain Analysis

- Digital Elevation Model Processing
- Terrain-Based Hydrological Modelling
- Flow Direction and Flow Accumulation Analysis
- Watershed and Subwatershed Delineation
- Catchment Area Assessment
- Drainage Network Extraction
- Conditional Raster Analysis
- Raster Thinning and Vectorisation

## Software & Tools

QGIS | GRASS GIS | Semi-Automatic Classification Plugin (SCP) | Python | PyQGIS | GDAL | NumPy | pandas

## Research and Application Interests

- Environmental Management
- Coastal and Marine Ecosystem Restoration
- Watershed and Water Resource Management
- Land Use and Land Cover Assessment
- Environmental Spatial Modelling
- Sustainable Land-Use Planning
- GIS-Based Environmental Decision Support

## Portfolio Development

This is an evolving portfolio. Future projects will expand into additional applications of GIS, remote sensing, environmental analysis and geospatial data science.

---

*Project maps, detailed methodologies, statistical results, data-source information and limitations are documented in their respective project folders.*

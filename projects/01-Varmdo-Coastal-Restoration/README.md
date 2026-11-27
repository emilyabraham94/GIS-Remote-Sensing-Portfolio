# Värmdö Coastal Restoration Priority Mapping – Sweden

## Project Overview

This project demonstrates the application of Geographic Information Systems (GIS) and Multi-Criteria Decision Analysis (MCDA) to identify priority areas for coastal ecosystem restoration in the Värmdö archipelago, Sweden.

The study explores how ecological, social and economic factors can be integrated into a spatial decision-support framework for sustainable coastal management and marine ecosystem restoration in the Baltic Sea region.

## Objectives

- Identify potential priority areas for coastal ecosystem restoration.
- Integrate ecological, social and economic indicators into a spatial suitability model.
- Apply the Analytical Hierarchy Process (AHP) to determine criterion weights.
- Generate a spatial Restoration Priority Index (RPI).
- Classify coastal areas according to their restoration priority.
- Explore the sensitivity of restoration priorities to changes in criterion weights.

## Study Area

The Värmdö archipelago is located in Stockholm County, Sweden, within the Baltic Sea region. Its coastal environment provides important ecological functions, recreational opportunities and ecosystem services.

## Software and Analytical Tools

- QGIS
- Raster Calculator
- Multi-Criteria Decision Analysis (MCDA)
- Analytical Hierarchy Process (AHP)
- Weighted Overlay Analysis
- Sensitivity Analysis

## Restoration Priority Indicators

### Ecological Criteria

- Benthic Species Potential Index (BSPI)
- Bathymetry and depth suitability
- Eutrophication status

### Social Criteria

- Proximity to population centres
- Proximity to recreational beaches

### Economic Criteria

- Proximity to harbours and boat routes
- Accessibility and infrastructure-related cost proxies

## Methodology

1. Spatial data collection and study area definition.
2. Reprojection of datasets to SWEREF 99 TM (EPSG:3006).
3. Raster clipping, resampling and spatial alignment.
4. Identification and management of NoData values.
5. Normalisation of spatial indicators to a common suitability scale.
6. Application of AHP to determine criterion weights.
7. Integration of ecological, social and economic suitability scores through weighted overlay analysis.
8. Generation of the Restoration Priority Index.
9. Classification of restoration priority zones.
10. Exploration of sensitivity to changes in criterion weights.
11. Final cartographic visualisation and map preparation.

## AHP Criterion Weights

| Criterion | Weight | Percentage |
|---|---:|---:|
| Ecological | 0.6864 | 68.64% |
| Social | 0.2114 | 21.14% |
| Economic | 0.1022 | 10.22% |
| Total | 1.0000 | 100% |

Ecological criteria were assigned the highest importance in the trial weighting scenario to prioritise ecosystem restoration objectives.

## Restoration Priority Index

The Restoration Priority Index integrates the three criterion groups using a weighted linear combination:

**RPI = (Ecological Score × 0.6864) + (Social Score × 0.2114) + (Economic Score × 0.1022)**

The resulting spatial index was classified into four restoration priority categories:

- Low Priority
- Moderate Priority
- High Priority
- Very High Priority

## Results

The project produced a spatial restoration priority map illustrating the relative suitability of coastal areas for potential restoration activities.

The resulting map demonstrates how multiple environmental and socioeconomic considerations can be integrated to support spatial planning and coastal restoration decision-making.

## Technical Specifications

| Parameter | Specification |
|---|---|
| Study area | Värmdö archipelago, Sweden |
| Coordinate reference system | SWEREF 99 TM |
| EPSG code | 3006 |
| Analysis grid resolution | 500 m |
| Decision-making approach | MCDA and AHP |
| Analysis method | Weighted raster overlay |
| Output | Restoration Priority Map |

## Skills Demonstrated

- Coastal and marine spatial analysis
- Environmental suitability modelling
- Multi-Criteria Decision Analysis
- Analytical Hierarchy Process
- Raster data preprocessing
- Spatial data normalisation
- Raster resampling and alignment
- NoData management
- Weighted overlay analysis
- Sensitivity analysis
- Environmental decision-support mapping
- Scientific cartographic visualisation

## Potential Applications

- Coastal ecosystem restoration
- Marine spatial planning
- Marine biodiversity conservation
- Sustainable coastal management
- Ecosystem-based management
- Environmental decision-support systems

## Limitations

The restoration priority results are influenced by spatial data availability, raster resolution, indicator selection and assigned criterion weights.

The AHP weights represent an exploratory weighting scenario rather than priorities established through formal stakeholder consultation.

The economic indicators represent spatial cost proxies rather than actual restoration expenditure.

The resulting priority map is intended as an exploratory decision-support tool and requires further ecological assessment, stakeholder consultation and field validation before practical implementation.

## Project Context

This project was undertaken as an independent GIS learning and research-oriented portfolio exercise to explore spatial decision-support methods for coastal and marine ecosystem restoration.

## Data Attribution

- Baltic Sea environmental datasets, including HOLAS 3 eutrophication data.
- Bathymetric and benthic habitat suitability datasets.
- OpenStreetMap contributors: https://www.openstreetmap.org/copyright


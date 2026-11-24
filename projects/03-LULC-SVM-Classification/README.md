# Land Use and Land Cover Classification Using SVM — Landsat 8 (2023)

## Project overview
This project demonstrates supervised land-use and land-cover (LULC) classification using Landsat 8 multispectral imagery, QGIS and the Support Vector Machine (SVM) algorithm. The objective was to distinguish seven land-cover classes, quantify their mapped areas and assess classification agreement through visual reference interpretation.

## Data and tools
- Landsat 8 imagery (2023), six-band clipped composite
- QGIS and Semi-Automatic Classification Plugin (SCP)
- Python, PyQGIS, GDAL, NumPy and pandas
- Google Satellite imagery and Landsat composite for visual reference interpretation
- 181 training polygons and 210 stratified validation points

## Workflow
1. Prepare the multispectral composite and study-area subset.
2. Digitise training polygons and assign seven land-cover classes.
3. Perform supervised SVM classification.
4. Prepare the final cartographic layout.
5. Visually interpret 30 validation points per mapped class.
6. Check training-validation separation, replace affected points and verify their reference labels.
7. Calculate the confusion matrix, accuracy metrics and mapped class areas.

## Mapped land-cover distribution

| Class | Area (ha) | Coverage (%) |
|---|---:|---:|
| Water | 14,269.34 | 1.83 |
| Cultivation | 158,105.09 | 20.31 |
| Bare Agricultural Land | 289,587.07 | 37.20 |
| Natural Vegetation | 126,870.81 | 16.30 |
| Bare Land with Sparse Vegetation | 22,939.58 | 2.95 |
| Fallow Land | 157,815.95 | 20.27 |
| Built-Up | 8,879.38 | 1.14 |
| **Total** | **778,467.22** | **100.00** |

Bare agricultural land was the dominant mapped class, followed by cultivation and fallow land. Percentages are rounded independently.

## Accuracy assessment

| Metric | Observed result |
|---|---:|
| Validation points | 210 |
| Correctly classified validation points | 210 |
| Sample overall accuracy | 100% |
| Sample Cohen's Kappa | 1.00 |
| Sample producer's and user's accuracy | 100% for each class |
| Area-weighted overall accuracy point estimate | 100% |
| Points within 30 m of training polygons | 0 |

Reference labels were assigned through visual interpretation with the classified raster hidden. Three validation locations were replaced to satisfy the training-separation criterion.

## Limitations
The perfect observed agreement is unusually high and should not be interpreted as proof of an error-free map. Google Satellite imagery dates were not verified against the 2023 Landsat acquisition. The Landsat composite was also used for reference interpretation, so the reference evidence is not entirely independent of the classification inputs. A 30 m separation reduces direct training overlap but does not eliminate spatial autocorrelation. No field-based validation or uncertainty intervals are reported. Mapped class areas are not independently verified true land-cover areas.

## Project outputs
- Final LULC map
- `LULC_Final_Class_Areas.csv`
- `LULC_Final_Confusion_Matrix.csv`
- `LULC_Final_Class_Accuracy.csv`
- `LULC_Final_Accuracy_Summary.csv`
- [Detailed methodology](Methodology.md)

## Skills demonstrated
Multispectral remote sensing, training sample preparation, supervised classification, stratified sampling, spatial validation, accuracy assessment, raster area statistics, Python-assisted GIS analysis and cartographic presentation.

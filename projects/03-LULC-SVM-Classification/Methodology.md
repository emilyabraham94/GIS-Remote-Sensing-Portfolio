# Methodology — Landsat 8 LULC Classification (2023)

## 1. Image preparation
A six-band Landsat 8 multispectral composite was prepared and clipped to the study area in QGIS. The composite was configured as a band set in SCP for supervised classification. Exact scene identifiers, acquisition date, band order and preprocessing parameters should be recorded from the original project metadata before formal publication.

## 2. Training sample preparation
Training polygons were digitised through visual interpretation of satellite imagery. The original set contained 184 polygons; the final classification used 181 after filtering. Seven class codes were assigned:

| Code | Class | Interpretation |
|---|---|---|
| 1 | Water | Water-covered surfaces |
| 2 | Cultivation | Actively vegetated agricultural fields |
| 3 | Bare Agricultural Land | Harvested or ploughed agricultural fields |
| 4 | Natural Vegetation | Non-cultivated vegetation |
| 5 | Bare Land with Sparse Vegetation | Bare or unused land with limited vegetation |
| 6 | Fallow Land | Temporarily uncultivated agricultural land |
| 7 | Built-Up | Developed surfaces and settlements |

## 3. Supervised classification
Support Vector Machine (SVM) classification was performed using SCP and the six-band composite. SVM uses training observations to learn decision boundaries between classes in spectral feature space. The final classified raster contains seven thematic classes. Exact SVM kernel and hyperparameter settings were not established in the available project record and are therefore not claimed here.

## 4. Validation sampling and reference interpretation
A stratified validation sample of 210 points was generated, with 30 points per mapped class. Reference classes were manually assigned using Google Satellite imagery and the clipped Landsat composite, with the SVM classified raster hidden during visual interpretation.

## 5. Training-validation separation
PyQGIS was used to compare validation point geometries against the 181 training polygons. Two points (17 and 27) intersected training polygons and were replaced. A subsequent 30 m buffer check identified one additional point (5), which was also replaced. Replacement locations were randomly selected from the same mapped class, outside the training buffers, and visually reinterpreted. All three replacement reference labels were Water.

The final dataset contained 210 points, zero missing reference labels and zero points intersecting the 30 m training buffers. This is a spatial separation criterion, not proof of complete statistical independence.

## 6. Accuracy assessment
A confusion matrix was generated in Python using pandas and NumPy, with reference classes in rows and mapped classes in columns.

- Overall accuracy (OA): correctly classified points divided by total validation points.
- Producer's accuracy (PA): diagonal count divided by the reference-class row total in the sample matrix.
- User's accuracy (UA): diagonal count divided by the mapped-class column total.
- Cohen's Kappa: (observed agreement − expected agreement) / (1 − expected agreement).

All seven diagonal counts were 30 and all off-diagonal counts were zero. The sample OA was 100%, sample Kappa was 1.00, and sample PA and UA were 100% for every class. These are observed sample statistics.

## 7. Raster area calculation
GDAL and NumPy were used to count raster pixels for each of the seven class codes. Pixel area was calculated from the absolute determinant of the raster geotransform, using projected metre-based coordinates. The reported pixel area was approximately 899.916 m². Class area in hectares equals pixel count multiplied by pixel area and divided by 10,000. Coverage percentage equals class area divided by total classified area, multiplied by 100. Only the seven mapped class codes were included in the area totals.

The total classified area was 778,467.22 ha (approximately 7,784.67 km²).

## 8. Area-weighted accuracy
Because equal numbers of validation points were sampled from classes with unequal mapped areas, area-weighted overall accuracy was calculated conceptually as the sum of each mapped class area proportion multiplied by its observed user's accuracy. All observed user's accuracies were 1.0, so the area-weighted OA point estimate was also 100%. No confidence interval was calculated; the absence of observed errors does not establish zero population error.

## 9. Cartographic output and reporting
The final LULC map was prepared in QGIS. Class-area statistics, confusion matrix, class-wise accuracy and overall accuracy summary were exported as CSV files.

## 10. Limitations and reproducibility
- Reference imagery dates were not verified against the 2023 Landsat acquisition; seasonal agricultural changes may affect interpretation.
- Visual reference interpretation is subject to interpreter uncertainty, especially for spectrally similar agricultural classes.
- The Landsat composite was used both for classification and reference interpretation, limiting independence of the reference evidence.
- Training separation does not eliminate spatial autocorrelation.
- Perfect observed agreement is unusual and warrants further independent validation using date-matched imagery or field observations.
- The replacement procedure excludes training-buffer locations from the validation sampling frame; accuracy for excluded areas is not directly assessed by this sample.
- Exact scene metadata, study-area name and boundary source, preprocessing details and SVM settings should be documented from the original QGIS project before formal publication.

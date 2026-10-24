# GEOM7001 — Data Processing Log (Jupyter notebooks)

These notebooks document the research processing and modelling workflow for Sentinel-2 optical, Sentinel-1 SAR, and Landsat-derived FVC at New Acland Coal Mine.

## Reading order

1. `01_EO_Preprocessing.ipynb` — optical indices, SAR ingestion, Landsat FVC preparation and alignment.
2. `02_Random_Forest_Modelling.ipynb` — spatial samples, Random Forest models, holdout evaluation and spatial cross-validation.
3. `03_Model_Analysis.ipynb` — analysis of model results and visualisations.
4. `04_Full_Area_Prediction.ipynb` — spatial predictions and mapping.
5. `05_One_Year_Prediction_Reproduction.ipynb` — supplementary reproduction of 1-year model predictions.

## Reproducibility and limitations

- These are **organised copies of the original research notebooks**, not newly executed or fully validated workflows.
- The notebooks depend on external input data, intermediate NetCDF/CSV files, the study-area polygon, and the DEA Sandbox / Google Earth Engine processing environment. Those large inputs are **not bundled**.
- Previously saved outputs have been retained where available; saved outputs are not proof that all cells currently execute sequentially.
- Two observed `NameError` issues in diagnostic/memory-cleanup cells were addressed conservatively. The scientific modelling code and saved model metrics were not intentionally altered.
- An earlier alternative one-year notebook version was not included to avoid duplicate submissions; originals are retained separately.
- To reproduce the analysis, restore the original input paths and compatible software environment, then run notebooks in order.

## Review notes

### 01_EO_Preprocessing.ipynb (103 cells)
- Warning: Cell 2: syntax issue invalid syntax (line 1)

### 02_Random_Forest_Modelling.ipynb (132 cells)
- Edit: Made optional memory cleanup robust to variables already deleted.
- Edit: Removed stale error output from corrected cell 114.

### 03_Model_Analysis.ipynb (51 cells)
- Edit: Removed reference to undefined test_idx in preliminary diagnostic cell 5.
- Edit: Removed stale error output from corrected cell 5.

### 04_Full_Area_Prediction.ipynb (26 cells)
- No known saved exception outputs or Python syntax errors detected.

### 05_One_Year_Prediction_Reproduction.ipynb (15 cells)
- No known saved exception outputs or Python syntax errors detected.


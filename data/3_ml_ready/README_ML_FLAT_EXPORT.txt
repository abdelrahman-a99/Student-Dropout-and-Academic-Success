ML-ready analytical table exported from the Power BI data warehouse.

File:
- ML_StudentOutcome_Flat.csv

Shape:
- 4424 student records.
- 44 columns:
  - 36 original predictor features.
  - 6 DWH surrogate keys.
  - Target.
  - TargetEncoded.

Python preparation notebook:
_02_Data_Cleaning_Preprocessing/02_powerbi_ml_ready_preprocessing.ipynb

The notebook excludes surrogate keys and target columns from the
predictor features, then creates the shared stratified train/test split.

This exported CSV allows the Python experiments to run without
refreshing the Power BI project first.
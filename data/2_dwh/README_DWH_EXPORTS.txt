Power BI / Power Query data warehouse exports.

Fact table:
- Fact_StudentOutcome.csv: 4424 rows, one row per student.

Dimension tables:
- Dim_Student.csv: 4424 rows.
- Dim_Admission.csv: 3660 rows.
- Dim_Course.csv: 17 rows.
- Dim_Financial.csv: 8 rows.
- Dim_AcademicPerformance.csv: 3821 rows.
- Dim_EconomicContext.csv: 10 rows.

Dimension keys are unique in the supplied exports.
All fact-table foreign keys match existing dimension keys.

Target mapping:
- Dropout: 0
- Enrolled: 1
- Graduate: 2

Power BI project:
- DWH_Phase_One.pbix

The analytical flat-table export is stored separately:
data/3_ml_ready/ML_StudentOutcome_Flat.csv
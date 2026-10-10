# Enhanced multiple linear regression for vehicle CO₂

This is an improved, thoroughly explained successor to the lecturer-provided `multiple linear regression.ipynb`. It retains the original 1,022-row CSV and uses cleaned modelling data derived from it. The notebook teaches simple-versus-multiple regression, source data quality, avoiding duplicate leakage, group-based train/test separation, model evaluation, manual prediction, coefficient interpretation, cross-validation and new vehicle scenarios.

## Run
1. Keep notebook and CSV files in one folder.
2. Install `pip install -r requirements.txt`.
3. Open `CO2_Multiple_Linear_Regression_Enhanced.ipynb` and select *Run All*.
4. Review inline output figures and generated CSVs/PNGs.

See `DATA_DICTIONARY.md` for provenance and data choices. The CO₂ unit and original source are not verified. The provided vehicle scenarios are simulated **inputs** only, not fabricated labelled emissions records.

## Evaluation
This is regression, so use MAE, RMSE and R²—not accuracy, precision, recall or confusion matrices.

**Course connection:** OMC9000UK7, Lecture 4 concepts and Lecture 5 regression practice; MLO1/MLO3; MLO4 extension.

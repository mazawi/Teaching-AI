# Data dictionary / change log

## Provenance
Original uploaded source: `CO2_sum.csv`, 1,022 rows. Original notebook contained three code cells: load, fit two-predictor LinearRegression, predict [2.3,4]. Source units and measurement methodology are not established in the provided files.

## Original fields
- make: vehicle brand/manufacturer text.
- model: model text.
- eng_size: engine-size numeric value; original source does not state unit explicitly.
- cylender: original source typo for cylinder count.
- co2: recorded numerical CO₂ outcome; original source does not state unit explicitly.

## Added and transformed fields
- cylinders: renamed from cylender.
- source_row: original row number (1-based) retained for traceability.
- duplicate_exact: whether the row repeats a previous complete source record after text standardisation.
- vehicle_family: uppercase make and model concatenated for grouped evaluation.
- engine_per_cylinder: exploratory derived ratio, NOT used in baseline multiple regression.

## Delivered datasets
- CO2_sum_original.csv: unchanged original, 1,022 rows.
- CO2_cleaned_all_records.csv: all source records, cleaned text, metadata and flags.
- CO2_modeling_unique.csv: first occurrence of each repeated complete observation, for teaching the estimation workflow.
- CO2_new_vehicle_scenarios.csv: 10 hypothetical combinations of engine size/cylinders, without invented CO₂ ground truth.

Dataset duplicates can represent truly repeated specifications; we do not claim the rows are invalid. Engine size and cylinder count show substantial correlation. No extra labelled vehicle measurements were fabricated.

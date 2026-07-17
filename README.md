# Author: Keith Howen

## What this repo is

A short-term University end-to-end Healthcare Data Science Project to curate datasets for a Supervised Machine Learning task to predict 30-day ICU readmission among Coronary Heart Disease patients.

Patient data is obtained from de-identified Electronic Health Records (EHRs) in the MIMIC-IV healthcare database, and is stored in BigQuery, where SQL queries and exports were also done. 


## Key files and folders

1. `data/curated/merged_chd_model_v2.csv` is the merged CHD dataset we use for modelling. `data/curated/merged_chd_model_full_v2.csv` is similar except it contains additional flags for Myocardial Infraction subtypes.

2. All notebooks end with a team member's first name, reflecting the authors responsible for developing the code in the notebook.

3. All files prefixed with `models/manual_mlp_clip*` are outputs (model and metadata) from the hyperparameter tuning workflow present in the `notebooks/MLP_full_workflow_keith.ipynb` notebook. 

4. `docs/` include all human-facing documents related to this project, which includes meeting notes and the final written report compiling our results.

## Note on code structure

All scripts are embedded in `.ipynb` Jupyter Notebooks due to the short-term nature of this project. However, code refactors may be considered in the future to make this project reproducible and production-like.
# Unequal Urban Transition Positions under a Shared Carbon-Peaking Deadline

This repository contains analysis code, aggregated result tables, and input-data documentation associated with the study.

Repository  
https://github.com/hizhukai/Unequal-urban-transition-positions-under-a-shared-carbon-peaking-deadline

## Contents

- `code/` contains the trajectory, peaking-status, predictor-attribution, scenario, backtesting, sensitivity, and ordering analyses.
- `results/` contains pathway-level and model-level summaries used in the manuscript and Supporting Information.
- `data/README.md` and `data/input_schema.csv` describe the input fields and source roles.
- `requirements.txt` lists the Python dependencies.

## Data and results

The underlying CEADs, EDGAR, and municipal statistical-yearbook materials were obtained from the original providers cited in the manuscript. Source workbooks, city-year input panels, city-level assignments, and intermediate trajectories are not included in this repository. The result tables contain aggregated pathway-level and model-level values.

Historical observations and simulated trajectory shares are identified with separate field names. Simulated shares describe the proportion of simulated trajectories reaching a turning point under the stated scenario settings.

## Analysis code

The main analysis follows `s1_data_preparation.py`, `s2_dtw_clustering.py`, `s3_peak_detection.py`, `s4_xgboost_shap.py`, and `s5_monte_carlo.py`. Supplementary scripts provide external label transfer, city-level backtesting, parameter sensitivity, and post-2019 ordering checks. The scripts use the input schema documented in `data/input_schema.csv` and write intermediate files to `runtime_output/`.

## Data availability

The code and aggregated result tables supporting this study are available at the repository URL above. The underlying source materials are available from the original providers cited in the manuscript and are not redistributed here.

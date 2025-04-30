This repository contains postprocessed data and Python scripts used for the analyses presented in the manuscript:

**"Vertically Varying Cloud Responses to Southern Hemisphere Jet Shifts and Their Role in Southern Annular Mode Persistence in Observations and CMIP6 Models"**

---

## 📁 Repository Structure

### `data/`
This folder contains the processed datasets used in the analysis:

- `SAM_ACRE_index_models_with_obs.pkl` — Jet–ACRE index from AMIP model runs and CERES observations  
- `sam_monthly_2000_2014.pkl` — Monthly Southern Annular Mode (SAM) index from 2000–2014  
- `sam_daily_2000_2014.pkl` — Daily SAM index from 2000–2014  
- `CRH_LW_CloudSat_combined.nc` — 5-day binned mean cloud radiative heating (CRH) from CloudSat/CALIPSO satellite data  
- `regression_maps_cloud_fraction.pkl` — Regression maps of cloud fraction against SAM
- `regression_maps_cloud_fraction_p_values.pkl` — Corresponding p-values for cloud fraction regressions  
- `regression_maps_crh.pkl` — Regression maps of CRH against SAM
- `regression_maps_crh_p_values.pkl` — Corresponding p-values for CRH regressions  

---

### `scripts/`
This folder contains Python notebooks and modules for reproducing the figures and results:

- `calculate_SAM_indices.ipynb` — Computes the SAM index and persistence index across datasets  
- `calculate_jet_ACRE.ipynb` — Computes the jet–ACRE relationship for MERRA2 and CMIP6 models  
- `calculate_CL_CRH-SAM.ipynb` — Calculates regression between cloud/CRH anomalies and the SAM index  
- `calculate_CRH_models.ipynb` — Calculates CRH data for models  
- `plot_figure1&4.ipynb` — Scripts to generate Figures 1 and 4  
- `plot_figure2.ipynb` — Script to generate Figure 2  
- `plot_figure3.ipynb` — Script to generate Figure 3  
- `read_cloudsat_each_year.ipynb` — Reads and processes CloudSat data  
- `util.py` — Utility functions used throughout the analysis  
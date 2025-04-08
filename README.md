# Cloud Response to Jet Shifts: Data and Analysis Scripts

This repository contains postprocessed data files from CloudSat, MERRA2, and CMIP6, along with Python scripts used to analyze these datasets for the manuscript:

**"Vertically Varying Cloud Responses to Southern Hemisphere Jet Shifts and Their Role in Southern Annular Mode Persistence in Observations and CMIP6 Models"**

---

## 📂 Repository Structure

### `data/`
This folder includes the key datasets used in the analysis:

- `SAM_ACRE_index_models_monthly.pkl`: Jet–ACRE index from AMIP model runs.
- `sam_monthly_2000_2014.pkl`: Monthly Southern Annular Mode (SAM) index from 2000–2014.
- `sam_daily_2000_2014.pkl`: Daily SAM index from 2000–2014.
- `SAM_persistence_index.pkl`: SAM persistence index.
- Binned 5-day mean cloud radiative heating (CRH) from CloudSat/CALIPSO satellite data.
- Interpolated monthly CRH fields from:
  - MERRA2 reanalysis
  - CMIP6 model simulations

---

### `scripts/`
Python notebooks and modules for reproducing the analysis:

- `calculate_SAM_indices.ipynb`: Computes the SAM index and persistence index across all datasets.
- `calculate_jet_ACRE.ipynb`: Computes the jet–ACRE relationship for MERRA2 and CMIP6 models.
- `util.py`: Utility functions used throughout the analysis.
- `figure1.ipynb` through `figure4.ipynb`: Scripts to generate Figures 1–4 in the manuscript.

---

## 🔧 Requirements

To run the scripts, you will need Python 3 and the following libraries:
- `numpy`
- `pandas`
- `xarray`
- `matplotlib`
- `seaborn`
- `netCDF4`

You can install the requirements using:
```bash
pip install -r requirements.txt

# Midterm Project — Decision Trees on Breast Cancer Diagnostic (WDBC)

**Author:** Palden Arya  
**Date:** 2025-10-20

This repository contains a complete, reproducible pipeline for a midterm classification project
with numeric features and a categorical target (malignant vs benign).

## Contents
- `midterm.ipynb`: Main notebook (Colab-ready).
- `requirements.txt`: Dependencies.
- `figures/`: Generated plots (created at runtime).
- `outputs/`: Metrics and artifacts (JSON, optional PDF).

## Quick start (Colab)
1. Upload `midterm.ipynb` to Google Drive and open with **Google Colab**.
2. (Optional) Run the first cell to install dependencies.
3. Run all cells. Figures and outputs will be created in `./figures` and `./outputs`.

## Quick start (local)
```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab  # or jupyter notebook
```
Open `midterm.ipynb` and run all cells.

## Notes
- Dataset is loaded via `sklearn.datasets.load_breast_cancer` (UCI source).
- Decision Tree models: low-complexity, high/unrestricted, and medium (GridSearchCV).
- Evaluation includes accuracy, balanced accuracy, precision, recall, confusion matrix, and bootstrap 95% CIs.

# Practical Lab 2 — Diabetes Progression Modeling (Scikit‑Learn Diabetes)

This repository contains a complete ML report notebook for predicting **diabetes disease progression one year after baseline** using the Scikit‑Learn diabetes dataset.

## What’s inside the notebook
**Part 1**
- Problem framing (regression + screening classification context)
- EDA: summary statistics, histograms, scatter plots, correlation matrix
- Train/validation/test split (75% / 10% / 15%)

**Part 2 (Univariate)**
- Polynomial regression on **BMI** for degrees **0 to 5**
- Model comparison table on train/validation (R², MAE, MAPE)
- Best model selection + test metrics
- Best‑fit plot (train/val/test points + curve)
- Model equation, example prediction, and parameter count

**Part 3 (Multivariate)**
- 2 Polynomial models (deg=2 and deg=3)
- 2 Decision Trees (max_depth=3 and 6)
- 2 kNN models (k=5 and 15)
- 2 Logistic Regression screening models (C=1.0 and 0.1), evaluated on probabilities

## Files
- `Practical_Lab_2_Diabetes_FINAL_CLEAN.ipynb` — main notebook
- `requirements.txt` — dependencies
- `README.md` — this file

## How to run (VS Code / Jupyter)
```bash
pip install -r requirements.txt
```
Open the notebook and run cells from top to bottom.

## Notes
- The dataset is loaded directly from `sklearn.datasets.load_diabetes(as_frame=True)` (no CSV needed).
- Metrics used throughout: **R²**, **MAE**, **MAPE**.
- Logistic Regression is used as a **screening classifier** by converting the continuous target into a binary label using the **training median** threshold, and then evaluating predicted probabilities.

## Author
- Param Avinashkumar Rasaniya, Student ID: 9086095
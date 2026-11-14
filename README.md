# Reweighing – Algorithmic Fairness

This repository contains the implementation and evaluation of the Reweighing bias mitigation method for Data Wrangling Assignment 4.

## Datasets

The experiment uses three publicly available datasets: Adult Census Income, German Credit, and COMPAS.

The datasets are downloaded automatically using `kagglehub` and `ucimlrepo`.

## Requirements

The analysis was developed in Google Colab using Python.

The notebook uses pandas, NumPy, scikit-learn, kagglehub, and ucimlrepo. The required additional packages are installed in the notebook.

## How to reproduce the results

1. Open `DW_assignment_4.ipynb` in Google Colab.
2. Select **Runtime → Run all** to execute all cells in order.
3. Allow the notebook to install the required packages and download the datasets.
4. Wait for the analysis to finish. The results will appear below the code cells.

An internet connection is required to download the datasets.

## Methodology

The notebook calculates Demographic Parity Difference, Disparate Impact Ratio, and Consistency for the original datasets. It then uses an 80/20 stratified train/test split with `random_state=42`.

Baseline Logistic Regression models are compared with models trained using Reweighing sample weights. Both approaches are evaluated using accuracy and the three fairness metrics.

Consistency is calculated using five nearest neighbors.

## Results

The notebook presents the fairness metrics before training and compares baseline and Reweighing predictions on the held-out test sets for all three datasets.# Reweighing-Fairness-Analysis
Evaluation of the Reweighing Bias mitigation method on Adult, German Credit and COMPAS datastets.

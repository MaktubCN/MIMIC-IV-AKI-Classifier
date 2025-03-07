# MIMIC-IV AKI Classifier

![GitHub repo size](https://img.shields.io/github/repo-size/MakiuhCN/MIMIC-IV-AKI-Classifier)  
![GitHub last commit](https://img.shields.io/github/last-commit/MakiuhCN/MIMIC-IV-AKI-Classifier)

## Overview

This repository contains the code and documentation for a predictive modeling project aimed at classifying the most severe **Acute Kidney Injury (AKI)** stage a patient reaches during their ICU stay using first-day ICU data from the **MIMIC-IV** dataset. The project was developed as part of the *Advanced Statistical Learning - Assignment 1* at the National University of Singapore (Mar 2025).

The goal is to predict AKI stages (0 = No AKI, 1-3 = Increasing severity levels) by leveraging machine learning techniques, with a focus on early detection to improve clinical decision-making and patient outcomes in critical care settings. The final model, a tuned **XGBoost classifier**, achieves a test set accuracy of **0.48** and an AUC-ROC of **0.7025**.

For more details, refer to the accompanying paper: *Predictive Modeling for Classifying Acute Kidney Injury Stages Using First-Day ICU Data*.

## Repository Contents

- **`mimiciv_data_dictionary.md`**: A detailed data dictionary describing the features in the MIMIC-IV dataset used for this project, including identifiers, outcomes, demographics, vital signs, blood gas parameters, laboratory results, and more.
- **`MIMIC-IV-AKI-Classifier.ipynb`**: The Jupyter Notebook containing the full pipeline for data preprocessing, feature selection, model development, and evaluation. It includes implementations of Random Forest, XGBoost, LightGBM, Logistic Regression, and AdaBoost, with Bayesian Optimization for hyperparameter tuning.

## Prerequisites

To run the code in this repository, ensure you have the following installed:

- Python 3.8+

- Required libraries:

  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm statsmodels bayesian-optimization
  ```

- Access to the MIMIC-IV dataset (available via [PhysioNet](https://physionet.org/content/mimiciv/2.2/)). You need to place the dataset file (`sph6004_assignment1_data.csv`) in the working directory.

## Usage

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/MakiuhCN/MIMIC-IV-AKI-Classifier.git
   cd MIMIC-IV-AKI-Classifier
   ```

2. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Notebook**:

   - Open `MIMIC-IV-AKI-Classifier.ipynb` in Jupyter Notebook or JupyterLab.
   - Ensure the MIMIC-IV dataset (`sph6004_assignment1_data.csv`) is in the same directory.
   - Execute the cells sequentially to preprocess data, train models, and evaluate results.

## Data

The dataset used is from [MIMIC-IV](https://physionet.org/content/mimiciv/2.2/#files), containing first-day ICU patient records with features like vital signs, lab results, and demographics. The target variable is `aki_stage` (0-3). See `mimiciv_data_dictionary.md` for a complete description.

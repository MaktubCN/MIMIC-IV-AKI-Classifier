# MIMIC-AKI-Classifier

## Overview
This repository contains a machine learning project designed to classify the most severe Acute Kidney Injury (AKI) stage a patient reaches during their ICU stay, using first-day ICU patient data from the MIMIC-IV dataset. The project implements a comprehensive pipeline including data preprocessing, feature selection, and model evaluation, with a focus on ensemble methods such as XGBoost and LightGBM. After Bayesian Optimization for hyperparameter tuning, XGBoost was selected as the final model, achieving a macro-average AUC-ROC of 0.7025 and a test set accuracy of 0.48. This work aims to support early AKI detection in critical care settings, contributing to improved clinical decision-making and patient outcomes.

## Features
- **Dataset**: Utilizes first-day ICU data from MIMIC-IV, filtered for patients aged 18–89.
- **Target Variable**: Classifies AKI stages into four categories (0 = No AKI, 1 = Stage 1, 2 = Stage 2, 3 = Stage 3).

![data-flow](https://github.com/user-attachments/assets/175648fe-8e65-41dd-b448-8f68524217ed)

![importance_all](https://github.com/user-attachments/assets/b769f9b5-66f2-4822-8a49-5a83ab9e5b02)


- **Methodology**: Includes Random Forest for feature selection, five ML models (Random Forest, XGBoost, LightGBM, Logistic Regression, AdaBoost), and Bayesian Optimization for tuning.

![ROC_Comparison](https://github.com/user-attachments/assets/75e22517-5d88-45ab-9a18-ac3aab3e8a1f)

- **Results**: XGBoost outperforms with an optimized AUC of 0.7025, validated on a 20% test set.

![coverage](https://github.com/user-attachments/assets/5e7370ea-67f2-4530-9b42-c35ae7580bca)

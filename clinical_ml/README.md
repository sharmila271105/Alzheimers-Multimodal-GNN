# Clinical Machine Learning Module

## Overview

This module contains the complete clinical analysis pipeline for Alzheimer's Disease classification using the OASIS-1 Cross Sectional dataset.

The objective is to evaluate the predictive power of demographic, cognitive, and MRI-derived biomarker features before integrating MRI image embeddings in the multimodal framework.

---

## Dataset

Features used include:

* Age
* Gender
* Education (EDUC)
* Socioeconomic Status (SES)
* MMSE
* CDR
* eTIV
* nWBV
* ASF

Target:

* Alzheimer's Disease Classification

---

## Workflow

### 1. Data Preprocessing

File: `OASIS_Preprocessing.ipynb`

Tasks:

* Data cleaning
* Missing value handling
* Feature selection
* Encoding categorical variables
* Data preparation for modeling

---

### 2. Exploratory Data Analysis

File: `OASIS_EDA.ipynb`

Tasks:

* Dataset overview
* Missing value analysis
* Class distribution analysis
* Correlation analysis
* Initial feature investigation

---

### 3. Feature Distribution Analysis

File: `OASIS_Distributions.ipynb`

Tasks:

* Histograms
* Density plots
* Boxplots
* Feature-wise comparison across classes

---

### 4. Baseline Machine Learning Models

File: `OASIS_Baseline_Models.ipynb`

Models:

* Logistic Regression
* Random Forest
* XGBoost

Evaluation:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC
* Confusion Matrix

---

### 5. SMOTE Experiments

File: `OASIS_SMOTE_Experiment.ipynb`

Tasks:

* Class imbalance analysis
* SMOTE oversampling
* Model retraining
* Performance comparison

---

### 6. Explainable AI

File: `OASIS_SHAP_Explainability.ipynb`

Tasks:

* SHAP feature importance
* SHAP summary plots
* SHAP beeswarm plots
* Model interpretability analysis

---

## Folder Structure

| Notebook                        | Description                      |
| ------------------------------- | -------------------------------- |
| OASIS_Preprocessing.ipynb       | Data cleaning and preparation    |
| OASIS_EDA.ipynb                 | Exploratory Data Analysis        |
| OASIS_Distributions.ipynb       | Feature distribution analysis    |
| OASIS_Baseline_Models.ipynb     | Baseline machine learning models |
| OASIS_SMOTE_Experiment.ipynb    | Class balancing experiments      |
| OASIS_SHAP_Explainability.ipynb | Explainable AI analysis          |

---

## Outputs

This module produces:

* Cleaned clinical dataset
* Baseline classification models
* SMOTE-balanced experiments
* SHAP explainability reports
* Feature importance rankings

These outputs form the first modality of the overall multimodal Alzheimer's Disease classification framework.

Subsequent modules will incorporate:

1. MRI Image Analysis (CNN)
2. Multimodal Feature Fusion
3. Graph Neural Networks (GCN/GAT)
4. Final Multimodal Alzheimer's Classification System

# Multimodal Feature Fusion

## Objective

Combine clinical features and MRI-derived embeddings into a unified subject-level representation.

## Notebooks

* 01_Merge_Modalities.ipynb
* 02_Fusion_Baseline.ipynb

## Modalities

### Clinical Features

* Age
* Gender
* EDUC
* SES
* MMSE
* CDR
* eTIV
* nWBV
* ASF

### MRI Features

* 512-dimensional ResNet18 embeddings

## Models Evaluated

* Random Forest
* XGBoost

## Results

| Model         | Macro-F1 |
| ------------- | -------: |
| Random Forest |    0.858 |
| XGBoost       |    0.858 |

## Key Inference

Combining MRI representations with clinical biomarkers significantly improved performance over unimodal approaches, demonstrating the value of multimodal learning.


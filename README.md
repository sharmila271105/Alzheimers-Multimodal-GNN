# Alzheimer's Disease Classification using Multimodal Learning and Graph Neural Networks

## Overview

This project presents a multimodal framework for Alzheimer's Disease classification by integrating clinical biomarkers, cognitive assessments, and MRI-derived deep features.

The objective is to investigate whether combining multiple modalities and modeling inter-subject relationships using Graph Convolutional Networks (GCNs) can improve classification performance compared to traditional machine learning and unimodal approaches.

---

## Dataset

**OASIS-1 Cross-Sectional Dataset**

The dataset contains 347 subjects with:

### Clinical & Cognitive Features

* Age
* Gender
* Education (EDUC)
* Socioeconomic Status (SES)
* MMSE
* CDR

### MRI-Derived Biomarkers

* eTIV
* nWBV
* ASF

### Structural MRI Scans

* T1-weighted brain MRI images

---

## Methodology

### 1. Clinical Machine Learning

* Data preprocessing
* Exploratory Data Analysis (EDA)
* Class imbalance handling
* SHAP explainability

Models:

* Logistic Regression
* Random Forest
* XGBoost

---

### 2. MRI Feature Extraction

* Transfer Learning using ResNet18
* MRI image classification
* Extraction of 512-dimensional feature embeddings

---

### 3. Multimodal Fusion

Clinical and MRI-derived features were combined to create a unified subject-level representation.

Models:

* Random Forest
* XGBoost

---

### 4. Graph Neural Networks

A subject similarity graph was constructed using K-Nearest Neighbors (KNN).

Model:

* Graph Convolutional Network (GCN)

Purpose:

* Capture relationships between similar subjects
* Improve multimodal classification performance

---

## Project Pipeline

```text
Clinical Features
        +
MRI Scans
        ↓
    ResNet18
        ↓
 MRI Embeddings
        ↓
 Multimodal Fusion
        ↓
    KNN Graph
        ↓
       GCN
        ↓
 Alzheimer's Classification
```

---

## Results

| Model                        |  Macro-F1 |
| ---------------------------- | --------: |
| Clinical Logistic Regression |     0.780 |
| Clinical Random Forest       |     0.820 |
| Clinical XGBoost             |     0.840 |
| MRI CNN (ResNet18)           |     0.594 |
| Fusion Random Forest         |     0.858 |
| Fusion XGBoost               |     0.858 |
| **GCN**                      | **0.910** |

### Key Findings

* Clinical features alone provided strong predictive performance.
* MRI embeddings improved classification when fused with clinical data.
* Graph-based learning further improved performance by leveraging inter-subject relationships.
* The proposed GCN framework achieved the highest Macro-F1 score of **0.910**.

---

## Repository Structure

```text
clinical_ml/    -> Clinical ML pipeline and SHAP analysis
mri_cnn/        -> MRI classification and feature extraction
fusion/         -> Multimodal feature fusion
gcn/            -> Graph Neural Network implementation
results/        -> Figures and evaluation results
report/         -> Project report and documentation
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* XGBoost
* PyTorch
* Torchvision
* PyTorch Geometric
* SHAP
* Matplotlib
* Seaborn

---

## Future Work

* Graph Attention Networks (GAT)
* Transformer-based multimodal fusion
* Integration of PET/fMRI modalities
* Longitudinal disease progression modeling

---

## Author

SHARMILA DEVI PK 
B.Tech Electrical and Electronics Engineering
National Institute of Technology Tiruchirappalli (NIT Trichy)


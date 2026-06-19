# Alzheimer's Multimodal GNN

A multimodal Alzheimer's Disease classification framework using clinical biomarkers, cognitive assessments, and structural MRI scans from the OASIS-1 Cross-Sectional Dataset.

## Modalities Used

### 1. Clinical & Cognitive Features

* Age
* Gender
* Education (EDUC)
* Socioeconomic Status (SES)
* MMSE
* CDR

### 2. MRI Biomarkers

* eTIV
* nWBV
* ASF

### 3. Structural MRI Scans

* T1-weighted MRI images
* CNN-based feature extraction using ResNet18

The same subjects are matched across both the clinical dataset and MRI dataset before multimodal fusion.

---

## Project Pipeline

```text
Clinical Features + MRI Biomarkers
                │
                ▼
      Clinical ML Analysis
                │
                ▼
      MRI CNN Feature Extraction
                │
                ▼
         Multimodal Fusion
                │
                ▼
      Graph Construction
                │
                ▼
          GCN / GAT
                │
                ▼
   Alzheimer's Classification
```

---

## Repository Structure

```text
Alzheimers-Multimodal-GNN/
│
├── data/
├── clinical_ml/
├── mri_cnn/
├── fusion/
├── gcn/
├── results/
├── report/
├── README.md
└── requirements.txt
```

---

## Dataset

* OASIS-1 Cross-Sectional Dataset
* Subject-matched clinical and MRI data
* Alzheimer's, Mild Cognitive Impairment, and Cognitively Normal subjects

---

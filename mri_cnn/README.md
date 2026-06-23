# MRI-Based Deep Learning

## Objective

Extract disease-related representations from structural MRI scans using deep convolutional neural networks.

## Notebooks

* 01_MRI_Exploration.ipynb
* 02_ResNet18_Training.ipynb
* 03_Feature_Extraction.ipynb

## Methodology

* Transfer Learning using ResNet18
* MRI image preprocessing and augmentation
* Feature extraction from the penultimate layer

## Results

| Model            | Macro-F1 |
| ---------------- | -------: |
| ResNet18 MRI CNN |    0.594 |

## Output

* 512-dimensional MRI embeddings for each subject

## Key Inference

MRI-only classification was challenging due to class imbalance and limited sample size. However, the extracted embeddings provided valuable information for multimodal fusion.

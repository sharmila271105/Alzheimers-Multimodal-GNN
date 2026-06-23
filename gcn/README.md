# Graph Convolutional Networks

## Objective

Model inter-subject relationships using Graph Neural Networks on fused multimodal features.

## Notebook

* 01_GCN.ipynb

## Graph Construction

* K-Nearest Neighbors (KNN)
* Cosine Similarity
* k = 5 and k = 10

## Node Features

* Clinical biomarkers
* Cognitive assessments
* MRI embeddings

## Results

| Model      | Accuracy | Macro-F1 |
| ---------- | -------: | -------: |
| GCN (k=5)  |   95.71% |    0.910 |
| GCN (k=10) |   95.71% |    0.910 |

## Key Inference

Graph-based learning achieved the best performance by leveraging relationships between similar subjects, outperforming both clinical-only and multimodal fusion baselines.


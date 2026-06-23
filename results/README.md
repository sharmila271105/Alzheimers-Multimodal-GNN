# Results Summary

## Model Comparison

| Model                        | Macro-F1 |
| ---------------------------- | -------: |
| Clinical Logistic Regression |    0.780 |
| Clinical Random Forest       |    0.820 |
| Clinical XGBoost             |    0.840 |
| MRI CNN                      |    0.594 |
| Fusion Random Forest         |    0.858 |
| Fusion XGBoost               |    0.858 |
| GCN                          |    0.910 |

## Overall Findings

1. Clinical features provided a strong baseline.
2. MRI-only models captured disease-specific imaging patterns but suffered from class imbalance.
3. Multimodal fusion improved classification performance substantially.
4. Graph Convolutional Networks achieved the highest performance by modeling relationships between similar subjects.

## Best Model

GCN (k=5 / k=10)

* Accuracy: 95.71%
* Macro-F1: 0.910

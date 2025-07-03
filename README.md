# Logistic Regression – IIT Kanpur AML

This project demonstrates **Logistic Regression**, a classification algorithm taught in the Applied Machine Learning course by IIT Kanpur.

##  Overview
Logistic Regression predicts whether an input belongs to class `0` or `1` using probability and a threshold (like 0.5).

## Dataset
Feature: `Hours_Studied`  
Target: `Passed` (0 = No, 1 = Yes)

| Hours_Studied | Passed |
|---------------|--------|
| 1             | 0      |
| 5             | 1      |
| 10            | 1      |

## How It Works
- Compute linear equation: `z = wX + b`
- Apply **Sigmoid**: `σ(z) = 1 / (1 + e^-z)`
- Convert probability → class (if > 0.5 → class 1)

## Outputs
- Accuracy
- Confusion Matrix
- Classification Report (Precision, Recall, F1)

## Author
**Krishna Teja Reddy Lingala**  
_IIT Kanpur Certified – AML_

---

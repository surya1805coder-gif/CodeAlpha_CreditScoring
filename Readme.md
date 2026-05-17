# Project: CreditLens — Credit Scoring Model

## Objective
Build a binary classification model to predict creditworthiness using the German Credit Dataset.

## Dataset
- Source: UCI Machine Learning Repository
- Samples: 1,000 | Features: 20 + 2 engineered
- Target: Credit Risk (1=Good, 0=Bad)

## Results
| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|-------|----------|-----------|--------|----|---------|
| Dummy (baseline) | 0.7000 | — | — | — | 0.5000 |
| LogisticRegression | 0.6800 | 0.7754 | 0.7643 | 0.7698 | 0.7548 |
| RandomForest | 0.7150 | 0.7862 | 0.8143 | 0.8000 | 0.7746 |
| XGBoost | 0.7100 | 0.7887 | 0.8000 | 0.7943 | 0.7276 |

*Best Model: RandomForest (ROC-AUC: 0.7746, F1: 0.8000)*
*Optimal Threshold (Youden's J): 0.5900*

## How to Run
1. `pip install -r requirements.txt`
2. Open `Credit_Scoring_Project.ipynb` in Jupyter/Colab
3. Run all cells

## Key Features
- SMOTE applied only after train-test split
- Feature engineering before scaling
- Dummy baseline for comparison

## Author
CodeAlpha ML Intern
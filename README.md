# Fraud Detection (Revolut)

Fraud detection on Revolut-style transaction data. **Work in progress.**

## Contents

- `1_EDA.ipynb` — exploratory data analysis, data distribution, visualisation
- `2_feature_engineering.ipynb` — feature engineering
- `3_undersampling.ipynb` — class balancing + model comparison
- `datasets/` — raw data (transactions, users, countries, currency details)

## Models

- Logistic Regression
- K-Nearest Neighbors
- Decision Tree
- Random Forest
- Gradient Boosting

## other techniques
- dimensionality redaction - PCA, t-SNE, SVD
- sampling - undersampling (working), SMOTE (next step)


## Latest results (undersampling, 5-fold cv) - suspect dataleakage

Logistic Regression: Recall=97%, Precision=96%, F1=97%
K-Nearest Neighbors: Recall=89%, Precision=91%, F1=90%
Decision Tree: Recall=97%, Precision=95%, F1=96%
Random Forest: Recall=98%, Precision=98%, F1=98%
Gradient Boosting:Recall=97%, Precision=97%, F1=97%

Recall as a main metrics for highly unbalanced data 
97% not fraudsters vs. 3% fraudsters

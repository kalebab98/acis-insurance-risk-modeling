# ACIS Insurance Risk Modeling

This project aims to perform end-to-end insurance risk analytics and build predictive models for pricing optimizations at AlphaCare Insurance Solutions (ACIS).

## Objectives

- Perform exploratory data analysis (EDA) to uncover risk patterns.
- Conduct A/B testing to identify statistically significant risk drivers.
- Build predictive models for claim severity and premium pricing.
- Provide actionable business recommendations.

## Tech Stack

- Python (Pandas, Seaborn, Scikit-learn, SHAP)
- Jupyter Notebook
- Git & GitHub
- DVC (Data Version Control)
  

## Key findings
- Premiums are skewed with many high-value policies.

- Higher risk seen in Gauteng and Limpopo provinces.

- Heavy commercial vehicles have higher average losses.

- Logistic regression worked best for predicting claim probability; XGBoost for claim severity.

- Important features include vehicle value estimates, insured sum, vehicle type, and province.

**Limitations**
- Claim data is imbalanced, which affects model performance.

- Model retraining needed over time due to changing patterns.

- Some risk factors like driver behavior are not captured.




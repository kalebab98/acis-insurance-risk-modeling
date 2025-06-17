# 📦 Task 4: Predictive Modeling – Claim Severity & Claim Probability

## 📁 Project Context

This task is part of the ACIS Insurance Risk Modeling Challenge. The goal is to build and evaluate predictive models that enable dynamic, risk-based pricing by forecasting:

- The **severity** of claims (how much a claim will cost)
- The **probability** that a policyholder will file a claim

---

## 🧠 Objectives

- Predict **claim severity** (TotalClaims) for policyholders who submitted a claim.
- Predict **claim probability** (HasClaim) using classification models.
- Evaluate model performance and interpret key drivers using **SHAP**.

---

## 📂 Files in This Task

| File | Description |
|------|-------------|
| `02_claim_severity_modeling.ipynb` | Regression models to predict claim amounts (severity). |
| `03_premium_probability_modeling.ipynb` | Classification models to predict the likelihood of a claim. |

---

## ⚙️ Methodology

### 🔢 Data Preparation

- Handled missing values and filtered records where necessary.
- Converted categorical variables using one-hot encoding.
- Applied feature scaling for regression models.
- Created new variables like `HasClaim`, `Margin`.

---

### 🧮 Claim Severity Modeling (`02_claim_severity_modeling.ipynb`)

- **Target Variable:** `TotalClaims` (for records where claims > 0)
- **Models Used:**
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor
- **Evaluation Metrics:**
  - RMSE (Root Mean Squared Error)
  - R² Score

**Outcome:** XGBoost achieved the best balance between accuracy and interpretability.

---

### 🎯 Claim Probability Modeling (`03_premium_probability_modeling.ipynb`)

- **Target Variable:** `HasClaim` (binary: 1 if claim made, else 0)
- **Models Used:**
  - Logistic Regression
  - Random Forest Classifier
- **Evaluation Metrics:**
  - Accuracy
  - Precision / Recall / F1 Score
  - AUC-ROC (to account for class imbalance)
- **Interpretability:**
  - Used **SHAP** to identify the most influential features impacting claim probability.

---

## 📊 Key Insights

- **Vehicle Make, Registration Year, Cubic Capacity**, and **Province** were influential in claim severity.
- **Claim probability** was better captured by Logistic Regression (higher recall), important for risk-sensitive use cases.
- **Random Forest** had high accuracy but lower sensitivity to actual claims (lower recall).

---

## 📌 How to Use

1. Clone the repository and activate your environment.
2. Ensure necessary libraries (`pandas`, `scikit-learn`, `xgboost`, `shap`, etc.) are installed.
3. Run the notebooks in order.
4. Review model outputs and SHAP values for insights into pricing decisions.

---

## ✅ Next Steps

- Integrate best-performing models into a risk-based pricing pipeline.
- Consider using the model output as input into pricing simulation tools.
- Enhance with more advanced techniques like stacking or hyperparameter tuning.

---




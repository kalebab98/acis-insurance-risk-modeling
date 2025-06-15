# Task 1: Git, GitHub Setup & Exploratory Data Analysis (EDA)

This branch includes two main components of the project:

1. **Git/GitHub version control setup**
2. **Data understanding and exploratory data analysis (EDA)** for a vehicle insurance dataset

---

## ✅ 1.1 Git and GitHub Setup

### Tasks Completed

- Initialized a Git repository for the weekly project
- Created and worked on this dedicated branch: `task-1`
- Followed good version control practices:
  - Committed multiple times with clear messages
  - Structured code and notebooks in a modular way
- Used GitHub for collaboration and backup
- GitHub Actions planned for future CI/CD setup

### KPIs Achieved

- ✔️ Development environment set up and Git integrated
- ✔️ Demonstrated proper version control using branches and commits

---

## 📊 1.2 Exploratory Data Analysis (EDA) and Statistical Thinking

### Dataset Overview

- ~1,000,000 records
- 53 columns including vehicle info, customer demographics, financials, and target metrics
- Created a new feature: `LossRatio = TotalClaims / TotalPremium`

### EDA Tasks Completed

#### ✅ Data Summarization
- Calculated summary statistics for numerical features
- Reviewed column data types and reformatted where necessary (e.g., `TransactionMonth` to datetime)

#### ✅ Data Quality Assessment
- Generated missing value reports
- Identified columns with high missingness (e.g., `CrossBorder`, `CustomValueEstimate`)
- Dropped or flagged irrelevant columns

#### ✅ Univariate Analysis
- Histograms: `TotalPremium`, `TotalClaims`, `LossRatio`
- Bar plots: `Province`, `VehicleType`, `Gender`

#### ✅ Bivariate/Multivariate Analysis
- Mean `LossRatio` by:
  - Province
  - Gender
  - Vehicle Type
- Scatter plots for `TotalPremium` vs `TotalClaims`
- Heatmap for correlation matrix

#### ✅ Outlier Detection
- Box plots to identify skew/outliers in `TotalClaims`, `CustomValueEstimate`

#### ✅ Trends Over Geography and Time
- Grouped by province and visualized average `LossRatio`
- Temporal trend analysis over 18 months using `TransactionMonth`

### Key Insights

- **Gauteng** had the highest loss ratio
- **Heavy commercial vehicles** tend to have high `LossRatio`
- **Male policyholders** had a lower average `LossRatio` than females
- Several car brands like `POLARSUN` had very high average claim amounts

### 📸 Visualizations

- 3 Insightful Plots:
  - Bar chart of Loss Ratio by Vehicle Type
  - Box plot of Claims Amounts by Province
  - Line plot of Total Claims over time

---

## 🧠 KPIs Achieved

- ✔️ Demonstrated strong EDA techniques
- ✔️ Applied statistical reasoning to draw insights
- ✔️ Used suitable visualizations to explain findings
- ✔️ Documented findings clearly

---

## 📁 Project Files

- `eda_notebook.ipynb` – Jupyter Notebook with all analysis
- `eda_summary.md` – Summary of key insights

---

## 🔜 Next Steps

Merge this branch to `main`, then start `task-2` for Data Version Control (DVC).

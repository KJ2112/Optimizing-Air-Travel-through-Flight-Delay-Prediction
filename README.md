✈️ Flight Delay Analysis & Prediction
📌 Project Overview

This project analyzes US airline flight delay data (2015–2023) to understand key causes of delays and build predictive models that forecast whether a flight will be delayed and by how long.

The work combines data cleaning, exploratory analysis, feature engineering, and ML modeling. I introduced a custom Operational Adjustability Index (OAI) to focus on controllable delays (e.g., carrier delays, late aircraft), making the predictions more actionable for airlines.

🎯 Objectives

Exploratory Data Analysis (EDA): Identify seasonal, temporal, and operational delay patterns.

Classification: Predict whether a flight will be delayed (>15 minutes).

Regression: Estimate expected delay duration (minutes).

Model Explainability: Use SHAP values to interpret model decisions.

Actionable Insights: Provide recommendations for airlines to reduce delays.

🛠️ Tech Stack

Languages: Python (Pandas, NumPy, Matplotlib, Seaborn)

ML Frameworks: XGBoost, scikit-learn

Explainability: SHAP

Environment: Jupyter Notebook

📊 Key Results

Classification Model (XGBoost):

Accuracy: ~87%

Recall: ~86% (high ability to catch delayed flights)

ROC-AUC: 0.94

Regression Model (XGBoost):

MAE: ~3.35 minutes

RMSE: ~12.8 minutes

R²: ~0.32 (reasonable given high variance in delays)

OAI-weighted Regression: Improved weighted MAE from 3.35 to 2.65 minutes by emphasizing controllable delays.

SHAP Analysis: Showed month/season and late aircraft intensity as top predictors.

📂 Repository Structure
├── data/
│   ├── Airline_Delay_Cause.csv        # Dataset (raw/processed subset if too large)
│
├── notebooks/
│   ├── flightdelaykj.ipynb            # Main analysis & modeling pipeline
│
├── reports/
│   ├── Flight Delay Analysis.pdf      # Full report with EDA & results
│   ├── Open Project Analytics.pdf     # Project overview & consulting-style insights
│
├── README.md                          # Project documentation (this file)
└── requirements.txt                   # Python dependencies

🚀 How to Run

Clone the repo:

git clone https://github.com/<your-username>/flight-delay-analysis.git
cd flight-delay-analysis


Install dependencies:

pip install -r requirements.txt


Open Jupyter Notebook and run:

jupyter notebook notebooks/flightdelaykj.ipynb

🔑 Learnings

Handling imbalanced datasets using SMOTE and class weights.

Improving generalization with cross-validation & hyperparameter tuning.

Importance of model interpretability (SHAP) in applied ML.

Translating ML outputs into business recommendations.

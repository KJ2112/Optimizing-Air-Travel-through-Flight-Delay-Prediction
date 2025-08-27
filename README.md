# ✈️ Flight Delay Analysis & Prediction  

## 📌 Project Overview  
This project analyzes **US airline flight delay data (2015–2023)** to understand key causes of delays and build predictive models that forecast whether a flight will be delayed and by how long.  

The work combines data cleaning, exploratory analysis, feature engineering, and ML modeling. I introduced a custom **Operational Adjustability Index (OAI)** to focus on controllable delays and make predictions more actionable.  

## 🎯 Objectives  
- **EDA:** Identify seasonal, temporal, and operational delay patterns.  
- **Classification:** Predict whether a flight will be delayed (>15 minutes).  
- **Regression:** Estimate expected delay duration (minutes).  
- **Explainability:** Use SHAP values to interpret model decisions.  
- **Insights:** Provide recommendations for airlines to reduce delays.  

## 🛠️ Tech Stack  
- **Languages:** Python (Pandas, NumPy, Matplotlib, Seaborn)  
- **ML Frameworks:** XGBoost, scikit-learn  
- **Explainability:** SHAP  
- **Environment:** Jupyter Notebook  

## 📊 Key Results  
- **Classification (XGBoost):**  
  - Accuracy: ~87%  
  - Recall: ~86%  
  - ROC-AUC: 0.94  

- **Regression (XGBoost):**  
  - MAE: ~3.35 minutes  
  - RMSE: ~12.8 minutes  
  - R²: ~0.32  

- **OAI-weighted Regression:** Weighted MAE improved from 3.35 → 2.65 minutes.  
- **SHAP Analysis:** Seasonal factors (month/season) and late aircraft intensity were top predictors.  

## 📂 Repository Structure  
```text
├── data/
│ └── Airline_Delay_Cause.csv
│
├── notebooks/
│ └── flightdelaykj.ipynb
│
├── reports/
│ ├── Flight Delay Analysis.pdf
│ └── Open Project Analytics.pdf
│
├── README.md
└── requirements.txt


## 🚀 How to Run  
```bash
git clone https://github.com/<your-username>/flight-delay-analysis.git
cd flight-delay-analysis
pip install -r requirements.txt
jupyter notebook notebooks/flightdelaykj.ipynb

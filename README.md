# amazon-delivery-time-prediction
Delivery time prediction on 43K Amazon orders using Random Forest. 57% RMSE reduction vs mean baseline (RMSE 22.3, R² 0.813). SHAP feature ranking, MLflow tracking. Python · scikit-learn · Random Forest · SHAP
# 📦 Amazon Delivery Time Prediction

> Predicts delivery time in days using Random Forest on 43K orders. Cuts prediction error by 57% vs the mean baseline. SHAP-explained.

---

## 📌 Problem Statement
Late deliveries damage customer trust. Accurate delivery time estimates at order placement allow customers to plan better and reduce support contacts. This project builds an ML model to predict delivery time (in days) from order and logistics features.

## 📊 Key Results

| Metric | Value |
|---|---|
| Dataset size | 43,739 orders × 16 features |
| Best model | Random Forest Regressor |
| RMSE | **22.3 days** |
| R² | **0.813** |
| Error reduction vs baseline | **57%** |
| Explainability | SHAP feature ranking |

## 🛠️ Tech Stack
`Python` · `scikit-learn` · `Random Forest` · `SHAP` · `MLflow` · `Pandas` · `Matplotlib` · `Seaborn`

## 📁 Project Structure
```
Amazon_Delivery_Prediction/
│
├── Amazon_Delivery_Time_Prediction.ipynb   ← Main notebook
├── amazon_delivery.csv                     ← Dataset (place here)
├── requirements.txt
└── README.md
```

## ▶️ How to Run
```bash
pip install -r requirements.txt
jupyter notebook Amazon_Delivery_Time_Prediction.ipynb
```

## 🔍 Key Findings
- Random Forest outperformed Gradient Boosting and Logistic Regression
- SHAP reveals top delay drivers: distance, agent rating, weather conditions
- Baseline (mean prediction) RMSE: 51.6 days → Model RMSE: 22.3 days → **57% improvement**
- Results logged and reproducible via MLflow

---
*Project completed as part of AI/ML Internship at Labmentix Pvt. Ltd. (2025–2026)*

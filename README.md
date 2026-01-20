# Profit-Optimized Credit Risk Engine with Explainable AI (XAI) 🏦

### 📌 Project Overview
Traditional credit scoring models focus only on accuracy (Who will default?). This project takes a step further by focusing on **Profitability** (Who should we approve to maximize revenue?). 

Using **Python (Random Forest)** and **SHAP (SHapley Additive exPlanations)**, I built a risk engine that not only predicts loan defaults but also determines the optimal **Risk Threshold** to balance risk vs. reward.

### 💼 Business Value
* **Reduced Bad Debt:** Identifies high-risk applicants with >85% precision.
* **Profit Optimization:** Simulations determined the optimal cut-off point, potentially increasing net profit by avoiding strict "zero-tolerance" policies.
* **Transparency (XAI):** Uses SHAP values to explain *why* a customer is rejected (e.g., "Loan duration too long relative to income"), ensuring regulatory compliance.

### 🛠️ Tech Stack
* **Language:** Python
* **Machine Learning:** Scikit-Learn (Random Forest Classifier)
* **Explainability:** SHAP (Game Theoretic approach to interpret ML models)
* **Data Analysis:** Pandas, NumPy, Matplotlib

### 📊 Key Insights

**1. The "Why" Behind the Risk (SHAP Analysis)**
![SHAP Analysis](1_Analisa_Faktor_Risiko.png)
* The model reveals that **Loan Duration** and **Credit Amount** are the strongest predictors of default. Longer durations exponentially increase risk.

**2. Finding the "Sweet Spot" for Profit**
![Profit Analysis](2_Analisa_Profit.png)
* A simple binary classification isn't enough. By simulating loan portfolio performance, we found that setting the risk threshold at the calculated optimal point maximizes profit, whereas a stricter threshold would actually *reduce* profit by rejecting too many good customers.

---
*Created by Adin W Pratama*

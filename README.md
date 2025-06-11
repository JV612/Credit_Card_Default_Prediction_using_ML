# Credit Card Default Prediction using Risk-Based Modeling

This project was developed under the guidance of **Finance Club, IIT Roorkee** as part of the Summer ML Project 2025.  
It involves building a risk-aware binary classification model to predict whether a credit card customer is likely to default in the upcoming month based on historical financial behavior.

---

## 📌 Project Objective

The primary goal is to identify high-risk credit card holders by learning from past billing, payment, and demographic data.  
Special emphasis is placed on:
- Financial behavior patterns (e.g., repayment irregularities, credit utilization)
- Class imbalance handling (e.g., SMOTE, weighted loss)
- Threshold optimization based on **F₂-score**, to prioritize defaulter recall

---

## ✅ Steps Followed

1. Data Cleaning and Preprocessing  
2. Exploratory Data Analysis (EDA)  
3. Financial & Behavioral Feature Engineering  
4. Class Imbalance Handling (Weighted Loss, SMOTE)  
5. Model Training and Validation (Logistic, RF, LightGBM, XGBoost)  
6. Threshold Optimization using F₂-score  
7. Final Model Selection and Prediction on Validation Set

---

## 📊 Model Performance (Split Validation Set)

| Model             | Accuracy | Recall | F1 Score | F₂ Score | AUC-ROC |
|------------------|----------|--------|----------|----------|---------|
| Logistic Regression | 0.774  | 0.558  | 0.485    | 0.582    | 0.746   |
| Random Forest       | 0.784  | 0.591  | 0.511    | 0.606    | 0.774   |
| LightGBM            | 0.756  | 0.652  | 0.504    | 0.612    | 0.775   |
| 🏆 **XGBoost (Final)** | **0.755** | **0.649** | **0.503** | **0.6149** | **0.777** |

---

## 📦 Final Prediction Distribution

| Prediction         | Count      |
|--------------------|------------|
| Default (1)        | 2910       |
| No Default (0)     | 2106       |
|                    |Total = 5016|

## 📂 Repository Structure

```bash
.
├── DefaultPrediction.ipynb       # Main notebook with full pipeline
├── validate_dataset_final.csv    # Test dataset (without labels)
├── train_dataset_final1.csv      # Labeled training dataset
├── README.md                     # Project overview and documentation
├── submission_XXXX.csv           # Final prediction output file
└── Report.pdf                    # Formal report submitted to Finance Club

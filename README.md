# 🏦 Bank Customer Churn Prediction

## 📌 Overview
This project applies machine learning classification techniques in **R** to predict bank customer churn based on historical data. By identifying at-risk customers, banks can implement proactive retention strategies to reduce revenue loss and improve customer loyalty.

## 🔍 Problem Statement
Predict whether a customer is likely to **churn (leave the bank)** using demographic and financial behavior data. The primary goal is to **enhance customer retention** through actionable insights.

---

## 🧾 Dataset

- Source: [Kaggle - Bank Customer Churn Dataset](https://www.kaggle.com/datasets/gauravtopre/bank-customer-churn-dataset)
- Size: ~10,000 records
- Key columns:
  - `credit_score`, `country`, `gender`, `age`, `tenure`, `balance`
  - `products_number`, `credit_card`, `active_member`, `estimated_salary`
  - `churn` (Target variable)

---

## 🔬 Methodology

1. **Data Cleaning & EDA**
   - Checked for null values
   - Visualized distributions and churn correlations

2. **Feature Engineering**
   - Categorical encoding
   - Removed `customer_id`

3. **Modeling Techniques Used:**
   - Linear Discriminant Analysis (LDA)
   - Quadratic Discriminant Analysis (QDA)
   - Logistic Regression (Normal & Polynomial Degree 7)
   - Naive Bayes

4. **Evaluation Metrics:**
   - Accuracy
   - Sensitivity
   - Specificity
   - Test Error

---

## 📊 Results Summary

| Model                      | Accuracy | Sensitivity | Specificity |
|---------------------------|----------|-------------|-------------|
| LDA                       | 81.42%   | 23.59%      | 95.55%      |
| QDA                       | **84.54%** | 40.26%      | 95.36%      |
| Logistic (Normal)         | 81.87%   | 21.54%      | **96.62%**  |
| Logistic (Polynomial 7)   | 84.24%   | **34.87%**  | 96.30%      |
| Naive Bayes               | 84.09%   | 30.77%      | 97.12%      |

✅ **QDA** and **Polynomial Logistic Regression** showed the strongest overall performance.

---

## 💡 Insights
- Customers aged 41–50 had the highest churn rates.
- Lower credit scores correlated with higher churn.
- Active membership and product count were significant churn indicators.

---

## 🛠 Tech Stack
- Programming: `R`
- Packages: `MASS`, `stats`, `naivebayes`, `ggplot2`
- Tools: RMarkdown, RStudio

---


# Customer Churn Prediction – Epochs '26 Assignment 6

**Name:** Nandhana S 
**MUID:** nandhanas-4@mulearn

---

## 📌 Business Objective
The goal of this project is to predict customer churn (whether a customer will discontinue service) using behavioral, demographic, and subscription data. Accurately predicting churn allows businesses to implement targeted retention strategies, reduce customer acquisition costs, and maximize customer lifetime value.

---

## 📂 Dataset Overview
* **Source:** Customer Churn Dataset (Kaggle)
* **Total Records:** ~440,000 rows
* **Target Variable:** `churn` (0 = Retained, 1 = Churned)
* **Key Features:**
  * **Demographics:** `age`, `gender`
  * **Usage Metrics:** `tenure`, `usage_frequency`, `support_calls`, `payment_delay`, `last_interaction`
  * **Account Details:** `subscription_type`, `contract_length`, `total_spend`

---

## ⚙️ Preprocessing Pipeline
1. **Handling Missing Values:** Dropped missing rows to clean raw data.
2. **Feature Dropping:** Excluded `customerid` as it holds no predictive value.
3. **Categorical Encoding:** Applied `OneHotEncoder` to categorical columns (`gender`, `subscription_type`, `contract_length`).
4. **Feature Scaling:** Applied `StandardScaler` to normalize numeric features.
5. **Data Splitting:** 80/20 train-test split stratified by target variable `churn`.

---

## 🤖 Models Implemented
1. **Logistic Regression:** Linear baseline model for binary classification.
2. **Decision Tree Classifier:** Non-linear rule-based tree classifier.
3. **Random Forest Classifier:** Ensemble bagger combining multiple decision trees to reduce overfitting.

---

## 📊 Performance Comparison

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Logistic Regression** | ~0.84 | ~0.82 | ~0.83 | ~0.82 |
| **Decision Tree** | ~0.91 | ~0.90 | ~0.89 | ~0.89 |
| **Random Forest** | **~0.96** | **~0.95** | **~0.96** | **~0.95** |


---

## 🏆 Best Model & Justification
**Random Forest Classifier** was selected as the best model because:
* It achieved the highest overall **F1-Score** and **Accuracy**.
* High **Recall** ensures at-risk customers are identified so retention offers can be delivered timely.
* Ensemble learning reduces variance and prevents overfitting compared to a single Decision Tree.

---

## 💡 Key Observations & Business Recommendations
* **Key Risk Factors:** High numbers of `support_calls`, frequent `payment_delay`, and short `contract_length` (Monthly) strongly correlate with higher churn.
* **Proactive Support:** Reach out to customers who place 3+ support calls within a month.
* **Incentivize Long-term Contracts:** Offer discounts on Annual contracts to shift users away from Monthly plans.

---

## 🔮 Future Improvements
* Perform Hyperparameter Tuning using `GridSearchCV`.
* Explore gradient boosting algorithms like **XGBoost** or **LightGBM**.
* Handle potential class imbalance using **SMOTE**.

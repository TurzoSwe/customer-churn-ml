#  Customer Churn Prediction (Machine Learning Project)

##  Overview

This project focuses on predicting customer churn using machine learning techniques. The goal is to identify customers who are likely to leave a telecom service so that businesses can take preventive actions.

---

## 📁 Dataset

* Dataset: Telco Customer Churn Dataset
* Contains customer information such as:

  * Demographics
  * Services subscribed
  * Account information
  * Churn status (Yes/No)

---

##  Data Preprocessing

* Handled data type issues (e.g., `TotalCharges` converted to numeric)
* Checked and confirmed no missing values
* Dropped unnecessary columns (e.g., `customerID`)
* Encoded categorical variables:

  * Binary encoding (Yes/No → 1/0)
  * One-hot encoding for multi-category features

---

##  Feature Engineering

* Converted all features into numeric format
* Prepared dataset for machine learning models

---

##  Models Used

###  Logistic Regression

* Used as a baseline model
* Applied `class_weight="balanced"` to handle class imbalance

###  Random Forest Classifier

* Used for improved performance and comparison
* Captures non-linear relationships

---

## 📊 Model Evaluation

### Metrics Used:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* ROC Curve (AUC)

### Results:

* Logistic Regression Accuracy: ~73–79%
* Improved Recall for churn after class balancing
* ROC-AUC Score: **0.83** (Strong performance)

---

##  Feature Importance

Used permutation importance to identify key features affecting churn:

Top important features:

* InternetService (Fiber optic)
* Tenure
* Monthly/Total Charges
* Paperless Billing
* Contract Type

---

##  Key Insights

* Customers with **short tenure** are more likely to churn
* **Fiber optic internet users** show higher churn rates
* Higher **charges** increase churn probability
* Long-term contracts reduce churn
* Lack of additional services (e.g., tech support) increases churn

---

##  Project Pipeline

1. Data Loading
2. Data Cleaning
3. Encoding
4. Train-Test Split
5. Model Training
6. Model Evaluation
7. Model Improvement
8. Feature Importance Analysis

---

##  Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib / Seaborn

---

##  Conclusion

This project demonstrates how machine learning can be used to predict customer churn and generate actionable business insights. The model performs well and can help companies improve customer retention strategies.

---

##  Future Improvements

* Hyperparameter tuning
* Cross-validation
* Deployment with UI (Streamlit)
* Advanced models (XGBoost)

---

## 👨‍💻 Author

Rakibul Hasan Turzo

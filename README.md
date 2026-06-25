# 📊 Customer Churn Prediction System

A Machine Learning project that predicts whether a telecom customer is likely to churn using **XGBoost Classification**. The project includes complete data preprocessing, exploratory data analysis (EDA), class balancing with **SMOTE**, hyperparameter tuning using **RandomizedSearchCV**, and an interactive **Streamlit** web application.

---

## 🚀 Demo

> *(Add your Streamlit deployment link here once deployed.)*

---

## 📌 Problem Statement

Customer churn is one of the biggest challenges for subscription-based businesses. Identifying customers who are likely to leave enables companies to take proactive retention measures.

This project predicts whether a customer will churn based on demographic information, services used, and account details.

---

## 📂 Dataset

**Dataset:** Telco Customer Churn Dataset

**Source:** IBM Sample Data

The dataset contains **7,043 customer records** with **19 input features**.

### Features include:

* Gender
* Senior Citizen
* Partner
* Dependents
* Phone Service
* Internet Service
* Online Security
* Online Backup
* Device Protection
* Tech Support
* Streaming TV
* Streaming Movies
* Contract
* Paperless Billing
* Payment Method
* Tenure
* Monthly Charges
* Total Charges

Target Variable:

* **0 → No Churn**
* **1 → Churn**

---

# 📊 Exploratory Data Analysis

The following analyses were performed:

* Class imbalance analysis
* Distribution plots
* Contract-wise churn analysis
* Feature importance visualization
* Confusion Matrix
* Classification Report

---

# ⚙️ Data Preprocessing

The preprocessing pipeline includes:

* Removed `customerID`
* Converted `TotalCharges` to numeric
* Binary Encoding
* Label Encoding
* Train-Test Split
* SMOTE Oversampling

---

# 🤖 Machine Learning Model

Model Used:

* **XGBoost Classifier**

Hyperparameter tuning performed using:

* **RandomizedSearchCV**

Optimized Parameters:

```python
{
    'subsample': 0.6,
    'n_estimators': 300,
    'max_depth': 6,
    'learning_rate': 0.01,
    'colsample_bytree': 0.8
}
```

---

# 📈 Model Performance

| Metric            |  Value |
| ----------------- | -----: |
| Training Accuracy | 80.94% |
| Test Accuracy     | 76.72% |
| Precision (Churn) |    55% |
| Recall (Churn)    |    68% |
| F1 Score (Churn)  |    61% |

---

# ⭐ Top Important Features

The most influential features identified by XGBoost are:

1. Contract
2. Online Security
3. Tech Support
4. Dependents
5. Internet Service
6. Online Backup
7. Device Protection
8. Phone Service
9. Tenure
10. Monthly Charges

---

# 💻 Streamlit Web Application

The project includes an interactive Streamlit application where users can:

* Enter customer details
* Predict churn probability
* View prediction confidence
* Analyze customer risk
* Visualize prediction probabilities
* Receive business recommendations

---

# 📁 Project Structure

```
Customer-Churn-Prediction/
│
├── churn_app.py
├── customer_churn.ipynb
├── customer_churn_model.pkl
├── churn_encoders.pkl
├── requirements.txt
├── Telco-Customer-Churn.csv
├── README.md
└── images/
```

---

# 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* SMOTE
* Joblib
* Plotly
* Streamlit

---

# ▶️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Customer-Churn-Prediction.git
```

Navigate to the project

```bash
cd Customer-Churn-Prediction
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the Streamlit application

```bash
streamlit run churn_app.py
```

---

# 📊 Future Improvements

* SHAP Explainability
* Probability Threshold Optimization
* Cross Validation
* Feature Selection
* Docker Deployment
* Cloud Deployment
* Model Monitoring

---

# 👨‍💻 Author

**Pranav Das**

B.Tech Computer Science Student

Interested in Machine Learning, Data Science, and Artificial Intelligence.

---

# ⭐ If you found this project useful

Please consider giving this repository a ⭐ on GitHub.

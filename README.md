# 📊 Customer Churn Prediction System

## 🚀 Overview

Customer Churn Prediction is a Machine Learning project that predicts whether a bank customer is likely to leave the bank or continue using its services.

The project uses customer information such as:

- Credit Score
- Age
- Geography
- Gender
- Balance
- Salary
- Number of Products
- Credit Card Status
- Active Membership

and predicts whether the customer is likely to churn.

---

## 🎯 Objective

Customer retention is one of the biggest challenges for banks and subscription-based businesses.

The objective of this project is to:

- Analyze customer behavior
- Predict customer churn
- Help businesses take preventive actions
- Improve customer retention strategies

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Joblib
- Streamlit
- Matplotlib
- Seaborn

---

## Github Link
https://github.com/nithika1405/customer-churn-prediction



## 📂 Project Structure

```text
Customer-Churn-Prediction/
│
├── data/
│   └── Churn_Modelling.csv
│
├── models/
│   ├── churn_model.pkl
│   ├── scaler.pkl
│   └── columns.pkl
│
├── app.py
├── train_model.py
├── requirements.txt
├── README.md
│
└── screenshots/
```

## 📊 Dataset

Dataset contains information about bank customers.

### Features

- CreditScore
- Geography
- Gender
- Age
- Tenure
- Balance
- NumOfProducts
- HasCrCard
- IsActiveMember
- EstimatedSalary

### Target Variable

```text
Exited

0 → Customer Stays
1 → Customer Leaves
```

---

## ⚙️ Machine Learning Workflow

### 1. Data Preprocessing

- Remove unnecessary columns
- Handle categorical variables
- Perform one-hot encoding

### 2. Feature Scaling

- StandardScaler is used for normalization

### 3. Model Training

Random Forest Classifier:

```python
RandomForestClassifier(
    n_estimators=300,
    max_depth=10,
    random_state=42
)
```

### 4. Model Evaluation

Metrics used:

- Accuracy Score
- ROC-AUC Score
- Classification Report
- Confusion Matrix

### 5. Model Saving

Trained model and preprocessing objects are saved using Joblib.

---

## 🚀 Installation

### Step 1: Clone Repository

```bash
git clone https://github.com/nithika1405/customer-churn-prediction.git
cd customer-churn-prediction
```

### Step 2: Create Virtual Environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### Linux / Mac

```bash
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install Requirements

```bash
pip install -r requirements.txt
```

---

## 🏋️ Train Model

Run:

```bash
python train_model.py
```

This will generate:

```text
models/
├── churn_model.pkl
├── scaler.pkl
└── columns.pkl
```

---

## 🌐 Run Streamlit Application

```bash
streamlit run app.py
```

The application will open automatically in your browser.

---

## 💻 Application Features

### User Inputs

- Credit Score
- Age
- Tenure
- Balance
- Number of Products
- Credit Card Status
- Active Member Status
- Salary
- Country
- Gender

### Output

- Churn Probability
- Customer Likely To Stay
- Customer Likely To Churn

---

## 📈 Model Performance

The model is evaluated using:

- Accuracy Score
- ROC-AUC Score
- Classification Report
- Confusion Matrix

Random Forest provides strong performance for customer churn prediction and handles non-linear relationships effectively.

---

## 🔮 Future Improvements

- Support for all countries
- XGBoost Model
- LightGBM Model
- Hyperparameter Tuning
- Explainable AI (SHAP)
- Cloud Deployment
- Customer Retention Recommendation System

---

## 🎓 Learning Outcomes

This project demonstrates:

- Data Cleaning
- Feature Engineering
- Machine Learning Classification
- Model Evaluation
- Streamlit Deployment
- End-to-End ML Pipeline Development

---

## 👩‍💻 Author

**Nithika**

---

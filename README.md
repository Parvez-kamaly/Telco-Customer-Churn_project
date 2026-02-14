# Telco Customer Churn Prediction

This project predicts customer churn for a telecom company using machine learning classification models. The goal is to identify customers likely to leave the service so that retention strategies can be applied.

---

## 📂 Dataset

Source: Kaggle – Telco Customer Churn Dataset  

**Features:**

- customerID, gender, SeniorCitizen, Partner, Dependents, tenure, PhoneService, MultipleLines
- InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport
- StreamingTV, StreamingMovies, Contract, PaperlessBilling, PaymentMethod
- MonthlyCharges, TotalCharges, Churn (target variable)

---

## 🛠️ Project Workflow

**1️⃣ Data Preprocessing:**

- Encode categorical variables
- Feature scaling
- Train-test split

## 🔍 Exploratory Data Analysis (EDA)

- **Churn distribution:** Bar / Pie chart — Check imbalance (No vs Yes)  
- **Gender vs Churn:** Countplot — Compare males vs females leaving  
- **Senior Citizen vs Churn:** Bar chart — Older customers churn more?  
- **Partner / Dependents vs Churn:** Countplot — Effect of family status  
- **Tenure vs Churn:** Histogram / Boxplot — Short-tenure customers churn more  
- **Internet Service / Tech Support / Online Security vs Churn:** Countplot — Fiber optic, Tech Support reduce churn  
- **Contract type vs Churn:** Bar chart — Month-to-month churn higher  
- **Payment Method / Paperless Billing vs Churn:** Countplot — Electronic check linked to churn  
- **MonthlyCharges / TotalCharges vs Churn:** Boxplot — High-paying customers leaving & anomalies


**3️⃣ Models Implemented:**

- Logistic Regression
- Random Forest Classifier
- Artificial Neural Network (ANN)

**4️⃣ Evaluation Metrics:**

- Accuracy, Precision, Recall, F1-score
- Confusion Matrix
- ROC-AUC curve
- Precision & Recall comparison bar chart

---

## 📊 Results

| Model                | Accuracy | Precision (Churn=1) | Recall (Churn=1) | F1-score (Churn=1) | ROC-AUC |
|---------------------|----------|--------------------|-----------------|-------------------|---------|
| ANN                  | 0.76     | 0.53               | 0.72            | 0.61              | 0.8367  |
| Logistic Regression  | 0.74     | 0.51               | 0.78            | 0.61              | 0.8411  |
| Random Forest        | 0.77     | 0.54               | 0.78            | 0.64              | 0.8445  |

**Note:** Random Forest performed slightly better overall in terms of ROC-AUC and F1-score for the churned customers.

---

## 🚀 Run the Project

Open the notebook in Google Colab or Jupyter Notebook:

```bash
git clone https://github.com/parvezkamaly/Telco-Customer-Churn_Prediction.git
cd Telco-Customer-Churn_Prediction
jupyter notebook Customer_Churn_Prediction.ipynb

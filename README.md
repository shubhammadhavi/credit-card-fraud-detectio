# 🚀 Credit Card Fraud Detection using Machine Learning

## 📌 Overview
Credit card fraud is a serious issue, affecting financial institutions and customers globally. This project builds a **machine learning model** to detect fraudulent transactions, ensuring security and reducing financial losses.

## 📊 Dataset Information
- **Source**: [Kaggle - Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Size**: 284,807 transactions
- **Features**:
  - `Time`: Seconds elapsed since the first transaction.
  - `Amount`: Transaction amount.
  - `V1-V28`: PCA-transformed features.
  - `Class`: **1 = Fraudulent transaction**, **0 = Legitimate transaction**.

---

## 🔍 **Project Workflow**
### 1️⃣ **Exploratory Data Analysis (EDA)**
- Analyzed **fraud vs. legitimate transaction distribution**.
- Examined **feature correlations** and transaction behavior.

### 2️⃣ **Data Preprocessing & Handling Imbalance**
- **SMOTE (Synthetic Minority Oversampling Technique)** was used to handle class imbalance.
- **Feature Scaling**: Normalized the `Amount` feature using **Min-Max Scaling**.

### 3️⃣ **Model Training & Hyperparameter Tuning**
- **Algorithm Used**: 🏆 `Random Forest Classifier`
- **Hyperparameter Tuning**: Performed using `GridSearchCV` to optimize model performance.

### 4️⃣ **Evaluation Metrics**
✅ **Accuracy**  
✅ **Precision & Recall (to measure fraud detection efficiency)**  
✅ **AUC-ROC Curve Analysis**  

---

## 📈 **Results & Findings**
- Fraudulent transactions account for **only 0.17% of the dataset** (highly imbalanced).
- **Feature V14 was the most influential** in detecting fraud.
- **SMOTE improved recall**, ensuring the model detects more fraud cases.
- **Random Forest achieved high precision**, minimizing false fraud alerts.

---

## 🛠 **How to Run This Project**
### **1️⃣ Install Dependencies**
```bash
pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn

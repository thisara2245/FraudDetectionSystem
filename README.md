# 🔍 Fraud Detection System using Machine Learning 💡

This project focuses on detecting **fraudulent financial transactions** using multiple **machine learning algorithms** — Logistic Regression, Random Forest, XGBoost, and LightGBM.  
It aims to identify **unusual or suspicious transactions** in financial datasets while minimizing false alarms, ensuring **accuracy, trust, and security**.

---

## 🧠 Project Overview

Fraud detection is one of the most critical applications of machine learning in the financial industry.  
This system is built to analyze transaction data and automatically detect **potential frauds** in banking systems.

The model was trained and evaluated on a labeled transaction dataset and achieves a balance between **high precision** (few false positives) and **high recall** (catching most frauds).

---

## 🚀 Key Features

- ✅ Detects suspicious bank transactions using ML models  
- 🧩 Handles **class imbalance** effectively using resampling and weighting  
- 🎯 Achieves **high precision and balanced recall**  
- ⚙️ Implements **feature engineering and preprocessing pipelines**  
- 📊 Compares multiple models to choose the best performer  
- 🌐 Includes a **Streamlit web app** for live prediction testing  

---

## ⚙️ Algorithms Used

| Algorithm | Description | Advantage |
|------------|--------------|------------|
| **Logistic Regression** | Baseline binary classifier | Fast and interpretable |
| **Random Forest** | Ensemble of decision trees | Handles complex non-linear patterns |
| **XGBoost** | Gradient boosting algorithm | Excellent accuracy and performance |
| **LightGBM** | Fast gradient boosting framework | Efficient for large-scale data |

---

## 🧩 Data Preprocessing

- Removed null or duplicate entries  
- Encoded categorical features (e.g., transaction type)  
- Created engineered features such as:
  - `balanceDiffOrg = oldbalanceOrg - newbalanceOrig`
  - `balanceDiffDest = newbalanceDest - oldbalanceDest`
  - `zero_after_transfer` flag for zero balances post-transfer  
- Scaled numerical features using **StandardScaler**
- Split dataset into **training (80%)** and **testing (20%)** sets  

---

## 📊 Model Evaluation Metrics

Each model was evaluated using:

- **Precision** – how many predicted frauds were correct  
- **Recall** – how many actual frauds were detected  
- **F1-score** – balance between precision and recall  
- **ROC-AUC** – overall model discrimination ability  


---

## 🧰 Tech Stack

- **Language:** Python 3.8+  
- **Libraries Used:**
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `xgboost`
  - `lightgbm`
  - `matplotlib`
  - `seaborn`
  - `joblib`
  - `streamlit`



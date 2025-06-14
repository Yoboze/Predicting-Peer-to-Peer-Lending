# 📊 Loan Default Prediction Using Statistical & ML Modeling

This project applies a range of **statistical** and **machine learning** models to predict **loan default** outcomes on peer-to-peer lending platforms. We analyze performance on both **imbalanced** and **SMOTE-balanced** datasets to determine the most robust modeling approach.

---

## 📁 Dataset Overview

The dataset includes categorical and continuous borrower attributes, such as:

- Loan term  
- Loan grade  
- Home ownership  
- Income and loan amount  
- Employment length  
- Loan purpose

---

## 🔄 Data Preprocessing

- Dropped one level of each categorical variable (e.g., `term = 36 months`, `grade = B`, `home_ownership = other`)
- Split dataset: **80% training**, **20% testing**
- Modeled under two settings:
  1. Using imbalanced data directly  
  2. Using **SMOTE** to balance the dataset

---

## 🧠 Models Applied

The following statistical and machine learning models were implemented:

- **Logistic Regression**
- **Gaussian Discriminant Analysis (GDA)** – custom implementation
- **Naive Bayes**
- **Fisher Linear Discriminant Analysis (FLDA)**
- **Support Vector Machines (SVM)**
  - Soft Margin: `C = 0.01`, `0.1`, `1`
  - Hard Margin: `C = 1000`, `10000`
  - Kernel SVMs: RBF, Polynomial

> All models were implemented using Python’s `scikit-learn`, except for GDA which was implemented from scratch.

---

## ✅ Evaluation Metrics

Each model was evaluated on the test set using:

- **Precision**
- **Recall**
- **F1-Score**
- **ROC AUC**

Metrics were reported for both **original (imbalanced)** and **SMOTE-balanced** datasets.

---

## 🏆 Key Results

- **Logistic Regression** and **Kernel SVM (RBF)** consistently outperformed other models
- Achieved:
  - **F1-Score up to 0.99**
  - **ROC AUC up to 0.94**
- Robust predictive performance observed on both balanced and imbalanced data

---

## 🧰 Tools & Libraries

- Python
- Scikit-learn
- Imbalanced-learn (SMOTE)
- NumPy / Pandas
- Matplotlib / Seaborn

---

## 👨‍💻 Author

**Ebenezer Oluwasakin, Ph.D.**  
Data Scientist | Computational & Data Science Researcher

---



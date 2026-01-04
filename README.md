
# Zenvy Task – Payroll Risk Scoring System

This repository contains my submission for the **Data Science Intern task**.

The goal of this project is to identify **high-risk payroll records** using a machine learning approach.  
Since no real dataset was provided, I created a **synthetic dataset** to simulate employee payroll behavior.

---

## What is this project about?
The system tries to flag employees who may be **high risk**, for example:
- Taking too many leaves
- Still receiving high salary hikes

This helps simulate how payroll anomalies could be detected in a real company.

---

## Files in this Repository
- **Payroll_Risk_Analysis.ipynb**  
  The main notebook with data generation, feature engineering, model training, and evaluation.

- **README.md**  
  Project explanation and instructions.

---

## What I Did

### 1. Data Generation
- Created a dataset of **1,000 employees**
- Included attendance, leaves, salary, and hike information
- Defined a simple rule to label **High Risk** employees

### 2. Feature Engineering
- Added new features to compare:
  - Employee cost
  - Employee work patterns

### 3. Modeling
Trained and compared three models:
- Logistic Regression
- Random Forest
- XGBoost

### 4. Evaluation
- Compared model accuracy
- Checked which features were most important

---

## Results
- **Random Forest and XGBoost** performed better than Logistic Regression
- Salary hikes and cost-related features were the strongest indicators of risk

---

## How to Run

### Requirements
- Python 3

### Install libraries
```bash
pip install pandas numpy scikit-learn seaborn matplotlib xgboost

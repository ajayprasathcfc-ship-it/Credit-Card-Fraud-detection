# Credit-Card-Fraud-detection
# Credit Card Fraud Detection using Machine Learning

## Project Overview

This project focuses on detecting fraudulent credit card transactions using Machine Learning techniques. Fraud detection is one of the most important applications of machine learning in the banking and financial sector because fraudulent transactions can lead to major financial losses.

The project includes data preprocessing, feature scaling, handling imbalanced datasets using SMOTE, exploratory data analysis (EDA), machine learning model training, and performance evaluation to accurately identify fraudulent transactions.

The objective of this project is to build an efficient fraud detection system that can help financial institutions identify suspicious transactions and reduce fraud-related losses.

---

## Problem Statement

The goal of this project is to predict whether a credit card transaction is fraudulent or legitimate based on transaction-related features.

By accurately identifying fraudulent transactions, financial institutions can:

- Prevent financial fraud
- Reduce monetary losses
- Improve transaction security
- Enhance fraud monitoring systems
- Support real-time fraud detection

---

## Dataset Description

The dataset contains credit card transaction records with anonymized features.

### Dataset Features

| Feature | Description |
|----------------|--------------------------------------------|
| Time | Time elapsed between transactions |
| V1 - V28 | PCA transformed transaction features |
| Amount | Transaction amount |
| Class | Target variable (0 = Non-Fraud, 1 = Fraud) |

### Target Variable

- **0 → Legitimate Transaction**
- **1 → Fraudulent Transaction**

The dataset is highly imbalanced because fraudulent transactions are very rare compared to normal transactions.

---

## Data Preprocessing

Several preprocessing steps were performed to ensure data quality and improve model performance.

### Preprocessing Steps

- Loaded and inspected dataset
- Checked missing values
- Removed duplicate records
- Split dataset into training and testing sets
- Applied feature scaling using StandardScaler
- Handled class imbalance using SMOTE

### Dataset Validation

The dataset integrity was verified using:

```python
df.info()
df.describe()
df.isnull().sum()
```

---

## Exploratory Data Analysis (EDA)

EDA was performed to understand transaction behavior and identify fraud patterns.

### Key Analysis Performed

- Fraud vs non-fraud transaction distribution
- Transaction amount analysis
- Correlation analysis
- Feature distribution analysis
- Outlier detection

### Visualizations Used

- Count plots
- Heatmaps
- Histograms
- Box plots
- Confusion matrix
- Feature importance charts

These visualizations helped identify transaction anomalies and fraud-related patterns.

---

## Handling Imbalanced Dataset using SMOTE

The dataset contained severe class imbalance because fraudulent transactions represented only a very small percentage of total transactions.

To solve this issue, **SMOTE (Synthetic Minority Oversampling Technique)** was applied to the training dataset.

SMOTE generates synthetic samples for the minority class to improve model learning and fraud detection performance.

### Benefits of SMOTE

- Improves recall and F1-score
- Reduces model bias toward majority class
- Enhances fraud detection capability

---

## Machine Learning Models Used

### K-Nearest Neighbors (KNN)

KNN predicts fraudulent transactions based on the nearest neighboring data points using distance calculations.

### Random Forest

Random Forest combines multiple decision trees to improve prediction accuracy and reduce overfitting.

### XGBoost

XGBoost improves fraud prediction performance using gradient boosting techniques.

---

## Model Evaluation

The models were evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC Score
- Confusion Matrix

### Final Model Selection

The **Random Forest model** was selected as the final model because it achieved the best balance between:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC score

compared to KNN and XGBoost models.

### Final Random Forest Performance

| Metric    | Score |
|------------|--------|
| Accuracy   | 99%    |
| Precision  | 94%    |
| Recall     | 91%    |
| F1-score   | 92%    |
| ROC-AUC    | 0.98   |

---

## Tools & Libraries Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn

### Development Environment

- Jupyter Notebook
- VS Code

---

## Project Workflow

```text
1. Data Collection
2. Data Cleaning
3. Data Preprocessing
4. Feature Scaling
5. Handling Class Imbalance using SMOTE
6. Exploratory Data Analysis
7. Model Training
8. Model Evaluation
9. Fraud Detection Analysis
10. Business Insights Generation
```

---

## Key Insights

Based on the analysis, the following insights were identified:

- Fraudulent transactions are extremely rare compared to legitimate transactions
- Class imbalance significantly affects model performance
- Feature scaling improves model efficiency
- SMOTE improves fraud detection capability
- Ensemble models perform better for fraud detection tasks

---

## Business Recommendations

### 1. Real-Time Fraud Monitoring

Implement real-time transaction monitoring systems to detect suspicious activities immediately.

### 2. Improve Fraud Prevention Systems

Use machine learning models to automate fraud detection processes.

### 3. Risk-Based Transaction Analysis

Flag high-risk transactions for additional verification.

### 4. Continuous Model Improvement

Regularly retrain fraud detection models using updated transaction data.

---

## Business Value of the Project

This project helps financial institutions:

- Detect fraudulent transactions efficiently
- Reduce financial losses
- Improve banking security
- Automate fraud detection systems
- Support data-driven fraud prevention strategies

---

## Conclusion

This project demonstrates how machine learning techniques can be applied to detect fraudulent credit card transactions.

By combining:

- Data preprocessing
- Feature scaling
- SMOTE
- Exploratory data analysis
- Machine learning models

the system effectively identifies fraudulent transactions and supports fraud prevention strategies.

---

## Future Improvements

Future enhancements may include:

- Deep Learning models for fraud detection
- Real-time fraud detection systems
- Advanced anomaly detection techniques
- Model deployment using Flask or Streamlit
- Integration with banking transaction systems

---

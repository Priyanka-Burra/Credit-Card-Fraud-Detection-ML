# Credit Card Fraud Detection using Machine Learning

## Overview
This project implements a machine learning–based system to identify fraudulent credit card transactions. The objective is to accurately classify transactions as legitimate or fraudulent using supervised learning techniques while addressing challenges such as class imbalance.

The project follows a structured machine learning workflow including data exploration, model training, evaluation, and model persistence.

---

## Dataset
The dataset consists of anonymized credit card transactions containing numerical features generated using PCA transformation. Due to confidentiality constraints, original feature names are not available.

- Total transactions: 284,807  
- Fraudulent transactions: 492  
- Legitimate transactions: 284,315  

This highlights a significant class imbalance, which is common in real-world fraud detection problems.

---

## Methodology

### 1. Data Preprocessing
- Loaded dataset using Pandas
- Verified data types and missing values
- Performed basic exploratory analysis

### 2. Exploratory Data Analysis
- Analyzed class distribution
- Visualized feature correlations using a heatmap

### 3. Model Development
The following models were implemented and compared:
- Dummy Classifier (baseline)
- Logistic Regression
- Random Forest Classifier

### 4. Model Evaluation
Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

Random Forest achieved the best balance between precision and recall for fraud detection.

---

## Results
The Random Forest model demonstrated strong performance in identifying fraudulent transactions while minimizing false positives. The trained model was saved for future inference.

---

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Joblib

---

## Model Saving
The final trained model is saved using `joblib` and can be reused for predicting new transactions without retraining.

---

## Conclusion
This project demonstrates a practical application of machine learning for fraud detection. It follows standard practices suitable for academic evaluation and entry-level machine learning roles.

Future improvements may include advanced imbalance handling techniques, hyperparameter tuning, and deployment as a web service.

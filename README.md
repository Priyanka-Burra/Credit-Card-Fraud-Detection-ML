# Credit Card Fraud Detection using Machine Learning

## Project Overview
This project focuses on building a supervised machine learning system to detect fraudulent credit card transactions. The solution addresses real-world challenges such as extreme class imbalance and evaluates multiple classification models to identify the most effective approach for fraud detection.

The project follows an end-to-end data science workflow including data exploration, model training, performance evaluation, and model persistence.

---

## Problem Statement
Credit card fraud poses significant financial risks to institutions and customers. The objective of this project is to accurately classify transactions as fraudulent or legitimate while minimizing false negatives, which are critical in fraud detection systems.

---

## Dataset Description
The dataset contains anonymized credit card transactions with numerical features generated using PCA transformation to preserve confidentiality.

- Total transactions: **284,807**
- Fraudulent transactions: **492**
- Legitimate transactions: **284,315**
- Target variable: `Class` (0 = Legitimate, 1 = Fraudulent)

The dataset is highly imbalanced, reflecting real-world fraud detection scenarios.

---

## Methodology

### 1. Data Understanding & Preprocessing
- Loaded and inspected dataset structure and data types
- Verified absence of missing values
- Analyzed class imbalance in the target variable

### 2. Exploratory Data Analysis (EDA)
- Examined class distribution
- Visualized feature correlations using a heatmap to understand relationships between variables

### 3. Model Development
The following models were implemented and compared:
- **Dummy Classifier** (baseline performance)
- **Logistic Regression**
- **Random Forest Classifier**

### 4. Model Evaluation
Models were evaluated using industry-relevant metrics:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Evaluation emphasized recall and precision due to the imbalanced nature of fraud detection.

---

## Results
The Random Forest classifier outperformed other models, achieving a strong balance between precision and recall while effectively identifying fraudulent transactions. This model was selected as the final solution.

---

## Model Deployment Readiness
- The trained model was serialized using `joblib`
- Saved model can be reused for predicting unseen transactions without retraining

---

## Technologies Used
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn  
- **Visualization:** Matplotlib, Seaborn  
- **Model Persistence:** Joblib  

---

## Conclusion
This project demonstrates a practical application of machine learning for financial fraud detection. It follows standard data science practices suitable for academic evaluation, internships, and entry-level data science roles.

Future enhancements may include advanced imbalance handling techniques, hyperparameter optimization, and deployment as a web-based prediction service.

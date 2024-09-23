# Credit Risk Classification Analysis Report


## Overview of the Analysis

The aim of this analysis is to create machine learning models that assess the creditworthiness of borrowers using historical lending data from a peer-to-peer lending service. The objective is to categorize borrowers as either low risk (0) or high risk (1), assisting financial institutions in making informed lending choices.


### Data Overview

The dataset includes financial details such as loan size, interest rates, borrower income, total debt, and additional factors like the number of accounts and derogatory marks. The target variable, loan_status, signifies whether the loan is classified as low risk (0) or high risk (1).


**Target Variable**: loan_status
0: Low risk (75,036 instances)
1: High risk (2,500 instances)

**Features variables:** loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, and total_debt.

### Machine Learning Process 
The process of constructing and assessing classifier models involved the following stages:


1. **Data Preprocessing:** The dataset was divided into features (X) and the target variable (y). We performed train-test splits to prepare the data for modeling.
   
2. **Model Selection:** Several machine learning models were trained and evaluated, including:
   
   **linear Models**
   - Logistic Regression
     
   **Tree-based Models**
   - Decision Tree Classifier
   - Random Forest Classifier
   - Extra Trees Classifier

   **Kernel-based Model**
   - Support Vector Machine (SVC)
     
   **Instance-based Learning**
   - k-Nearest Neighbors (kNN)
   - 
   **Ensemble Models**
   - Ada Boost Classifier
   - Gradient Boosting Classifier
   - XGBoost Classifier
   - Light GBM Classifier
     
4. Evaluation: The models were evaluated based on accuracy, precision, recall, F1 score, and area under the curve (AUC). Confusion matrices were utilized to assess the classification performance.
   
## Results

1. **Logistic Regression**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.98
   - AUC: 0.9939
  
     
2. **Decision Tree Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.85
   - AUC: 0.9493

     
3. **Random Forest Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.85
   - Recall (Class 1): 0.89
   - AUC: 0.9937

     
4. **Support Vector Machine (SVC)**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9936

     
5. **k-Nearest Neighbors (kNN)**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9937

     
6. **Extra Trees Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.85
   - Recall (Class 1): 0.87
   - AUC: 0.9679

     
7. **Ada Boost Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9945


8. **Gradient Boosting Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9943


9. **XGBOOST Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9942

     
10. **Light GBM Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9947

     
     
## Summary

All models attained 99% accuracy. LightGBM slightly outperforms the others, achieving the highest AUC of 0.9947, closely followed by XGBoost at 0.9942. Precision, recall, and F1-scores remain consistent across the models, suggesting effective management of class imbalance. Both LightGBM and XGBoost are strong contenders for credit risk classification, with LightGBM demonstrating marginally superior performance.




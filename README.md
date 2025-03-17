# Credit Card Fraud Detection

## Project Overview
This project aims to develop a machine learning-based classification model to detect fraudulent credit card transactions. The focus is on handling class imbalance, engineering meaningful features, and optimizing model performance to minimize false positives while ensuring high accuracy.

## Dataset
The dataset consists of anonymized transaction data, including:

- Time: The elapsed time since the first transaction  
- Amount: The transaction amount  
- V1 - V28: Principal components obtained from PCA to protect confidentiality  
- Class: The target variable (0 = Legitimate, 1 = Fraudulent)  

## Data Preprocessing
- Normalization: Standardization of Amount and Time for consistency  
- Handling Imbalance: Synthetic Minority Over-sampling Technique (SMOTE) is applied to address the skewed class distribution  
- Data Splitting: The dataset is divided into training (80 percent) and testing (20 percent) sets  

## Feature Engineering
- Transaction Frequency: The number of transactions per user within a given timeframe  
- Spending Patterns: Identification of unusual spending behavior based on transaction amounts  
- Anomaly Detection: Analysis of deviations from normal transaction activity  

## Model Selection
Several classification algorithms are implemented and evaluated:

- Logistic Regression  
- Random Forest  
- XGBoost  

## Evaluation Metrics
To ensure a reliable fraud detection system, multiple performance metrics are used:

- Accuracy: Measures overall correctness  
- Precision: Ensures legitimate transactions are not incorrectly flagged  
- Recall: Ensures fraudulent transactions are detected  
- F1-Score: Balances precision and recall  
- AUC-ROC: Evaluates the model’s ability to distinguish between legitimate and fraudulent transactions  

## Expected Outcome
The project aims to develop a robust fraud detection model that effectively identifies fraudulent transactions while minimizing false alarms. The final model will be selected based on the best balance of accuracy, recall, and precision.

## Repository Structure
- Data Preprocessing and Feature Engineering  
- Model Training and Evaluation  
- Results Analysis and Optimization  
- Documentation and Code Submission  

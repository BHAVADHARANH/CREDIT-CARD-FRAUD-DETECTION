# Credit Card Fraud Detection

## Project Overview
This project aims to develop a classification model to detect fraudulent credit card transactions efficiently. The dataset is highly imbalanced, requiring special handling to ensure accurate fraud detection while minimizing false positives.

## Dataset
The dataset contains anonymized credit card transactions, including transaction time, amount, and transformed numerical features. The target variable indicates whether a transaction is fraudulent or legitimate.

## Data Preprocessing

1. Missing values were checked, and since none were present, no imputation was required.  
2. The dataset had numerical features with different scales. The transaction amount and time were normalized to improve model performance.  
3. Class imbalance was addressed using Synthetic Minority Over-sampling Technique (SMOTE) to balance fraudulent and non-fraudulent transactions.  

## Feature Engineering

1. Transaction frequency was calculated to track how often similar transactions occur.  
2. Spending patterns were analyzed to detect deviations from normal spending behavior.  
3. Time-based anomalies were identified to detect unusual transactions occurring outside of typical hours.  

## Model Selection

1. Logistic Regression was used as a baseline model for comparison.  
2. Random Forest was chosen for its ability to handle imbalanced datasets effectively.  
3. XGBoost was used due to its high performance in classification tasks.  

## Model Evaluation

1. Accuracy was considered but not relied upon due to class imbalance.  
2. Precision was evaluated to ensure fraudulent transactions flagged by the model were truly fraudulent.  
3. Recall was prioritized to maximize the detection of actual fraudulent cases.  
4. F1-score was used to balance precision and recall.  
5. AUC-ROC was analyzed to measure the model’s ability to differentiate between fraud and legitimate transactions.  

## Results

1. Logistic Regression had high recall but very low precision, leading to many false positives.  
2. Random Forest achieved a good balance between precision and recall.  
3. XGBoost provided the best performance with the highest AUC-ROC and F1-score.  

## Conclusion

1. XGBoost was selected as the final model due to its superior fraud detection performance.  
2. Feature engineering contributed significantly to improving model accuracy.  
3. The model effectively detects fraudulent transactions while keeping false positives low.  

## Repository Structure

1. data - Contains the dataset.  
2. notebooks - Includes exploratory data analysis and model training scripts.  
3. src - Source code for preprocessing, training, and evaluation.  
4. README.md - Documentation of the project.  


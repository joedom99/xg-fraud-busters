# xg-fraud-busters - Hacklytics 2025 with DS club @ GT

# Evaluating Machine Learning Models for Fraud Detection in Financial Transactions

## Overview of the Jupyter Notebook

This project is implemented in a **Jupyter Notebook (.ipynb)** and evaluates **Random Forest** and **XGBoost** classifiers to detect fraudulent transactions in a **credit card dataset**. The goal is to determine which model is more effective in identifying fraud while minimizing false positives.

### Key Steps in the Notebook:

1. **Data Preprocessing**  
   - Loaded the credit card transaction dataset.  
   - Handled class imbalance using **SMOTE (Synthetic Minority Over-sampling Technique)** to ensure better fraud detection.  
   - Scaled the numerical features for optimal model performance.  

2. **Feature Selection & Model Training**  
   - Selected important transaction features, such as amount, time, and transaction frequency patterns.  
   - Split the dataset into **training (80%) and testing (20%)** sets.  
   - Trained two models:  
     - **Random Forest** – A powerful ensemble model that reduces variance and overfitting.  
     - **XGBoost** – A gradient boosting algorithm known for high accuracy and efficiency.  

3. **Evaluation Metrics**  
   - Measured model performance using:  
     - **Accuracy** – Overall correctness of the model.  
     - **Precision** – Ability to correctly identify fraud without false alarms.  
     - **Recall** – Ability to catch actual fraud cases.  
     - **F1-score** – Balance between precision and recall.  
     - **ROC-AUC Curve** – Measures the model’s ability to distinguish between fraud and non-fraud cases.  

## Results and Model Comparison

The evaluation of **Random Forest and XGBoost** revealed key insights into fraud detection performance:  

| Model          | Accuracy | Precision | Recall | F1-Score | ROC-AUC |  
|---------------|----------|-----------|--------|----------|---------|  
| Random Forest | 98.6%    | 87.2%     | 92.5%  | 89.8%    | 97.5%   |  
| XGBoost       | 99.1%    | 91.5%     | 95.3%  | 93.4%    | 98.8%   |  

### Key Observations:

- **XGBoost outperformed Random Forest** in every metric, achieving higher precision, recall, and overall accuracy.  
- **False Positives:** Random Forest generated more false positives, which could lead to unnecessary fraud alerts for legitimate customers.  
- **False Negatives:** XGBoost showed a lower false negative rate, making it better at detecting actual fraud cases.  
- **Computational Efficiency:** Random Forest was faster in training but less efficient in handling high-dimensional data compared to XGBoost.  

## Significance of This Work

### 1. Enhancing Fraud Detection Accuracy  
This study demonstrates that **XGBoost is a superior choice** for fraud detection due to its **high recall** and **precision**, reducing both missed fraud cases and false alarms. Businesses can **prevent financial losses** and improve customer trust by implementing such models.  

### 2. Real-World Applications  
- **Banking & Finance:** Prevent fraudulent credit card transactions in real-time.  
- **E-commerce:** Identify suspicious activities before they impact merchants.  
- **Insurance & Loan Fraud Detection:** Flagging high-risk transactions for further review.  

### 3. Reducing Financial and Operational Costs  
By **minimizing false positives**, businesses can **reduce fraud investigation costs** and avoid unnecessary disruptions for customers. **XGBoost’s efficiency allows for real-time fraud detection** without significant computational overhead.  

### 4. Scalability & Future Improvements  
- **Integrating Deep Learning:** Future work could explore hybrid models combining machine learning with deep learning for enhanced fraud detection.  
- **Adaptive Models:** Implement **self-learning fraud detection** that updates itself based on new fraudulent patterns.  
- **Explainability & Transparency:** Enhancing model interpretability using techniques like SHAP values to better understand fraud decision-making.  

## Conclusion

This project successfully demonstrated that **XGBoost outperforms Random Forest in detecting credit card fraud**, achieving higher precision, recall, and accuracy. The findings emphasize the importance of **data preprocessing, feature selection, and model choice** in financial fraud detection. Implementing such machine learning models in real-world financial systems can significantly **reduce fraud risks, improve customer security, and enhance operational efficiency**.  

Future improvements could focus on **real-time fraud detection**, **self-learning AI models**, and **improved model transparency** to make AI-driven fraud detection even more effective.

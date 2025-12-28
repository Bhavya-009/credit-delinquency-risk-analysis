# Credit Delinquency Risk Analysis & Prediction

## 📌 Project Overview
This project analyzes customer credit data to identify key risk factors driving account delinquency and outlines a predictive modeling approach to flag high-risk customers. The work combines exploratory data analysis (EDA), logistic regression–based risk modeling, and business-focused recommendations to support proactive intervention strategies.

This project was completed as part of the **Tata iQ – GenAI Powered Data Analytics Job Simulation** on **Forage**.

---

## 🎯 Objectives
- Understand the structure and quality of Geldium’s customer credit dataset  
- Identify early indicators of delinquency risk through EDA  
- Build and evaluate a baseline predictive model for delinquency risk  
- Translate analytical insights into clear business recommendations  
- Address ethical and fairness considerations in financial risk modeling  

---

## 📊 Dataset Summary
The dataset contains 500 customer records with demographic, financial, and behavioral attributes, including:
- Income, Credit Score, Credit Utilization  
- Debt-to-Income Ratio, Loan Balance  
- Missed Payments, Employment Status  
- Monthly payment behavior indicators  
- Target variable: **Delinquent_Account (binary)**  

Missing values were handled using median imputation and group-wise imputation where appropriate.

---

## 🔍 Key EDA Insights
- Customers with high credit utilization show significantly higher delinquency rates  
- High debt-to-income ratios are strongly associated with delinquent accounts  
- Missed payments are the strongest behavioral predictor of delinquency  
- Lower credit scores consistently correlate with higher delinquency risk  
- Certain employment and income groups exhibit elevated delinquency patterns  

---

## 🧠 Predictive Modeling Approach
- Model: Logistic Regression (with class weighting to address class imbalance)  
- Feature Engineering: One-hot encoding for categorical variables  
- Scaling: StandardScaler applied to numeric features  
- Output: Probability-based delinquency risk score  
- Thresholding: Custom probability threshold to prioritize recall  

---

## 📈 Model Performance (Test Set)
- Accuracy: ~82%  
- Recall (Delinquent class): 1.00  
- F1-Score (Delinquent class): 0.61  

High recall ensures high-risk customers are identified early, supporting proactive intervention.

---

## 💡 Business Recommendations
- Monitor customers with high credit utilization and DTI ratios more frequently  
- Trigger early outreach for customers showing missed payment behavior  
- Use delinquency risk scores to prioritize intervention strategies  
- Support decisions with transparent and explainable model outputs  

---

## ⚖️ Ethical & Responsible AI Considerations
- Audit model performance across income, employment, and location groups  
- Avoid using predictions as the sole basis for customer decisions  
- Explain model outputs in plain, non-technical language  
- Promote fairness, transparency, and accountability  

---

## 🛠️ Tools & Technologies
- Python (Pandas, NumPy, Matplotlib, Scikit-learn)  
- Jupyter Notebook  

---

## ⚠️ Disclaimer
This project is for educational and simulation purposes only and does not represent a production credit decision system.

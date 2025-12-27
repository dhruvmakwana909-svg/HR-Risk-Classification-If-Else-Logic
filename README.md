# HR Risk Classification – Explainable Machine Learning Project

# Project Overview
This project focuses on identifying employee attrition risk using a combination
of rule-based logic and machine learning. The goal is to balance explainability
for HR teams with predictive performance.

# Problem Statement
HR departments need to identify employees at risk of leaving the organization
and understand the reasons behind the risk.

# Approach
The project uses a two-layer approach:

# 1. Rule-Based Risk Classification (Explainability)
- Simple if-else rules based on employee satisfaction and working hours
- Produces Low, Medium, and High risk categories
- Used only for interpretation and HR insights

# 2. Machine Learning Model (Prediction)
- Decision Tree classifier trained on actual attrition (`left`) data
- Rule-generated features are excluded to avoid data leakage
- Model predicts whether an employee will leave the organization

# Key Improvements
- Fixed data leakage caused by training the model on rule-derived features
- Used real target variable (employee attrition) instead of rule outputs
- Applied pruning to control overfitting
- Clearly separated explainability logic from predictive modeling

# Results
- Achieved realistic accuracy without leakage
- Improved trust and interpretability for HR stakeholders
- Demonstrated correct model evaluation practices

# Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Decision Tree Classifier

# Key Learning
Accuracy of 1.0 can indicate data leakage. Proper separation of rules,
features, and targets is essential for reliable machine learning models.

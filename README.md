
# Predicting Employee Retention

A mid-sized technology company wants to improve its understanding of employee retention to foster a loyal and committed workforce. While the organization has traditionally focused on addressing turnover, it recognises the value of proactively identifying employees likely to stay and understanding the factors contributing to their loyalty.
## Overview
This project builds a logistic regression model to predict employee retention and extract actionable insights for HR leaders. It combines exploratory data analysis (EDA), data preprocessing, and model evaluation to identify the factors most associated with employees staying at the company.

In this assignment you’ll be building a logistic regression model to predict the likelihood of employee retention based on the data such as demographic details, job satisfaction scores, performance metrics, and tenure. The aim is to provide the HR department with actionable insights to strengthen retention strategies, create a supportive work environment, and increase the overall stability and satisfaction of the workforce.
## Problem Statement
A mid-sized technology company wants to move beyond reactive turnover management and proactively understand which employees are likely to stay. The goal is to identify key drivers of retention so HR can design programs that improve employee loyalty and workforce stability.


## Business Objective
- Predict the likelihood of employee retention using demographic, job satisfaction, performance, and tenure-related data.
- Translate model insights into retention strategies that improve employee experience and reduce churn risk.

The accuracy of the model on training data is 74.04% and on validation data is 73.74% which indicates that model generalises well to unseen data.
## Project Tasks / Workflow
1. **Data understanding & EDA**: Review distributions, correlations, and class balance.
2. **Data cleaning**: Handle missing values, remove redundant columns, and address outliers.
3. **Feature engineering**: Encode categorical variables, scale numerical features, and select important predictors.
4. **Modeling**: Train logistic regression with feature selection (RFE) and validate using holdout data.
5. **Evaluation**: Assess accuracy, recall, confusion matrix, ROC curve, and optimal cutoff.

The recall on validation data is 71.66% and 72.26% for training data which means model is predicting most of the actual positive cases consistently.
## Dataset & Variables
The dataset contains **24 columns** (23 predictors + 1 target):

Senior employees are most likely to stay so the company shall offer more leadership and growth opportunities.
**Target variable**
- `Attrition` (Stayed vs. Left)

Good work-life balance is a major factor in employee retention so the company should invest in flexible hours and wellness benefits.
**Predictor variables**
- Employee ID
- Age
- Gender
- Years at Company
- Job Role
- Monthly Income
- Work-Life Balance
- Job Satisfaction
- Performance Rating
- Number of Promotions
- Overtime
- Distance from Home
- Education Level
- Marital Status
- Number of Dependents
- Job Level
- Company Size
- Company Tenure (In Months)
- Remote Work
- Leadership Opportunities
- Innovation Opportunities
- Company Reputation
- Employee Recognition

Employees who have been promoted and who have dependents stay longer. Company should offer clear promotion pathways and family friendly policies.
## Methods
- **Exploratory Data Analysis**: Univariate and bivariate analysis of numerical and categorical features.
- **Data Preparation**: Dropped redundant columns, handled missing values, removed outliers, and applied dummy encoding for categorical features.
- **Feature Scaling**: Standardization of numerical variables for consistent model input.
- **Feature Selection**: Recursive Feature Elimination (RFE) to identify the most influential predictors.
- **Model**: Logistic regression (with statsmodels) and evaluation using accuracy, recall, ROC, and confusion matrix.

High performers tend to stay longer. Company can incentivize high performance and offer perks and recognitions.
## Results
- **Training Accuracy**: 74.04%
- **Validation Accuracy**: 73.74%
- **Validation Recall**: 71.66% (Training recall: 72.26%)

Married employees are more loyal. Company can offer spousal insurance and benefits to reward them.
The model generalizes consistently between training and validation sets, indicating a stable baseline for retention prediction.

## Key Conclusions & Insights
- **Senior employees are more likely to stay** → Invest in leadership and growth opportunities.
- **Work-life balance strongly impacts retention** → Offer flexible schedules and wellness benefits.
- **Promotions and dependents correlate with higher retention** → Provide clear career pathways and family-friendly benefits.
- **High performers stay longer** → Use recognition and incentives to retain top talent.
- **Married employees show stronger retention** → Consider spousal benefits or family-focused policies.

## Business Value & Real-World Use
This model can help HR and leadership teams to:
- Identify employees at higher risk of leaving and intervene early.
- Prioritize retention programs based on the most influential factors.
- Optimize investment in benefits, promotions, and employee engagement initiatives.
- Improve workforce stability, reduce hiring costs, and maintain organizational knowledge.

## How to Use
1. Open `Predicting_Employee_Retention_Starter.ipynb` in Jupyter or VS Code.
2. Run the notebook cells in sequence to reproduce EDA, preprocessing, modeling, and evaluation.
3. Adjust the model, add features, or experiment with other algorithms for improvement.

## Next Steps (Optional Enhancements)
- Try advanced models (Random Forest, XGBoost) for improved performance.
- Tune hyperparameters and compare metrics across models.
- Build a dashboard to monitor retention risk in real time.


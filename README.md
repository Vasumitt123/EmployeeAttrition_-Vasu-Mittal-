Employee Attrition Prediction using Machine Learning

Overview

Employee attrition is a major challenge for organizations, leading to increased recruitment costs, loss of experienced talent, and reduced productivity. This project develops a machine learning model to predict whether an employee is likely to leave the company based on demographic, job-related, and workplace factors.

The project includes data exploration, preprocessing, model training, evaluation, feature importance analysis, and business insights that can help Human Resources (HR) teams make data-driven decisions to improve employee retention.

Features
Exploratory Data Analysis (EDA) with visualizations
Data cleaning and preprocessing
Handling categorical variables using One-Hot Encoding
Feature scaling using StandardScaler
Handling class imbalance using class_weight='balanced'
Training and comparison of multiple machine learning models
Model evaluation using multiple performance metrics
ROC Curve comparison of all models
Confusion Matrix visualization
Feature Importance analysis
Actionable business insights and HR recommendations
Dataset

The dataset contains 1,470 employee records with 35 features, including:

Age
Department
Job Role
Monthly Income
Business Travel
Work-Life Balance
Job Satisfaction
Overtime
Years at Company
Environment Satisfaction
Education
Attrition (Target Variable)

Target Variable

Attrition
Yes → Employee Left
No → Employee Stayed
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Jupyter Notebook / Google Colab
Project Workflow
1. Data Exploration
Loaded the dataset
Checked dataset shape and structure
Identified missing values
Examined categorical and numerical features
Calculated employee attrition rate
2. Exploratory Data Analysis (EDA)

Performed analysis to understand employee attrition patterns:

Attrition distribution
Department-wise attrition
Job Role-wise attrition
Monthly Income vs Attrition
Work-Life Balance vs Attrition
Years at Company vs Attrition
Correlation Heatmap
3. Data Preprocessing
Removed irrelevant columns
Converted Attrition to binary (1/0)
Applied One-Hot Encoding to categorical features
Standardized numerical features
Split data into training and testing sets (80:20)
4. Model Building

Three machine learning models were trained:

Logistic Regression
Random Forest Classifier
Gradient Boosting Classifier

Class imbalance was handled us
ing:

class_weight='balanced'
Model Evaluation

Models were evaluated using:

Accuracy
Precision
Recall
F1 Score
ROC-AUC Score
Confusion Matrix
ROC Curve
Performance Summary
Model	Accuracy	Precision	Recall	F1 Score
Logistic Regression	74.83%	34.12%	61.70%	43.94%
Random Forest	83.33%	37.50%	6.38%	10.91%
Gradient Boosting	85.03%	58.82%	21.28%	31.25%
Best Model

Although Gradient Boosting achieved the highest accuracy, Logistic Regression was selected as the best model because it achieved the highest Recall and F1 Score.

For employee attrition prediction, correctly identifying employees who are likely to leave is more valuable than simply achieving high overall accuracy.

Key Business Insights
Overall employee attrition rate is 16.12%.
The Sales department has the highest attrition rate (20.63%).
Sales Representatives experience the highest employee turnover (39.76%).
Employees with the lowest Work-Life Balance rating have an attrition rate of 31.25%.
Employees are most likely to leave during their first two years with the company.
Business Recommendations
Prioritize retention strategies in the Sales department.
Improve onboarding and mentoring programs for new employees.
Enhance work-life balance initiatives.
Monitor employees working excessive overtime.
Use predictive analytics to identify employees at risk of leaving and intervene proactively.
Project Structure
Employee-Attrition-Prediction/
│
├── Employee_Attrition_Prediction.ipynb
├── employee_attrition.csv
├── README.md
├── requirements.txt
└── images/
    ├── attrition_distribution.png
    ├── department_attrition.png
    ├── jobrole_attrition.png
    ├── confusion_matrix.png
    └── roc_curve.png
Installation

Future Improvements
Hyperparameter tuning using GridSearchCV
Cross-validation
SHAP values for model explainability
XGBoost and LightGBM implementation
Interactive HR dashboard using Streamlit or Power BI
Employee attrition risk prediction web application

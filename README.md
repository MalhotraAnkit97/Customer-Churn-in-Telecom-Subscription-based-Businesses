# Customer-Churn-in-Telecom-Subscription-based-Businesses

Customer Churn Analysis in Telecom Subscription-based Businesses
Project Overview
This project aims to analyze customer churn in telecom subscription-based businesses to help improve customer retention and enhance business profitability. By identifying at-risk customers and understanding the factors that drive churn, we propose strategies to reduce churn and retain valuable customers. We also integrate Customer Lifetime Value (CLTV) analysis to better understand customer behaviors and make strategic business decisions.

Table of Contents
Motivation
Research Objectives
Data
Exploratory Data Analysis
Data Modeling
Conclusions and Recommendations
How to Use
Team
Motivation
With the increasing prevalence of subscription-based business models, ensuring a steady revenue stream through effective customer retention is critical. This project focuses on predicting customer churn by analyzing various factors such as customer demographics, service usage, and billing information. Understanding these patterns can lead to better business strategies, improved customer satisfaction, and a reduction in churn rates.

Key Goals:
Predict customer churn to identify at-risk clients.
Develop strategies for reducing churn by targeting switchers.
Improve profitability through better customer relationship management (CRM) and the integration of CLTV analysis.
Refine products and services to meet customer needs and reduce churn.
Research Objectives
The project aims to:

Reduce Churn: Identify the main reasons for customer churn and devise strategies to retain customers.
Enhance Customer Retention and Acquisition: Use customer behavior insights to develop new products and targeted marketing campaigns that attract and retain customers.
Data
The dataset used in this project contains information from a fictional telecommunications company offering phone and internet services. The dataset includes:

7043 customers with 33 variables such as customer demographics, service details, and financial information.
The dataset was obtained from Kaggle's Telco Customer Churn dataset.
Data Variables:
CustomerID, Gender, SeniorCitizen, Partner, Dependents, Tenure, PhoneService, MultipleLines, InternetService, Contract, MonthlyCharges, TotalCharges, Churn, among others.
Data Gaps:
The dataset lacks some variables such as promotions, employment status, income level, and service modification details, which could provide further insight into churn behavior.

Exploratory Data Analysis
Several key insights were identified through exploratory data analysis:

Churn Rate: 26.5% of customers have churned, while 73.5% remain.
Service Type: Customers using fiber-optic internet services are more likely to churn compared to DSL users.
Contract Type: Customers with month-to-month contracts have a significantly higher churn rate compared to those with longer-term contracts.
Demographic Factors: Senior citizens and customers without dependents show higher churn rates.
Charges: Higher monthly and total charges are positively correlated with churn, suggesting that cost is a major factor.
Data Modeling
We tested several models to predict customer churn:

Logistic Regression (After SMOTE)
Random Forest (After SMOTE)
SVM (Linear, Polynomial, and RBF Kernel)
Neural Networks
Best Model:
The SVM with RBF Kernel (After Hyperparameter Tuning) showed the best performance with an accuracy of 0.81 and an F1 score of 0.63.

Other notable models:
Logistic Regression (After SMOTE) with an F1 score of 0.66.
Random Forest with an F1 score of 0.62.
Conclusions and Recommendations
Key Findings:
Churn Factors: High costs of fiber services, unmet service quality expectations, and competitive market offerings were the primary reasons for churn.
Important Variables: Total and Monthly Charges, Internet Service (Fiber Optic), Tenure, and Dependents significantly influence churn.
Best Performing Model: SVM with RBF Kernel (after tuning) provided the most accurate churn predictions.
Recommendations:
Pricing Flexibility: Introduce tiered pricing plans, loyalty discounts, and bundled services to reduce churn.
Enhanced Customer Support: Focus on fiber optic users and long-tenure customers by providing improved technical support and satisfaction guarantees.
Loyalty Programs: Implement loyalty rewards and recognize customer milestones to reduce churn among long-term customers.
Family-Oriented Plans: Develop family-friendly packages and flexible plans to cater to the needs of customers with dependents.
How to Use
Clone this repository:
bash
Copy code
git clone https://github.com/yourusername/repositoryname.git
Install the required dependencies:
bash
Copy code
pip install -r requirements.txt
Run the Jupyter Notebook STAT208 - GROUP7.ipynb to explore the data and models.
Refer to the final report and presentation for a detailed analysis and conclusions.
Team
Team Leader: Hong Khanh Che
Team Members: Ankit Malhotra, David Bezhanyan, Zih Yu Chen

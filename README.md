Interconnect Churn Prediction: 
https://github.com/hamedtaeb/Customer-Churn-Prediction

📌 Project Overview

This project focuses on predicting customer churn for Interconnect, a telecom operator that provides landline, internet, and digital services. The goal is to build a machine learning model that forecasts which customers are likely to leave, enabling the company to take proactive measures such as offering promotions or tailored plans to improve customer retention.

The project was developed as part of a final sprint simulation, where a two-week bootcamp recreated the experience of working in a real company with business objectives, deadlines, and peer reviews.

🎯 Business Problem

Churn, or the rate at which customers leave a service, directly impacts revenue and long-term growth. By predicting churn in advance, Interconnect can:

Identify at-risk customers.

Offer targeted incentives to retain them.

Reduce marketing costs by focusing only on users likely to leave.

Business value: Improving customer loyalty and reducing churn translates into higher customer lifetime value (CLV).

📂 Dataset

The dataset consists of information about Interconnect’s clients, collected from multiple sources and linked by customerID:

contract.csv → Contract details (BeginDate, EndDate, payment type, etc.)

personal.csv → Personal data (gender, age, partner, dependents, etc.)

internet.csv → Internet services (DSL, Fiber optic, OnlineSecurity, OnlineBackup, etc.)

phone.csv → Phone services (multiple lines, plan types, etc.)

Target variable:

EndDate = "No" → Customer is active (not churned).

EndDate = date → Customer churned.

🛠️ Methodology

The project followed three structured stages:

Exploratory Data Analysis (EDA):

Reviewed datatypes, missing values, and distributions.

Analyzed churn rates by contract type, payment methods, and services.

Feature Engineering & Preprocessing:

Converted contract dates into tenure/duration.

Encoded categorical features.

Scaled numerical variables.

Handled class imbalance if present.

Model Development:

Compared multiple models: Logistic Regression, Random Forest, Gradient Boosting.

Tuned hyperparameters for optimal performance.

Evaluated using AUC-ROC (primary metric) and Accuracy (secondary metric).

📊 Results

Best Model: [Fill in model name, e.g., CatBoostClassifier]

AUC-ROC: [Fill in result, e.g., 0.87]

Accuracy: [Fill in result, e.g., 0.80]

👉 Achieved a strong predictive model that met the sprint requirements.

📖 Key Insights

Customers with month-to-month contracts were more likely to churn.

Fiber optic internet users showed higher churn compared to DSL.

Customers with automatic payment methods (e.g., credit card, bank transfer) were less likely to churn than those paying manually.

🚀 Next Steps

Deploy the model as a service for real-time churn prediction.

Build a dashboard for the marketing team to monitor churn risk.

Test additional features (e.g., usage intensity, customer support interactions).

📚 Tech Stack

Languages: Python

Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, LightGBM / XGBoost / CatBoost

Environment: Jupyter Notebook

🏆 Credits

This project was completed as part of the Final Sprint Bootcamp, simulating a real-world machine learning project with business objectives.

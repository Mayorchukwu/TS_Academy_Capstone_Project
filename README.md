# TS Academy Capstone Project | Group 9: Telco Customer Churn Prediction


## Table of Contents<br>
* Project Overview<br>
* Dataset<br>
* Methodology<br>
* Key Notebook Sections<br>
* Model Performance & Comparison<br>
* Key findings <br>
* Model Limitations
* Business Justification & Recommendations<br>
* Author
<br>

## Project Overview<br>
This project focuses on building an end-to-end classification pipeline to predict customer churn for a telecommunications provider. The primary goal is to identify customers at risk of churning using supervised learning techniques. <br> 
* **Chosen Track:** Classification <br> 
* **Problem Statement:** Predict whether a telecom customer will churn (Yes/No).
<br>

## Dataset <br>
**Telco Customer Churn Dataset (IBM)** <br>
The dataset contains 7,043 customer records with 21 features covering demographic information, service subscriptions, and billing details.
<br>
<br>

## Methodology <br>
The project follows a standard machine learning workflow: <br> 
1. **Data Preprocessing:** Type conversion (specifically TotalCharges to float), handling missing values, and feature selection. <br> 
2. **Exploratory Data Analysis (EDA):** Analysis of churn distribution and relationship between features like Contract and MonthlyCharges with the target. <br>
3. **Modeling:** Implementation of a **Baseline Logistic Regression** and an **Advanced Random Forest Classifier**. <br>
4. **Evaluation:** Assessment using Accuracy, Precision, Recall, and F1-score. <br>
5. **Interpretation:** Analyzing feature importance to understand what drives customer decisions.
<br>

## Key Notebook Sections <br> 
1. **Problem Framing & Track Justification** <br>
Identifies the project as a Supervised Learning (Classification) task aimed at binary outcomes. <br>
2. **Data Understanding & Preprocessing** <br>
Handles the conversion of string data to numeric format (Float64) to allow for mathematical modeling. <br>
3. **Exploratory Data Analysis (EDA)** <br>
Visualizes data patterns, showing that month-to-month contracts and high charges are significant churn indicators. <br>
4. **Baseline Model: Logistic Regression** <br>
The initial model used to set a performance benchmark, achieving approximately 80% accuracy. <br>
5. **Advanced Model: Random Forest** <br>
A robust ensemble model used to capture non-linear relationships and provide Feature Importance insights. <br>
<br>

## Model Performance & Comparison <br> 
| Model | Accuracy | Type |
| :--- | :--- | :--- |
| **Logistic Regression** | 0.80 | Baseline |
| **Random Forest** | 0.79 | Advanced |
<br>

## Key Findings:
* Logistic Regression performed best for overall accuracy.  
* Random Forest helped identify the most important features.
<br>

## **Model Limitations**
While the models achieve high accuracy, there are key limitations to consider:

* **Class Imbalance:** The dataset contains significantly more "Non-Churners" (74%) than "Churners" (26%). This can cause the model to be biased toward predicting that a customer will stay.
* **Feature Scope:** The data focuses on billing and contract types but lacks "Sentiment Data" (like customer service call logs or satisfaction surveys) which are strong predictors of churn.
* **Static Snapshot:** This is a "Point-in-Time" analysis. It does not account for seasonal changes or new competitor offers that might happen after the data was collected.
<br>

## Business Justification & Recommendations <br> 
Based on the **Feature Importance** analysis, the following strategic actions are recommended: <br> 
1. **Contract Migration:** Incentivize customers on month-to-month plans to move to one-year or two-year contracts. <br>
2. **Price Sensitivity:** Offer loyalty discounts to high-paying customers who show early signs of churn (high monthly charges). <br>
3. **Proactive Retention:** Use the 80% accuracy model to flag at-risk customers before they terminate their service.
<br>

## Author
* **Name:** Chukwudalu Udojike
* **Role:** Data Scientist
* **Email:** [udojykdalu@gmail.com]
* **GitHub Repository:** https://github.com/Mayorchukwu/TS_Academy_Capstone_Project

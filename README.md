# Customer Churn Prediction

## Project Overview

Customer churn prediction is a machine learning project that focuses on identifying customers who are likely to stop using a company’s service. In any business, retaining existing customers is very important because losing customers can directly affect revenue, growth, and customer trust.

In this project, customer data is analyzed to understand which factors may influence churn. These factors include age, gender, location, subscription length, monthly bill amount, and total usage. By studying these details, the model learns patterns from past customer behavior and predicts whether a customer is likely to churn or continue using the service.

The main aim of this project is to help the company take action before losing valuable customers. For example, if the model identifies a customer as high-risk, the company can offer discounts, better support, personalized plans, or special offers to retain that customer.

This project follows a complete machine learning workflow, including data cleaning, exploratory data analysis, feature preprocessing, model training, model evaluation, and final prediction.

## Problem Statement

The goal of this project is to build a predictive machine learning model that can classify customers into two categories:

* Customers who are likely to churn
* Customers who are not likely to churn

Customer churn is a major problem for businesses because acquiring new customers is often more expensive than retaining existing ones. By predicting churn in advance, businesses can reduce customer loss and improve customer satisfaction.

## Dataset Description

The dataset contains customer-related information. Each row represents one customer, and each column provides details about that customer.

The main features used in the project are:

* **CustomerID:** Unique ID of each customer
* **Name:** Name of the customer
* **Age:** Age of the customer
* **Gender:** Male or Female
* **Location:** City where the customer is located
* **Subscription_Length_Months:** Number of months the customer has been subscribed
* **Monthly_Bill:** Monthly amount paid by the customer
* **Total_Usage_GB:** Total data usage of the customer
* **Churn:** Target column where `1` means the customer churned and `0` means the customer did not churn

## Tech Stack Used

This project uses basic and important machine learning tools:

* **Python** for programming
* **Pandas** for data cleaning and analysis
* **NumPy** for numerical operations
* **Matplotlib and Seaborn** for data visualization
* **Scikit-learn** for machine learning models
* **StandardScaler** for feature scaling
* **Logistic Regression, Decision Tree, and Random Forest** for classification
* **Accuracy, Precision, Recall, F1-score, Confusion Matrix, and ROC-AUC** for model evaluation

## Project Workflow

### 1. Data Collection

The customer churn dataset was loaded into a Jupyter Notebook using Pandas. The dataset contained customer demographic details, subscription information, billing details, usage behavior, and churn status.

### 2. Data Cleaning

The dataset was checked for missing values, duplicate records, incorrect data types, and unnecessary columns. Columns like `CustomerID` and `Name` were not useful for prediction, so they were removed before training the model.

### 3. Exploratory Data Analysis

Exploratory Data Analysis was performed to understand customer behavior and churn patterns. Visualizations were created to analyze how churn is affected by age, gender, location, subscription length, monthly bill, and total usage.

This helped in understanding which features may be important for predicting churn.

### 4. Feature Preprocessing

Categorical columns like `Gender` and `Location` were converted into numerical format because machine learning models cannot directly understand text values.

Numerical columns were scaled using StandardScaler so that all features were on a similar scale. This improves model performance, especially for algorithms like Logistic Regression.

### 5. Model Training

Multiple classification models were trained on the dataset, including:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier

The dataset was divided into training and testing sets. The training data was used to teach the model, while the testing data was used to check how well the model performs on unseen data.

### 6. Model Evaluation

The models were evaluated using different performance metrics:

* **Accuracy:** Measures overall correct predictions
* **Precision:** Measures how many predicted churn customers were actually churn customers
* **Recall:** Measures how many actual churn customers were correctly identified
* **F1-score:** Balances precision and recall
* **Confusion Matrix:** Shows correct and incorrect predictions
* **ROC-AUC:** Measures how well the model separates churn and non-churn customers

Among the trained models, the best-performing model was selected for final prediction.

## Outcome

The final machine learning model can predict whether a customer is likely to churn or not based on customer details such as age, location, subscription length, monthly bill, and total usage.

This prediction can help businesses identify high-risk customers early and take proper action to retain them. The project shows how machine learning can be used in real-world business problems to reduce customer loss and improve customer retention strategies.

## Business Impact

This project can help a company:

* Identify customers who are likely to leave
* Reduce customer churn rate
* Improve customer satisfaction
* Create targeted retention campaigns
* Save revenue by retaining existing customers
* Make data-driven business decisions

Overall, this project demonstrates the use of machine learning for solving a practical business problem.

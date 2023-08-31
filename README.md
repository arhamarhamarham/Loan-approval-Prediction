# Loan approval prediction using logistic regression

This repository contains a machine learning project that focuses on solving a binary classification problem - predicting loan approvals. The project utilizes a Logistic Regression model to make these predictions. This README file provides an overview of the project, its structure, and key steps in the analysis.

**Project Overview**

Loan approval is a critical decision-making process in the financial sector. This project aims to build a predictive model that can automate this process, making it faster and more efficient while maintaining accuracy. The dataset used in this project contains various features related to loan applications and their approval status.

**Project Structure**

The project is organized into several key stages:

==Data Preparation==

Imported necessary libraries.
Loaded the dataset.
Conducted exploratory data analysis (EDA) to gain insights into the data.
Detected and handled missing values by removing rows with missing data.
Detected and removed outliers by visualizing them through boxplots.
Feature Engineering

Encoded categorical columns:
Label encoded the 'loan_grade' column.
One-hot encoded the 'loan_intent', 'cb_person_default_on_file', and 'person_home_ownership' columns.
Dealing with Class Imbalance

Addressed the severe class imbalance in the target variable 'loan_status'.
Applied stratified train-test splitting to ensure a representative distribution of classes in the training and testing sets.
Conducted undersampling to balance the classes in the training data.
Feature Selection

Performed univariate feature selection using two methods: ANOVA and RandomForestClassifier.
Both methods yielded similar results, indicating the importance of selected features for modeling.
Model Training and Evaluation

Utilized Logistic Regression for classification.
Evaluated the model's performance using a classification report, which provides metrics such as precision, recall, and F1-score.
Classification Report
The classification report for the Logistic Regression model is as follows:


              precision    recall  f1-score   support

           0       0.93      0.79      0.86      4961
           1       0.52      0.79      0.63      1429

    accuracy                           0.79      6390
   macro avg       0.73      0.79      0.74      6390
weighted avg       0.84      0.79      0.80      6390

This classification report provides insights into the model's performance, showing its precision, recall, and F1-score for each class (0 and 1). These metrics help assess the model's ability to distinguish between approved (class 0) and denied (class 1) loan applications.

***Getting Started***

If you'd like to replicate or further explore this project, follow these steps:

Clone this repository to your local machine.
Ensure you have the required libraries and dependencies installed (listed in the project's Python environment file).
Run the Jupyter notebooks or Python scripts provided in the repository to reproduce the analysis and model training.
Feel free to reach out if you have any questions or need assistance with the project. Happy coding!

# Customer Churn Prediction

This project aims to predict customer churn using machine learning classifiers. The dataset used contains information about various factors influencing whether a customer will leave the service.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Dataset](#dataset)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Preprocessing](#data-preprocessing)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)
- [Conclusion](#conclusion)
- [Acknowledgments](#acknowledgments)

## Introduction

Customer churn is a critical metric for businesses as it reflects the percentage of customers that stop using a company's products or services over a given period. Predicting customer churn allows businesses to take preventive measures and improve customer retention.

## Installation

To run this project, clone the repository and install the required libraries using the following commands:

```bash
git clone https://github.com/iamprabhanjan/Customer-Churn-Prediction.git
cd customer-churn-prediction
pip install -r requirements.txt
Dataset
The dataset used in this project is called Churn_Modelling.csv, which contains the following columns:

CreditScore
Age
Tenure
Balance
NumOfProducts
HasCrCard
IsActiveMember
EstimatedSalary
Gender
Geography
Exited (target variable)
Exploratory Data Analysis (EDA)
EDA is performed to understand the distribution of data, relationships between features, and the impact of categorical variables like Gender and Geography on customer churn. The following visualizations are included:

Count plots of Geography and Gender with respect to Exited.
Bar plot of Exited to visualize the class distribution.
Data Preprocessing
Several preprocessing steps were performed:

Dropping unnecessary columns (CustomerId, Surname, RowNumber).
Encoding categorical variables (Gender, Geography) using one-hot encoding.
Scaling numerical features using StandardScaler.
Splitting the data into training and testing sets.
Model Training and Evaluation
Three classifiers were used to predict customer churn:

Logistic Regression
Random Forest Classifier
Gradient Boosting Classifier
The models were trained using the training dataset, and their performance was evaluated on the test dataset. The following metrics were used:

Accuracy
Precision
Confusion Matrix
The results of the models were as follows:

Classifier	Accuracy	Precision
Random Forest	86.5%	78.68%
Gradient Boosting	84.9%	76.33%
Logistic Regression	83.2%	75.10%
Confusion matrices for each classifier were also plotted for a detailed view of the predictions.

Results
The Random Forest Classifier outperformed the other models, achieving the highest accuracy and precision. This demonstrates the effectiveness of ensemble methods in predicting customer churn.
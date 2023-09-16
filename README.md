# IBM HR Analytics Employee Attrition & Performance Analysis

## Overview

This Jupyter Notebook project focuses on the analysis of employee attrition and performance using the [IBM HR Analytics dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset). The dataset contains 1470 records and 35 columns, with no missing values. It encompasses 26 numerical and 9 categorical columns. Some columns, such as 'EmployeeCount', 'EmployeeNumber', 'Over18', and 'StandardHours,' have been excluded from the analysis due to their lack of relevance.

## Data Exploration

The analysis includes visualizations to gain insights into attrition and its relationship with various factors:

- **Attrition by Age:** A count plot illustrating attrition by age.
- **Attrition by Business Travel:** A count plot showing attrition by business travel frequency.
- **Attrition by Department:** A count plot depicting attrition by department.
- **Attrition by DistanceFromHome:** A count plot demonstrating attrition by distance from home.
- **Attrition for Other Columns:** Count plots for other pertinent columns.

## Data Preprocessing

To prepare the data for analysis, the `wrangle` function has been employed. This function handles tasks such as encoding categorical variables and mapping binary categories. Additionally, feature selection and engineering have been carried out.

## Modeling

Four different models have been implemented and evaluated to predict employee attrition:

1. **Logistic Regression (LR):** A logistic regression model.
2. **Random Forest (RF):** A random forest classifier.
3. **Decision Tree (DT):** A decision tree classifier.
4. **K-Nearest Neighbors (KNN):** A k-nearest neighbors classifier.

Each model's performance has been cross-validated, and accuracy scores are reported.

## Model Tuning

To optimize the models, hyperparameter tuning has been performed on the Random Forest (RF) and Logistic Regression (LR) models using GridSearchCV.

## Feature Importance

A bar plot visualizes the top 10 features that are most important in predicting attrition.

## Usage

To run this Jupyter Notebook project:

1. Install the necessary Python libraries (Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn) if not already installed.
2. Download the [IBM HR Analytics dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset) and place it in the same directory as this notebook.
3. Execute the code cells in this notebook in sequential order.

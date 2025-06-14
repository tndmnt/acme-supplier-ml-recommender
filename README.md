# Acme Supplier ML Recommender

This project develops a machine learning-based recommendation system for Acme Corporation to select the most cost-effective supplier for daily operational tasks.

## Project Overview

Acme must complete daily tasks (e.g., deliveries, projects, recruitment) by assigning one of 64 suppliers. The aim is to predict the best supplier for a given task by minimizing the cost difference between the predicted supplier and the optimal one. The project involves:

- **Data Cleaning & Feature Engineering**: Merging task, supplier, and cost datasets; handling missing values and scaling features.
- **Exploratory Data Analysis (EDA)**: Visualizing task/supplier features and performance patterns.
- **Model Training & Evaluation**: Fitting regression models (Linear, Lasso), Random Forest, and Neural Network, using group-based cross-validation (Leave-One-Group-Out), and evaluating via RMSE.
- **Hyperparameter Tuning**: Implementing Grid Search to find optimal model configurations.
- **Model Comparison**: Comparing different regression algorithms based on prediction error and robustness.

## Files

- `cost.csv`, `suppliers.csv`, `tasks.csv`: Raw input datasets.
- `Step1_Step2.ipynb`: Data preparation and cleaning.
- `Step3_Step4_Step5.ipynb`: Model fitting, scoring, and cross-validation.
- `Step6_Linear.ipynb`, `Step6_Lasso.ipynb`, `Step6_DecisionTree.ipynb`: Regression model experiments and evaluation.

## Evaluation Metric

The model performance is evaluated using Root Mean Squared Error (RMSE), based on the cost difference between selected vs. optimal suppliers.


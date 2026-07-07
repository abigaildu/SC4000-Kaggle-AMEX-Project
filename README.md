# SC4000-Kaggle-AMEX-Project
Machine learning pipeline for predicting customer loan default risk using LightGBM, XGBoost, CatBoost, and ensemble learning on the American Express Kaggle dataset.

# American Express Loan Default Prediction (SC4000 Machine Learning Project)

## Overview

This repository contains the group project for **SC4000 Machine Learning** at NTU.

The objective of this project is to predict whether a customer will default on a loan using the American Express (AMEX) Default Prediction dataset. The project covers the complete machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, model development, hyperparameter tuning, ensemble learning, and model evaluation.

---

## Project Objectives

* Predict customer loan default risk using historical financial data.
* Compare the performance of multiple gradient boosting algorithms.
* Improve predictive performance through hyperparameter optimisation and ensemble learning.
* Evaluate models using the AMEX competition metric.

---

## Dataset

The project uses the **American Express Default Prediction** dataset provided for the Kaggle competition. This is the link to the dataset: https://www.kaggle.com/competitions/amex-default-prediction/

Dataset Statistics:
5.5+ million transaction records
458,913 unique customers after aggregation
190 financial and behavioural features
Binary classification task (Default / No Default)

To prepare the data for model training, customer-level features were aggregated from multiple monthly observations into a single record for each customer.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* LightGBM
* XGBoost
* CatBoost
* Optuna
* Matplotlib
* Jupyter Notebook

---

## Machine Learning Pipeline

The project includes the following stages:

* Data cleaning and preprocessing
* Exploratory Data Analysis (EDA)
* Feature engineering
* Missing value handling
* One-hot encoding of selected categorical features
* Model training
* Hyperparameter tuning using Optuna
* Ensemble learning
* Performance evaluation using the AMEX competition metric

---

## Models Evaluated

* LightGBM
* XGBoost
* CatBoost
* Ensemble model (LightGBM + XGBoost + CatBoost)

The ensemble model achieved the best overall performance among the evaluated models.

---

## Repository Contents

* `sc4000_main.ipynb` – Complete machine learning workflow
* `SC4000 Project Report - Group 17.pdf` – Project report

---

## Results

The final solution combines multiple gradient boosting models into an ensemble, resulting in improved predictive performance compared to the individual baseline models.

| Model        | Baseline AMEX |   Tuned AMEX |
| ------------ | ------------: | -----------: |
| LightGBM     |      0.794310 |     0.795962 |
| XGBoost      |      0.792682 |     0.795224 |
| CatBoost     |      0.792617 |     0.794574 |
| **Ensemble** |             — | **0.796716** |

This project demonstrates practical experience in:

* Large-scale data preprocessing
* Feature engineering
* Gradient boosting algorithms
* Model optimisation
* Ensemble learning
* Machine learning experimentation and evaluation

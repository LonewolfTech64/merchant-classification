Merchant Classification — Machine Learning Project

Overview

This project builds a supervised machine learning model to classify merchants based on transaction‑level behavioural data.
It was completed as part of a technical assessment and demonstrates end‑to‑end capability across:

Data exploration

Feature engineering

Model development

Evaluation and validation

Communication of insights

Reproducible workflow and documentation

The final deliverables include a Jupyter notebook, a written report, a presentation, and model predictions.

Repository Structure

merchant-classification/
│
├── notebook/
│   ├── FableData_Analysis.ipynb
│   └── FableData_Analysis.html
│
├── data/
│   ├── train_set.zip
│   ├── test_set.csv
│   └── submission_predictions.csv
│
├── report/
│   └── Final_Report.pdf
│
├── presentation/
│   └── Fable_data_overview.pdf
│
├── context/
│   └── Interview Assignment.pdf
│
├── requirements.txt
└── README.md

Problem Description

The goal is to predict the merchant category for each entity in the dataset using historical transaction data.
This is a multi‑class classification problem with a mix of:

Categorical variables

Numerical behavioural features

Time‑based patterns

Aggregated transaction metrics

The challenge lies in extracting meaningful signals from sparse, noisy, and sometimes highly skewed behavioural data.

Modelling Approach
1. Data Exploration
Identified distributional differences between merchant categories

Explored transaction frequency, spend patterns, and temporal behaviour

Assessed missingness and feature stability

2. Feature Engineering
Key engineered features included:

Aggregated spend metrics (mean, median, std)

Transaction frequency and recency

Category‑level ratios

Normalised behavioural indicators

Log‑transformed skewed variables

3. Model Development
Several models were tested, including:

Logistic Regression

Random Forest

Gradient Boosting (XGBoost / LightGBM)

The final model was selected based on cross‑validated performance and generalisation to the test set.

4. Evaluation
Performance was assessed using:

Accuracy

F1‑score

Confusion matrix

Cross‑validation stability

The final model produced strong, stable performance across classes and generalised well to unseen data.

5. Results
The model achieved strong predictive accuracy on the validation set

Behavioural features contributed most to predictive power

The model successfully captured differences between merchant types

Predictions for the test set are included in submission_predictions.csv

How to Use This Repository

Run the Notebook
Install dependencies:

pip install -r requirements.txt

jupyter notebook notebook/FableData_Analysis.ipynb

Data
train_set.zip contains the training dataset (compressed due to GitHub size limits)

test_set.csv is the unseen evaluation dataset

submission_predictions.csv contains the final model outputs

Deliverables
Notebook — full analysis and modelling workflow

Report — written summary of approach and findings

Presentation — high‑level overview for stakeholders

Predictions — final model outputs

Author: Jonathan Addison  

UK

Machine Learning & Data Science

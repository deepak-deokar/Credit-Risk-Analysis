# Credit-Risk-Analysis

This project focuses on predicting credit risk based on applicant data using an ensemble of machine learning models. The ensemble model includes a Neural Network, Random Forest, and XGBoost, with Logistic Regression as the meta-learner to improve prediction accuracy.

## Project Overview

The goal of this project is to classify loan applications as low or high risk, helping financial institutions make better lending decisions. The dataset contains features such as age, income, loan amount, and employment length.

## Features

- **Data Preprocessing**: Handling missing values, encoding categorical features, and scaling numerical data.
- **Exploratory Data Analysis (EDA)**: Understanding data distributions and correlations between features.
- **Model Building**: Implementing an ensemble model with Random Forest, XGBoost, and a Neural Network.
- **Evaluation Metrics**: Accuracy, confusion matrix, and ROC-AUC to assess model performance.

## Dataset

The dataset used for this project includes features such as:
- `person_age`: Age of the individual
- `person_income`: Annual income
- `person_home_ownership`: Type of home ownership (e.g., RENT, OWN, MORTGAGE)
- `loan_intent`: Purpose of the loan (e.g., PERSONAL, EDUCATION)
- `loan_status`: Loan repayment status (target variable)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-risk-analysis.git
   cd credit-risk-analysis


## Usage

Run the main script to preprocess the data, train the models, and evaluate performance:
python credit_risk.py


## Results

The ensemble model achieved an accuracy of 93% and an AUC score of 84%, outperforming individual models in capturing high-risk and low-risk applicants effectively.

## Future Improvements

Experimenting with different ensemble techniques, such as stacking with other meta-learners.
Using more advanced neural network architectures.
Implementing additional features, like feature selection or dimensionality reduction.

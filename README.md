# Credit Risk Analysis and Prediction

This project focuses on building and evaluating a machine learning model to predict credit risk associated with loan applications. The primary goal is to assist financial institutions in making informed lending decisions by classifying loan applicants as either high or low risk.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Project Overview

Credit risk analysis is a critical process for financial institutions to minimize losses from loan defaults. This project tackles this challenge by leveraging machine learning techniques to build a predictive model. The model analyzes various applicant attributes to assess the likelihood of a loan default. The project includes data preprocessing, exploratory data analysis (EDA), model training, and evaluation.

## Dataset

The dataset used in this project is `credit_risk_dataset.csv`. It contains various features about loan applicants, including:

- `person_age`: Age of the applicant.
- `person_income`: Annual income of the applicant.
- `person_home_ownership`: Type of home ownership (e.g., RENT, OWN, MORTGAGE).
- `person_emp_length`: Employment length in years.
- `loan_intent`: The purpose of the loan (e.g., PERSONAL, EDUCATION, MEDICAL).
- `loan_grade`: The grade of the loan.
- `loan_amnt`: The loan amount.
- `loan_int_rate`: The interest rate of the loan.
- `loan_status`: The loan status (0 for non-default, 1 for default - the target variable).
- `loan_percent_income`: The percentage of income represented by the loan amount.
- `cb_person_default_on_file`: Whether the person has a default on file.
- `cb_person_cred_hist_length`: The credit history length.

## Installation

To run this project, you need to have Python and the following libraries installed:

```bash
pip install pandas numpy tensorflow scikit-learn matplotlib seaborn xgboost
```

## Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/credit-risk-analysis.git
   cd credit-risk-analysis
   ```

2. **Run the Jupyter Notebook:**
   The main code is in the `Credit_Risk.ipynb` notebook. You can run it cell by cell to see the data preprocessing, exploratory data analysis, model training, and evaluation steps.

3. **Run the Python script:**
   Alternatively, you can run the `credit_risk.py` script:
   ```bash
   python credit_risk.py
   ```

## Model Architecture

This project implements and evaluates several machine learning models:

- **Neural Network:** A sequential model built with TensorFlow/Keras.
- **Random Forest:** An ensemble learning method that constructs a multitude of decision trees.
- **XGBoost:** A gradient boosting framework that is highly effective for a wide range of problems.
- **Ensemble Model:** A stacking ensemble model that combines the predictions of the Neural Network, Random Forest, and XGBoost models, using Logistic Regression as the meta-learner to improve overall prediction accuracy.

The final trained model is saved as `credit_risk_model.h5`.

## Results

The models' performance is evaluated based on accuracy, precision, recall, F1-score, and the ROC-AUC score. The ensemble model demonstrated the best performance, outperforming the individual models.

- **Ensemble Model Accuracy:** 93%
- **Ensemble Model ROC-AUC Score:** 0.86

For a detailed comparison of the models' performance, please refer to the classification reports and visualizations in the Jupyter Notebook.

## Future Improvements

- **Hyperparameter Tuning:** Further optimization of the models can be achieved through more extensive hyperparameter tuning using techniques like GridSearchCV or RandomizedSearchCV.
- **Feature Engineering:** Exploring and creating new features could potentially improve the model's predictive power.
- **Advanced Ensemble Techniques:** Experimenting with other ensemble methods like blending or different meta-learners.
- **Deployment:** The trained model can be deployed as a web service or API for real-time credit risk assessment.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgments

- The dataset used in this project is from a publicly available source.
- This project was inspired by the need for more accurate and automated credit risk assessment in the financial industry.

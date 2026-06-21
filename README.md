# Customer Churn Prediction and Retention Strategy

End-to-end machine learning project focused on predicting customer churn and translating model results into actionable retention strategies.

The project uses an e-commerce customer dataset containing demographic, behavioral, satisfaction, complaint, and transaction-related features. The analysis combines data quality assessment, exploratory data analysis, supervised machine learning, lift analysis, and business-oriented marketing recommendations.

## Objective

The goal of this project is to identify customers at risk of churn and support targeted retention actions.

The analysis compares interpretable and non-linear machine learning models, evaluates them using business-relevant metrics, and identifies the main behavioral drivers behind customer churn.

## Workflow

* **Data Audit and Cleaning**
  Assessed missing values, duplicates, inconsistent categories, data types, and outliers. Missing numerical values were imputed using the median, categorical inconsistencies were standardized, and selected outliers were capped or retained depending on their business meaning.

* **Exploratory Data Analysis**
  Analyzed churn distribution, satisfaction score, complaints, tenure, days since last order, cashback amount, and correlations with churn.

* **Feature Engineering and Preprocessing**
  Encoded categorical variables, selected relevant predictors, applied train-test split with stratification, and standardized features for modeling consistency.

* **Predictive Modeling**
  Trained and compared Logistic Regression and Random Forest models to predict customer churn.

* **Model Evaluation**
  Evaluated model performance using accuracy, precision, recall, F1-score, confusion matrices, and lift analysis. Recall was prioritized because missing a real churner is more costly than contacting a customer who would have stayed.

* **Business Recommendations**
  Translated model insights into retention actions focused on onboarding, complaint management, cashback incentives, and targeted customer communication.

## Key Insight

Random Forest provided the strongest performance for churn detection, especially when recall and lift were considered. The most important churn drivers were short customer tenure, complaints, and lower cashback amounts.

This suggests that retention efforts should focus on early customer lifecycle interventions, fast complaint resolution, and value-based incentives for customers with high churn risk.

## Tech Stack

Python · pandas · NumPy · scikit-learn · matplotlib · seaborn · openpyxl

## Repository Structure

```text
customer-churn-prediction-and-retention-strategy/
│
├── customer_churn_prediction_retention_strategy.ipynb
├── requirements.txt
├── README.md
└── data/
    └── data.xlsx
```

## How to Run

Open the notebook in Google Colab or Jupyter Notebook.

The dataset is stored in the `data/` folder and can be loaded directly from this repository.

```bash
pip install -r requirements.txt
```

## Author

Oliwia Iwańska


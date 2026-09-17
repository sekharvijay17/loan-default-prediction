## Loan Default Prediction (VaultSense)

**Repository:** `loan-default-prediction`

## What this project does

This project predicts whether a customer will **default on their loan** or not.

In simple words: given information about a person (income, credit score, loan amount, job history, etc.), the model tries to answer one question —

> **Will this person default on their loan? Yes or No?**

## What I am predicting

The target column is `target_default_risk`:
- `0` = Customer will **NOT** default (safe)
- `1` = Customer **WILL** default (risky)

## About the dataset

- 10,000 customers
- 20 features + 1 target column
- Some features used:
  - `age`, `income`, `savings`, `credit_score`
  - `loan_amount`, `loan_term_months`
  - `employment_years`, `home_ownership`
  - `education`, `marital_status`, `region`
  - `debt_to_income`, `has_credit_card`, `recent_default`
- The data is messy on purpose (missing values, typos, outliers) — just like real-world data.

## Steps I followed

1. **Explore the data** – look at the numbers, charts, and missing values.
2. **Clean the data** – fix typos, fill missing values, handle outliers.
3. **Prepare the data** – convert text columns into numbers, scale the numeric ones.
4. **Train models** – try 5 different models:
   - Logistic Regression
   - Decision Tree
   - Support Vector Machine (SVM)
   - Random Forest
   - XGBoost
5. **Check performance** – using accuracy, precision, recall, F1-score.
6. **Improve models** – tune settings using GridSearchCV to get better results.

## What I learned

- Cleaning messy data takes more effort than training the model itself.
- Accuracy alone can be misleading — recall matters a lot here, because missing an actual defaulter is worse than a false alarm.
- Simple models (Logistic Regression) give a good starting point, but tree-based models (Random Forest, XGBoost) usually perform better on this kind of data.

## Project status

🚧 In progress — EDA and cleaning done, model training next.

## Author

Made as part of my Machine Learning coursework.

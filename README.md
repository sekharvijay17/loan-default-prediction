# Loan Default Prediction

End-to-end machine learning project on a realistic synthetic credit-risk dataset — covering EDA, data cleaning, feature engineering, model training, evaluation, and hyperparameter tuning across five classification algorithms.

**Repo:** https://github.com/sekharvijay17/loan-default-prediction

---

## 📌 Project Overview

This project simulates a real-world loan default risk assessment problem. The dataset (10,000 rows × 20 features + 1 target) is synthetic but intentionally messy — containing missing values, categorical typos, outliers, and skewed distributions — to mirror the kind of preprocessing challenges seen in production data science work.

**Target variable:** `target_default_risk` (binary — 1 = Default, 0 = No Default)

**Goal:** Predict whether a borrower will default, and compare how different models and preprocessing choices affect performance.

---

## 🗂️ Repository Structure

```
loan-default-prediction/
├── generate_data.py       
├── preprocessing.py       
├── requirements.txt
└── README.md
```

---

## 🔍 Workflow

1. **Exploratory Data Analysis** — shape, dtypes, missing values, distributions, outliers, correlations, class balance.
2. **Data Preprocessing** — missing value imputation, fixing categorical typos (e.g. "Bachlors" → "Bachelors"), outlier capping (winsorization), one-hot/ordinal encoding, feature scaling, and feature engineering (e.g. `debt_to_income`, recency from `signup_date`, income per dependent).
3. **Model Building** — trained and evaluated:
   - Logistic Regression
   - Decision Tree
   - Support Vector Machine (SVM)
   - Random Forest
   - XGBoost
4. **Evaluation** — accuracy, precision, recall, F1-score, and confusion matrices for every model.
5. **Hyperparameter Tuning** — GridSearchCV / RandomizedSearchCV, focused on Random Forest and XGBoost, with baseline-vs-tuned comparison.

---

## 📊 Results Summary

| Model | Accuracy (baseline) | Accuracy (tuned) |
|---|---|---|
| Logistic Regression | ~ | — |
| Decision Tree | ~ | ~ |
| SVM | ~ | — |
| Random Forest | ~ | ~ |
| XGBoost | ~ | ~ |

*(Full metrics, confusion matrices, and discussion are in `reports/report.md` and the notebook.)*

---

## ⚙️ Setup & Usage

```bash
git clone https://github.com/sekharvijay17/loan-default-prediction.git
cd loan-default-prediction
pip install -r requirements.txt
python generate_data.py
python preprocessing.py
```

---

## 🛠️ Tech Stack

- Python 3
- pandas, numpy
- scikit-learn
- xgboost
- matplotlib, seaborn

---

## 📝 Notes

- The dataset is synthetic, generated to mimic realistic data quality issues (missing values, typos, outliers) for learning purposes — it does not represent real borrowers.
- Benchmark accuracy targets in the assignment are approximate; actual results depend on preprocessing and tuning choices, documented in the report.

---

## 📄 License

This project is for educational purposes.
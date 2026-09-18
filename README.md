# Loan Default / Credit Risk Prediction — Machine Learning

A machine-learning project for predicting loan default risk from borrower and loan-application data.

## Project Overview

This project follows the complete ML workflow:

**Load dataset → Filtering → Data cleaning → Exploratory analysis → Feature engineering → Feature selection → 70/30 train-test split → Preprocessing → Model training → Evaluation → ROC curves → Cross-validation → Class-imbalance handling → Feature importance → New-applicant prediction → Cost-benefit analysis → Risk tiering → Executive summary**

## Models Used

- Logistic Regression
- Decision Tree
- Random Forest

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Classification reports
- Confusion matrices
- ROC curves
- Cross-validation

## Dataset

`Loan_Default_csv.xlsx` is the project dataset used by the notebook.

The dataset contains borrower, loan, credit and application information, with `Status` used as the target after the notebook's cleaning/filtering steps.

## Feature Engineering

The notebook creates/uses risk-related features including:

- Loan-to-Income Ratio
- Loan-to-Property Ratio
- High-DTI Flag
- Low-Credit-Score Flag
- Application year/month
- Age grouping / normalized credit-related features where applicable

## Risk Tiering

The notebook demonstrates:

- Low Risk: default probability below 20%
- Medium Risk: 20%–50%
- High Risk: above 50%

These thresholds are for the project demonstration and should not be treated as lending-policy rules.

## How to Run

### Google Colab

1. Upload `Loan_Default_csv.xlsx`.
2. Open `loan_default_ml_models.ipynb`.
3. Run the notebook from top to bottom.

### Local Python / Jupyter

Install dependencies:

```bash
pip install -r requirements.txt
```

Then open the notebook:

```bash
jupyter notebook loan_default_ml_models.ipynb
```

## Repository Structure

```text
loan-default-prediction/
├── loan_default_ml_models.ipynb
├── Loan_Default_csv.xlsx
├── README.md
├── requirements.txt
├── DATA_DICTIONARY.md
├── .gitignore
└── LICENSE
```

## Important Note

This is an educational machine-learning project. A real lending deployment would require additional validation, monitoring, fairness checks, explainability, data-governance controls and regulatory/compliance review.

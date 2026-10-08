# CreditWise Loan System

A machine learning system that predicts whether a loan application should be **approved or rejected** based on the applicant's financial and personal details, helping lenders make faster and more consistent decisions.

## Problem Statement
Manual loan screening is slow and can be inconsistent. This project builds a model that learns from past applications to predict loan approval and highlights the factors that matter most.

## Dataset
- Source: Kaggle 
- Size: <rows x columns>
- Features: income, credit score, loan amount, employment status, existing debt, etc.
- Target: <Loan_Status / Approved (Yes/No)>

## Approach
1. Data cleaning and handling missing values
2. Exploratory data analysis (distributions, correlations)
3. Encoding categorical variables
4. Feature scaling
5. Train-test split
6. Model training: Logistic Regression, Gaussian Naive Bayes,knn
7. Evaluation and model comparison

## Results
| Model | Accuracy | Precision | Recall | F1 |
| Logistic Regression | 0.875 | 0.790  | 0.803 | 0.796 |
| knn | 0.76 | 0.62 | 0.524 | 0.571 |
| Naive Bayes | 0.865 | 0.803  | 0.737 | 0.769 |

Best model : Logistic Regression with 87.6 % accuracy

## Key Insights
- Credit score and income were the strongest predictors
- Applicants with high existing debt were more likely to be rejected

## Tech Stack
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Jupyter Notebook


## How to Run
```
git clone https://github.com/asthachouhan06/CreditWise_Loan_System.git
cd CreditWise_Loan_System
pip install -r requirements.txt
jupyter notebook credit_wise.ipynb
```

## Future Work
- Hyperparameter tuning, handling class imbalance (SMOTE)
- Deploy as a web app (Streamlit / Flask)

## Author
Astha Chouhan | asthachouhan06@gmail.com
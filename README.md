# FinTech Innovations - Loan Approval Risk Model

Machine learning model predicting loan approval decisions to replace inconsistent manual review. Follows the CRISP-DM framework.

## Dataset
'financial_loan_data.csv' - 20,000 historical loan applications. Target: 'LoanApproved' (binary).

## Approach
1. Business understanding - asymmetric cost analysis ($50k per bad approval, $8k per missed good loan)
2. Data exploration - EDA, missing value analysis, feature engineering
3. Preprocessing - ColumnTransformer with separate numeric/categorical pipelines
4. Modeling - 5 algorithms compared; top model tuned via GridSearchCV
5. Evaluation - ROC-AUC, recall, and custom Expected Dollar Loss metric

## Key Results
- Best model: [Tuned Gradient Boosting]
- Test ROC-AUC: [0.999996]
- Dollar savings vs. baseline: [99.24%]

## File
- 'fintech_loan_approval.ipynb' - full analysis notebook

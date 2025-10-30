# SuperLender-Loan-Prediction
This project predicts whether a loan will be Good (1) or Bad (0) using machine learning models. The goal is to help SuperLender assess credit risk effectively.
---

SuperLender is a digital lending company struggling with loan defaults. Using customer demographics, loan history, and repayment behavior, this project builds machine learning models to predict the likelihood that a new loan will be repaid (“Good”) or default (“Bad”).
The analysis revealed that loan amount, repayment history, and employment status were among the strongest predictors of creditworthiness.
With the best-performing model (Random Forest, 95.87% accuracy), SuperLender can automate risk scoring and reduce default rates by focusing on high-risk applicants before disbursing loans.

## Datasets
1. **traindemographics.csv** – Customer demographic information  
2. **trainperf.csv** – Performance of current loans (target: good_bad_flag)  
3. **trainprevloans.csv** – History of previous loans  
4. **test...** files – Similar structure for testing
---

## Features
- Data cleaning (handling nulls, datetime conversion)
- Feature engineering (loan ratios, repayment gaps, etc.)
- Correlation analysis via heatmap
- Multiple ML models:
  - Logistic Regression
  - SVM
  - KNN
  - LightGBM
  - XGBoost
  - Gradient Boosting
- Model comparison and evaluation using accuracy, ROC-AUC, and confusion matrix.
---

### Data Cleaning
****-Converted date columns to datetime
Removed null values and irrelevant columns
Merged all train and test data into unified datasets
- Feature Engineering
Created ratios such as totaldue / loanamount
Calculated repayment duration and loan term features
Encoded categorical variables (education, bank name, etc.)
- Exploratory Data Analysis
Correlation analysis with heatmap
Visualization of loan amount distribution and term duration
Identification of key predictors for default****
---
###Key Insights
-Customers with shorter repayment gaps and stable employment have better repayment behavior.
-Loan amount and education level strongly influence credit performance.
-Ensemble models (Random Forest, LightGBM, XGBoost) achieved the best overall accuracy and ROC-AUC.

## Results
- LightGBM achieved the best performance (highest ROC-AUC).  
- Feature importance plots highlight key predictors of loan repayment.
---

### Technologies
- Python 3
- Pandas, NumPy
- Scikit-learn
- LightGBM, XGBoost
- Matplotlib, Seaborn
- Jupyter Notebook

---

Thank you for viewing this project! Feedback and suggestions are welcome. 
---

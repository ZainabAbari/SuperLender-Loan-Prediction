# SuperLender-Loan-Prediction
This project predicts whether a loan will be Good (1) or Bad (0) using machine learning models. The goal is to help SuperLender assess credit risk effectively.

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

## Results
- LightGBM achieved the best performance (highest ROC-AUC).  
- Feature importance plots highlight key predictors of loan repayment.

---

## 🧰 Technologies
- Python 3
- Pandas, NumPy
- Scikit-learn
- LightGBM, XGBoost
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/loan-default-prediction.git
   cd loan-default-prediction

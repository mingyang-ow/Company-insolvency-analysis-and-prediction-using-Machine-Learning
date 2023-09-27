## <strong>Company Insolvency Exploratory Data Analysis and prediction using Machine Learning</strong>
This notebook is designed for the examination of financial data from 9792 Polish companies. Its primary objective is to assess the solvency of these companies and predict the likelihood of insolvency.<br>
To evaluate the model's performance, it was pitted against a dummy model and the Altman Z-Score in a test scenario. <br>
This comparison was done to gauge the model's effectiveness in predicting insolvency risk. <br>

The were taken from the UCI Machine Learning Repository Repository: http://archive.ics.uci.edu/ml/datasets/polish+companies+bankruptcy+data

# Approach
1. Exploratory Data Analysis (EDA)
  - Understand data distributions and correlations between data and insolvency risk
2. Design Classification ML Model
  - Plan ML model using results from EDA
  - Selecting ML model 
  - Upsampling
  - Hyperparameter tuning
3. Analysis
  - Tuned model compared against dummy model to test for prediction accuracy
  - Tuned model compared against Altman's Z-Score in a test scenario to test for prediction accuracy

# Metric
1. Measuring Return of Investment (ROI) of ML model predictions or Altman's Z-Score to approve or deny loans in test scenario
2. ROI made from ML model predictions measured against ROI made from Altman's Z-Score predictions in test scenario
* Test scenario: Starting cash of $0, with approved companies given $10000 per loan, at 5% interest when repaying loans. Bankrupt companies will not repay loans

# Conclusion
The tuned Gradient Boosting Classifier Model was more accurate in approving profitable loans, compared to using the Altman's Z-Score, and produced a greater ROI<br>
<br>
**Tuned Gradient Boosting Classifier Model:**<br>
f1 score: 0.181<br>
Final cash: $630000<br>
Approved loans: 2373<br>
Denied loans: 108<br>
Repaid loans: 2320<br>
Defaulted loans: 53<br>
<br>

**Altman's Z-Score:**<br>
f1 score: 0.098<br>
Final cash: $555500<br>
Approved loans: 2224<br>
Denied loans: 257<br>
Repaid loans: 2171<br>
Defaulted loans: 53<br>



# Google Advanced Data Analytics Capstone  
**Salifort Motors – Employee Churn Prediction**  

**Evelyn Roxana Pérez Umana** • PhD Pathology → Data Scientist (Health & Biotech)  
Google Advanced Data Analytics Professional Certificate – Dic 2025  

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)

## Business problem
Predict employee turnover using highly imbalanced HR data (churn ≈ 3%).

## Model results – Logistic Regression (baseline)
| Metric                | Value | Notes                                      |
|-----------------------|-------|--------------------------------------------|
| Accuracy              | 0.82  | High due to class imbalance                |
| Precision (churn)     | 0.44  |                                            |
| Recall (churn)        | 0.26  | Only 26 % of actual leavers detected       |
| F1-score (churn)      | 0.33  |                                            |

**Top predictors**  
`last_evaluation` • `number_project` • `average_montly_hours` • `time_spend_company` • `satisfaction_level`

## Confusion Matrix
![Confusion Matrix](confusion_matrix.png)

## Real conclusion (honest & professional)
The baseline logistic regression model achieves 82 % accuracy, but its **recall for the minority class (employees who actually leave) is only 26 %**.  
This is a classic symptom of severe class imbalance. While the model is simple and interpretable, it fails to identify most employees at risk of leaving — exactly the ones the business most needs to retain.

**Production recommendation**  
In a real environment I would implement stronger models (Random Forest or XGBoost) and/or resampling techniques (SMOTE, class_weight='balanced') to significantly improve recall without sacrificing overall performance.

## Healthcare & Clinical Research applications (PhD perspective)
The same challenge appears constantly in biomedical settings:  
- Predicting patient dropout in long-term clinical trials  
- Forecasting treatment non-adherence in postmenopausal hormone therapy  
- Early detection of physician burnout using HR + inflammatory biomarkers  

## Links
## Links
- [Interactive Notebook](https://github.com/umanaevelyn/google-advanced-data-analytics-capstone/blob/main/Salifort_Motors_Capstone.ipynb)  
- [View on nbviewer – pretty render](https://nbviewer.org/github/umanaevelyn/google-advanced-data-analytics-capstone/blob/main/Salifort_Motors_Capstone.ipynb)  
- [Portfolio](https://umanaevelyn.github.io) • [LinkedIn](https://www.linkedin.com/in/evelyn-roxana-perez-umana)

© 2025 Evelyn Roxana Perez Umana

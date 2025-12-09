
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

![Confusion Matrix](confusion_matrix.png)

## Real conclusion
The baseline model achieves 82 % accuracy but only detects **26 %** of employees who actually leave.  
In production I would use Random Forest / XGBoost + resampling techniques to significantly improve recall.

## Healthcare applications
Same pipeline applicable to patient dropout prediction in clinical trials and treatment adherence in postmenopausal cohorts.

## Links
- [Interactive Notebook](https://github.com/umanaevelyn/google-advanced-data-analytics-capstone/blob/main/Salifort_Motors_Capstone.ipynb)  
- [View on nbviewer – pretty render](https://nbviewer.org/github/umanaevelyn/google-advanced-data-analytics-capstone/blob/main/Salifort_Motors_Capstone.ipynb)  
- [Portfolio](https://umanaevelyn.github.io) • [LinkedIn](https://www.linkedin.com/in/evelyn-roxana-perez-umana)

© 2025 Evelyn Roxana Perez Umana

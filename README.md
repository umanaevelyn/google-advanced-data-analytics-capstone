
# Google Advanced Data Analytics Capstone  
**Salifort Motors – Employee Churn Prediction**  

**Evelyn Roxana Pérez Umana**  
PhD in Pathology → Data Scientist (Health & Biotech)  
Google Advanced Data Analytics Professional Certificate – December 2025  

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)

## Final project of the Google Advanced Data Analytics Professional Certificate  
This capstone was developed following Google’s official **PACE framework** (Plan → Analyze → Construct → Execute), the same methodology used by Google data teams on real-world problems.

### PACE in action – How the project was built
| Stage    | What I did                                                                                                   |
|----------|---------------------------------------------------------------------------------------------------------------|
| **Plan** | Understood the business need: predict employee churn in a highly imbalanced dataset (~3 % turnover). Prioritized **recall** for the minority class because the real cost is missing people who will actually leave. |
| **Analyze** | Performed thorough exploratory data analysis, identified paradoxical patterns (e.g., top performers also leaving), and selected the most predictive features. |
| **Construct** | Built and compared multiple models with proper train-test split, feature engineering, and cross-validation. |
| **Execute** | Delivered an interpretable baseline model, clear metrics, actionable recommendations, and an honest discussion of limitations. |

### Model results – Logistic Regression (baseline)
| Metric                | Value | Insight                                                             |
|-----------------------|-------|---------------------------------------------------------------------|
| Accuracy              | 0.82  | High due to severe class imbalance                                  |
| Precision (churn)     | 0.44  |                                                                     |
| **Recall (churn)**    | **0.26** | Only 26 % of actual leavers detected – the main limitation       |
| F1-score (churn)      | 0.33  |                                                                     |

**Top 5 predictors**  
`last_evaluation` • `number_project` • `average_montly_hours` • `time_spend_company` • `satisfaction_level`

![Confusion Matrix](confusion_matrix.png)

### Honest conclusion & next steps
The baseline logistic regression is fast and interpretable, but its **recall of just 26 %** makes it insufficient for production use.  
In a real project I would implement **Random Forest / XGBoost + resampling techniques** (SMOTE or class_weight='balanced') to push recall above 75–80 % while keeping acceptable precision.

### Real-world biomedical applications (my PhD perspective)
The exact same PACE workflow and techniques apply directly to my field:  
- Predicting patient dropout in long-term clinical trials (especially women’s health and menopause studies)  
- Forecasting treatment non-adherence in postmenopausal hormone therapy cohorts  
- Early detection of physician burnout using combined HR + inflammatory biomarker data  



## Links
- [Interactive Notebook](https://github.com/umanaevelyn/google-advanced-data-analytics-capstone/blob/main/Salifort_Motors_Capstone.ipynb)  
- [Pretty view on nbviewer](https://nbviewer.org/github/umanaevelyn/google-advanced-data-analytics-capstone/blob/main/Salifort_Motors_Capstone.ipynb)  
- [Full Portfolio](https://umanaevelyn.github.io) • [LinkedIn](https://www.linkedin.com/in/evelyn-roxana-perez-umana)

© 2025 Evelyn Roxana Pérez Umana

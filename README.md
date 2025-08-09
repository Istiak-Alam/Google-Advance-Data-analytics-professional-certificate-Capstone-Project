# Predicting Employee Turnover

[View Full Project Notebook](https://github.com/Istiak-Alam/Google-Advance-Data-analytics-professional-certificate-Capstone-Project/blob/main/Salifort_Motors_project_lab.ipynb)

---

## Overview

This project predicts employee turnover using multiple logistic regression and machine learning algorithms, including:

- Decision Tree  
- Random Forest  
- XGBoost (best performing)  

The dataset is from the fictional company **Salifort Motors** and is part of the Google Advanced Data Analytics Professional Certificate Capstone Project.

| Model Name                       | Precision | Recall | F1 Score | Accuracy | AUC   |
|---------------------------------|-----------|--------|----------|----------|-------|
| XGBoost (with feature engineering) | 90.1%     | 87.8%  | 89.0%    | 96.4%    | 97.0% |

The key predictive features for employee turnover include:  
`number_project`, `tenure`, `last_evaluation`, `overworked` (hours > 175/month), `work_accident`, and `salary`.

---

## Business Understanding

Salifort Motors faces costly employee turnover due to investments in recruitment, training, and upskilling. By predicting which employees are likely to leave and understanding key drivers, leadership can develop targeted retention strategies to reduce turnover and improve workplace culture.

---

## Data Understanding

- **Source:** Kaggle HR Analytics Dataset  
- **License:** Creative Commons Zero (CC0)  
- **Size:** ~12,000 employee records  
- **Features:** Employee satisfaction, last evaluation, number of projects, average monthly hours, tenure, work accidents, promotions, department, salary level, turnover status (target variable)

---

## Employee Turnover Proportion

*Include your turnover proportion image here (upload to repo and link)*  
`![Employee Turnover Proportion](Images/left.png)`

---

## Modeling & Evaluation

An XGBoost model with tuned hyperparameters and feature engineering was built to classify employees as staying or leaving. The feature importance plot below highlights the top factors influencing turnover:

*Include your feature importance image here*  
`![Feature Importances - XGBoost with Feature Engineering](Images/fi_xgb_fe.png)`

---

## Conclusion

The XGBoost model effectively predicts employee turnover with high accuracy and recall. By focusing retention efforts on key predictive factors, Salifort Motors can reduce employee churn and foster a better work environment.

---

## Tools & Technologies

- Python (Pandas, NumPy, Scikit-learn, XGBoost)  
- Jupyter Notebook  
- Matplotlib & Seaborn for visualization  

---

## How to Run

```bash
git clone https://github.com/Istiak-Alam/Google-Advance-Data-analytics-professional-certificate-Capstone-Project.git
cd Google-Advance-Data-analytics-professional-certificate-Capstone-Project
pip install -r requirements.txt
jupyter notebook Salifort_Motors_project_lab.ipynb

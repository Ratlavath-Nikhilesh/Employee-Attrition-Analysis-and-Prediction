# Employee Attrition Analysis and Prediction

## Project Overview

Employee attrition has a significant impact on organizational performance and hiring costs. This project aims to analyze employee-related factors and build a machine learning model to **predict employee attrition**, i.e., whether an employee is likely to leave or stay in the organization.

The project follows a structured machine learning pipeline, starting from data validation and preprocessing, followed by feature engineering, model training, and evaluation. Special emphasis is placed on **maximizing recall**, ensuring that employees at risk of leaving are identified effectively.

---

## Dataset

- **Source:** Kaggle  
- **Link:** https://www.kaggle.com/datasets/stealthtechnologies/employee-attrition-dataset/data  

### Dataset Size

- Training data: **59,598 records**
- Test data: **14,900 records**
- Total columns: **24** (including target)

### Target Variable

- **Attrition**
  - `0` → Stayed  
  - `1` → Left  

---

## Methodology (High-Level)

- Validated dataset structure and target distribution  
- Performed data preprocessing for numeric and categorical features  
- Applied feature engineering to create domain-relevant risk indicators  
- Encoded features and prepared model-ready datasets  
- Trained multiple models with hyperparameter tuning using Optuna  
- Selected the best-performing model based on recall  

---

## Model and Result

- **Final Model:** XGBoost Classifier  
- **Optimization:** Optuna with probability threshold tuning  

### Key Performance Metric

- **Final Recall:** **0.889**

This high recall ensures that most employees who are likely to leave are successfully identified, making the model suitable for practical HR attrition risk analysis.

---

## Conclusion

This project demonstrates a complete and practical machine learning workflow for employee attrition prediction. By combining structured preprocessing, meaningful feature engineering, and recall-focused model selection, the final model effectively identifies employees at high risk of attrition.


# Adverse Model Prediction for Hospital Readmissions


![Description of Image](https://github.com/kwakpovwe/Predict-30-day-hospital-readmission-or-emergency-visits-likelihood./blob/main/DATASET/hospitalization.jpg?raw=true)



## Overview

This project focuses on predicting the likelihood of hospital readmissions or emergency visits within 30 days of patient discharge. By accurately identifying high-risk patients, healthcare providers can prioritize interventions, reduce hospital resource usage, and improve patient outcomes.

## Objective

The primary goal is to build an interpretable and efficient machine learning model to:

    Predict patients at high risk of readmission.
    Highlight key predictors driving readmissions for actionable interventions.

## Key Features

    Data Integration: Combining multiple healthcare-related datasets for a comprehensive patient profile.
    Feature Engineering: Creating new features like High-Risk Medication and Total Healthcare Visits to enhance predictive capabilities.
    Class Imbalance Handling: Techniques to balance the target variable for accurate model performance.
    Model Comparison: Comparing Logistic Regression, Random Forest, XGBoost, LightGBM, and CatBoost.
    Explainability with SHAP: Using SHAP values to interpret model predictions.
    Actionable Insights: Identifying key features like Medication_Metformin and Medication_Salbutamol as critical indicators of readmission risk.

## Datasets Used

    Coded_Conditions.csv: Standardized records of diagnosed medical conditions.
    Medications.csv: Prescription details for pharmacological analysis.
    A_and_E.csv: Data on Accident & Emergency visits.
    Emergency_Admissions.csv: Insights into emergency hospital admissions.
    Outpatients.csv: Follow-up and outpatient visit records.
    Social_Care.csv: Social care service usage impacting patient health.

## Steps in the Project

    Data Preparation:
    Merging datasets using Patient_ID as the primary key.
    Handling missing values:
    Numerical: Replaced with mean.
    Categorical: Replaced with mode.
    
## Feature Engineering:
        Key new features:
        - Total Healthcare Visits
        - Count of Comorbidities
        - High-Risk Medications

## Class Imbalance Management:
        Addressed imbalance to ensure the model focuses on both low-risk and high-risk patients.

## Data Splitting:
        Train (70%), Validation (15%), Test (15%) for unbiased evaluation.

## Model Selection:
        Compared 5 models:
        Logistic Regression, Random Forest, XGBoost, LightGBM, CatBoost.

## Evaluation:
        Metrics: Accuracy, Precision, Recall, F1-Score, and AUC-ROC.

## Model Explainability:
        Used SHAP Analysis to validate and explain feature contributions.

## Why Logistic Regression Was Selected

    Achieved perfect performance on test data.
    Provides probabilistic outputs for risk stratification.
    Easy to interpret and deploy in clinical environments.

## Top predictors:
        Medication_Salbutamol: High association with respiratory issues.
        Medication_Metformin: Strong link to diabetes-related readmissions.

## Insights from SHAP Analysis

    SHAP values confirmed the importance of:
        Medication_Metformin
        Medication_Salbutamol
        Age and Comorbidity Counts.
    SHAP analysis enhances trust in the model's predictions and provides transparency.

## Actionable Steps

    Targeted Interventions: Prioritize follow-ups for high-risk patients (e.g., flagged medications like Salbutamol).
    Integration: Embed the model into healthcare systems for real-time risk assessment.
    Resource Optimization: Focus resources on top 10 high-risk patients identified by the model.

## Contact

For questions or collaborations, reach out:

Peter Kwakpovwe

    Email: P.kwakpovwe@gmail.com or peter.kwakpovwe@gmail.com
    LinkedIn: Peter Kwakpovwe

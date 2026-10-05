# Thyroid Cancer Recurrence Prediction

## Project Overview
This project explores the **Differentiated Thyroid Cancer Recurrence** dataset from the UC Irvine Machine Learning Repository. The goal is to predict whether a patient's differentiated thyroid cancer will recur based on demographic and clinical variables collected at the time of diagnosis.

## Objective
To build and evaluate binary classification models that predict thyroid cancer recurrence (`Recurred`: Yes/No) using patient demographics, clinical history, and diagnostic staging information.

## Dataset
- **Name:** Differentiated Thyroid Cancer Recurrence
- **Source:** [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/915/differentiated+thyroid+cancer+recurrence)
- **Observations:** 383 patients
- **Features:** 16 predictor variables (demographic, lifestyle, and clinical)
- **Target Variable:** `Recurred` (binary: Yes/No)

### Predictor Variables Include:
- **Demographics:** Age, Gender
- **Lifestyle/History:** Smoking, History of Smoking, History of Radiotherapy
- **Clinical/Diagnostic:** Thyroid Function, Physical Examination, Adenopathy, Pathology, Focality, Risk Classification, T/N/M Staging, Overall Stage, Treatment Response


## Methods & Approach

### 1. Data Exploration
- Imported dataset and examined structure, data types, and summary statistics
- Visualized target variable distribution and relationships between key predictors (Age, Risk Classification) and recurrence outcome

### 2. Data Quality Assessment
- Checked for missing values and inconsistent categorical coding
- Identified potential challenges, including class imbalance and high-dimensionality after encoding categorical variables

### 3. Preprocessing
- Encoded categorical variables (one-hot/label encoding)
- Scaled numeric features as needed
- Addressed class imbalance in the target variable

### 4. Modeling
- Trained and compared classification models, including:
  - Logistic Regression
  - Random Forest
- Evaluated models using cross-validation and metrics including:
  - F1-score
  - AUC-ROC
  (prioritized over raw accuracy due to class imbalance)

### 5. Interpretation
- Reviewed feature importance to identify which clinical variables were most predictive of recurrence
- Compared findings to known clinical risk factors for thyroid cancer recurrence

## How to Run



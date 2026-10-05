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
- Encoded categorical variables
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
1. Go to this GitHub repository and download or clone it using GitHub Desktop, or simply download the ZIP file by clicking **Code > Download ZIP**.

2. Locate the notebook file (`thyroid_recurrence_analysis.ipynb`) and the dataset file (`Thyroid_Diff.csv`) included in this repository.

3. Open Google Colab at [https://colab.research.google.com](https://colab.research.google.com).

4. Select **File > Upload Notebook**, then upload `thyroid_recurrence_analysis.ipynb` from this repository.

5. Once the notebook is open, upload the dataset file (`Thyroid_Diff.csv`) using the file upload cell included at the top of the notebook, or mount Google Drive if you've stored the file there.

6. Make sure the file path in the notebook matches wherever you uploaded the dataset.
## Requirements
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

Original Colab Link to Project: https://colab.research.google.com/drive/1KS-CcKHKJ8Y4huOswWIfl-hSLZd5oGQB#scrollTo=W4RUud0oIrXJ



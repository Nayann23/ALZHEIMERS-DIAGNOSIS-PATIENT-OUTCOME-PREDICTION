# ALZHEIMERS-DIAGNOSIS-PATIENT-OUTCOME-PREDICTION

**INCOMPLETE! Needs further testing.**

A machine learning project aimed at predicting patient outcomes based on Alzheimer’s diagnosis data. The project includes data exploration, preprocessing, handling imbalanced datasets, and model evaluation using logistic regression and random forest classifiers.

---

## Table of Contents

- [Project Overview](#project-overview)  
- [Dataset](#dataset)  
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)  
- [Preprocessing](#preprocessing)  
- [Handling Imbalanced Data](#handling-imbalanced-data)  
- [Modeling](#modeling)  
- [Evaluation](#evaluation)  
- [Future Work](#future-work)  
- [Installation](#installation)  

---

## Project Overview

This project focuses on predicting whether a patient has Alzheimer’s disease based on demographic, lifestyle, and health-related features. The workflow follows standard machine learning pipeline practices including:

- Data cleaning and inspection  
- Exploratory Data Analysis (EDA) with visualizations  
- Feature encoding (OneHotEncoding) and scaling  
- Train/Test splitting  
- Handling imbalanced classes using SMOTE  
- Model training and evaluation with logistic regression and random forest  
- Hyperparameter tuning and cross-validation  

---

## Dataset

The dataset includes the following types of features:

- **Demographic**: Age, Gender, Country, Marital Status, Income Level, Urban/Rural Living  
- **Health-related**: BMI, Physical Activity Level, Smoking Status, Alcohol Consumption, Diabetes, Hypertension, Cholesterol Level, Family History of Alzheimer’s, Depression Level, Sleep Quality, Dietary Habits, Air Pollution Exposure, Genetic Risk Factor (APOE-ε4 allele), Stress Levels  
- **Cognitive**: Cognitive Test Score  
- **Target**: Alzheimer’s Diagnosis (Yes/No)

Some columns like Employment Status and Social Engagement Level were removed during preprocessing due to low predictive power.

---

## Exploratory Data Analysis (EDA)

- Histograms for numeric features  
- Countplots for categorical features  
- Correlation heatmap for numeric features  
- Pairplots for numeric features  

All visualizations are saved in the `Visuals/` directory and logged using Python’s `logging` module.

---

## Preprocessing

- Dropped irrelevant columns  
- Scaled numeric features using `StandardScaler`  
- One-hot encoded categorical features using `OneHotEncoder`  
- Separated features (X) and target (y)  

---

## Handling Imbalanced Data

The target variable (`Alzheimer’s Diagnosis`) is imbalanced. SMOTE (Synthetic Minority Over-sampling Technique) was applied to the training set to balance classes.

---

## Modeling

Two models were used:

1. **Logistic Regression**  
   - Fitted on SMOTE-resampled training data  
   - Hyperparameter tuning performed using `GridSearchCV` with F1-score as metric  

2. **Random Forest Classifier**  
   - Fitted on SMOTE-resampled training data  
   - Hyperparameter tuning performed using `GridSearchCV`  

---

## Evaluation

- Accuracy, confusion matrix, and classification report for both models  
- Cross-validation performed to check model stability  
- Best F1-scores logged for each model  

---

## Future Work

- Further hyperparameter tuning for both logistic regression and random forest  
- Test additional models such as Gradient Boosting or XGBoost  
- Evaluate using more metrics like ROC-AUC, precision-recall curves  
- Perform feature engineering to improve predictive performance  
- Improve EDA with more detailed statistical analysis  
- Automate pipeline for reproducibility  

---

## Installation

Clone this repository:

```bash
git clone https://github.com/Nayann23/ALZHEIMERS-DIAGNOSIS-PATIENT-OUTCOME-PREDICTION.git
cd ALZHEIMERS-DIAGNOSIS-PATIENT-OUTCOME-PREDICTION
```

----


## 📜 License

This project is open-source and licensed under the [MIT License](LICENSE). See the LICENSE file for full details.

---

## 👤 Author:  **Nayan Darokar** 

## GitHub
```bash
https://github.com/Nayann23
```

## Email:
```bash
reachout.nayan@gmail.com  
```
## Portfolio: 
```bash
https://nayan-datascience-portfolio.vercel.app/
```


## Install required dependencies:

```bash
pip install -r requirements.txt

```

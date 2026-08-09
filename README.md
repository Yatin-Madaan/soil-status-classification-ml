# Soil Status Classification Using Machine Learning

## Overview

This project develops a supervised machine learning pipeline for binary classification of soil nutrient status.

The objective is to predict whether soil nutrient status is **Sufficient** or **Insufficient** using soil properties and agricultural management factors.

## Dataset

The dataset contains 3,000 samples and 13 columns, including:

- pH
- Organic Matter
- Nitrogen
- Phosphorus
- Potassium
- CEC
- Soil Moisture
- Soil Type
- Region
- Crop Type
- Irrigation Level
- Fertilizer Use
- Soil Status (target)

## Machine Learning Workflow

The project follows a complete ML workflow:

1. Data exploration and statistical analysis
2. Missing-value analysis and cleaning
3. Train-validation-test splitting
4. Feature preprocessing
5. Feature engineering
6. Stratified cross-validation
7. Hyperparameter optimization
8. Model comparison
9. Hold-out test evaluation
10. Final model training and prediction

## Preprocessing

The workflow includes:

- Mean imputation for numerical variables
- Most-frequent imputation for categorical variables
- One-hot encoding of categorical features
- Ordinal encoding of irrigation level
- StandardScaler for numerical features
- Preprocessing within cross-validation folds to reduce data leakage

## Models

Five classification algorithms were evaluated:

- K-Nearest Neighbors (KNN)
- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- XGBoost

Hyperparameters were optimized using **Grid Search** and **Random Search**, depending on the model and search space.

## Evaluation

**Matthews Correlation Coefficient (MCC)** was used as the primary evaluation metric.

The models were compared using the same StratifiedKFold cross-validation strategy to ensure a consistent evaluation framework.

A separate hold-out test set was used for final generalisation evaluation.

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn
- Jupyter Notebook

## Repository Contents

- `AI_01_project.ipynb` — complete machine learning workflow and analysis

## Author

**Yatin Madaan**

MSc Digital Farming  
Hochschule Weihenstephan-Triesdorf (HSWT)

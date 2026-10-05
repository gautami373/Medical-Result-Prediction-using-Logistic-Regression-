# Medical Result Prediction using Logistic Regression

## Project Overview

This project uses Logistic Regression to predict the medical `Result` based on patient health-related features.

The dataset contains medical measurements such as Age, Gender, Heart rate, blood pressure, Blood sugar, CK-MB, and Troponin.

The target variable is `Result`, which contains two classes:

- `negative`
- `positive`

## Objective

The main objective of this project is to build a binary classification model that predicts whether a medical result is positive or negative.

## Dataset

The project uses the `Medicaldataset (1).csv` dataset.

### Features

- Age
- Gender
- Heart rate
- Systolic blood pressure
- Diastolic blood pressure
- Blood sugar
- CK-MB
- Troponin

### Target Variable

`Result`

- `negative` → Negative result
- `positive` → Positive result

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

## Machine Learning Algorithm

### Logistic Regression

Logistic Regression is used for binary classification.

The model is trained using balanced class weights.

```python
from sklearn.linear_model import LogisticRegression

model = LogisticRegression(
    class_weight="balanced",
    random_state=42
)

model.fit(X_train, y_train)

# Artificial Intelligence Project – Medical Result Prediction using Logistic Regression

## Project Overview

This project is an **Artificial Intelligence and Machine Learning project** that uses **Logistic Regression** to predict whether a medical test result is **Positive** or **Negative**.

The project demonstrates the complete machine learning workflow, including data loading, exploratory data analysis, preprocessing, model training, prediction, evaluation, and feature analysis.

---

## Project Objective

The main objective of this project is to build a machine learning model that can predict the medical **Result** based on patient health-related features.

### Target Classes

- **Negative** – Negative medical result
- **Positive** – Positive medical result

---

## Dataset

The dataset used in this project is:

**`Medicaldataset (1).csv`**

### Features

The dataset contains the following features:

- Age
- Gender
- Heart rate
- Systolic blood pressure
- Diastolic blood pressure
- Blood sugar
- CK-MB
- Troponin

### Target

- Result

The target contains two classes:

- `negative`
- `positive`

---

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

---

## Machine Learning Algorithm

### Logistic Regression

Logistic Regression is a supervised machine learning algorithm used for classification problems.

In this project, Logistic Regression is used for **binary classification** to predict whether the medical result is positive or negative.

---

## Project Workflow

The project follows these steps:

1. Import required libraries
2. Upload and load the dataset
3. Inspect the dataset
4. Check missing values
5. Check duplicate values
6. Perform Exploratory Data Analysis (EDA)
7. Encode categorical data
8. Separate features and target
9. Split data into training and testing sets
10. Handle missing values using median imputation
11. Standardize the features
12. Train the Logistic Regression model
13. Make predictions
14. Evaluate the model
15. Generate confusion matrix
16. Generate ROC curve and calculate ROC-AUC
17. Analyze model coefficients
18. Save the trained model

---

## Data Preprocessing

The following preprocessing techniques were used:

### 1. Categorical Encoding

The `Gender` column was converted into numerical form using one-hot encoding.

```python
pd.get_dummies(X, columns=["Gender"], drop_first=True)

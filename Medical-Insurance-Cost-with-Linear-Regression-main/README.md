# Polynomial Regression on Medical Charges Dataset

This repository contains a Python project that applies Polynomial Regression to predict medical charges based on various features such as age, BMI, number of children, and smoking status. The project leverages the `scikit-learn` library for model training and evaluation.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Model Training](#model-training)
- [Feature Importance](#feature-importance)
- [Results](#results)

## Project Overview

This project demonstrates the use of Polynomial Regression to model the relationship between features like age, BMI, number of children, and smoking status to predict medical charges. The model is evaluated using metrics such as R² score.

## Dataset

The dataset used in this project contains the following features:

- **age**: Age of the individual
- **bmi**: Body Mass Index (BMI)
- **children**: Number of children covered by health insurance
- **smoker**: Smoking status (Yes/No)
- **region**: The region where the individual resides
- **charges**: The medical charges incurred by the individual

Note: The dataset should be in CSV format, and the project assumes the dataset is loaded into a pandas DataFrame named `df`.

## Installation

To run this project, you need to have Python 3 installed along with the following libraries:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

You can install the required packages using `pip`:

## Model Training
  1. The model is trained using Polynomial Regression with a degree of 2. The following steps are performed:
  2. Dropping unnecessary features such as sex and region.
  3. Creating polynomial features from the remaining features.
  4. Splitting the data into training and testing sets using an 80/20 split.
  5. Training a LinearRegression model on the transformed features.
  6. Evaluating the model using the R² score.

## Feature Importance
The importance of each feature is calculated and displayed. The features with the highest importance are plotted in a bar chart.

## Results

After training the model, the following outputs are generated:

1. **Intercept**: The intercept of the polynomial regression model.
2. **Coefficients**: The coefficients of the polynomial regression model.
3. **R² Score**: The R² score on the test set, which indicates the model's performance.

### Actual vs. Predicted Values

A DataFrame is created to compare the actual medical charges with the predicted charges for the test set. This comparison helps to visually assess the accuracy of the model's predictions.

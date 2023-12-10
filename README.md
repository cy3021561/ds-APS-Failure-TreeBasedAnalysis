# Tree-Based Methods for APS Failure Data Analysis

## Overview

This project involves analyzing the APS Failure data from Scania Trucks using tree-based methods. It includes handling missing data, feature selection, and applying advanced machine learning techniques like random forests and XGBoost.

## Data Source

- **APS Failure Data**: [UCI Machine Learning Repository - APS Failure at Scania Trucks](https://archive.ics.uci.edu/ml/datasets/APS+Failure+at+Scania+Trucks)
- **Dataset Details**: The dataset comprises a training set with 60,000 rows (1,000 positive class instances) and a test set. It includes 171 numeric attributes.

## Tasks

### 1. Data Preparation

#### (a) Missing Value Treatment

- Research and apply techniques for handling missing data.

#### (b) Feature Analysis

- Calculate the coefficient of variation (CV) for each of the 170 features.
- Create a correlation matrix for the features.
- Select features with the highest CV and visualize them using scatter plots and box plots. Assess their significance.
- Analyze the balance of positive and negative data in the dataset.

### 2. Random Forest Classification

#### (c) Initial Model Training

- Train a random forest without compensating for class imbalance.
- Evaluate the model using metrics like confusion matrix, ROC, AUC, and misclassification rates for both training and test sets. Calculate the Out of Bag error.

#### (d) Addressing Class Imbalance

- Research and apply methods to address class imbalance in random forests.
- Re-train and evaluate the model, comparing results with the initial training.

### 3. XGBoost and Model Trees

#### (e) XGBoost Training

- Implement XGBoost with L1-penalized logistic regression at each decision node.
- Determine the regularization term (α) using cross-validation.
- Estimate error using cross-validation methods (5-fold, 10-fold, leave-one-out) and compare with test error.
- Report metrics like Confusion Matrix, ROC, and AUC for both training and test sets.

#### (f) SMOTE Application

- Pre-process data using SMOTE to address class imbalance.
- Train the XGBoost model on the pre-processed data.
- Compare results of the uncompensated case with the SMOTE case.

## Objectives

- Explore tree-based methods in machine learning for APS Failure data analysis.
- Develop models capable of handling class imbalance and missing data effectively.
- Compare the effectiveness of random forests and XGBoost in this context.

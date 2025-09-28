# Breast-Cancer-Prediction-Using-Classificarion
Breast Cancer Classification using Logistic Regression on the Wisconsin dataset. Includes EDA, preprocessing, model training, evaluation (confusion matrix, ROC, PR curves), and feature importance. Achieves high accuracy and recall, making it useful for early cancer detection analysis.

📌 Project Overview

This project applies Logistic Regression to the Breast Cancer Wisconsin Dataset to predict whether a tumor is benign (0) or malignant (1).

The notebook includes:

🔎 Exploratory Data Analysis (EDA)

⚙️ Preprocessing (scaling, encoding, train-test split)

🤖 Logistic Regression Model Training

📊 Evaluation Metrics & Visualizations

🧠 Feature Importance Analysis

🔮 Predictive System for New Patient Data

🎯 Objectives

Understand the dataset through EDA.

Build a predictive model using Logistic Regression.

Evaluate performance with accuracy, precision, recall, F1, and ROC-AUC.

Interpret which features contribute most to classification.

Develop a predictive system to classify new patient records.

📊 Dataset

Dataset: Breast Cancer Wisconsin Dataset

Features: 30 numeric features describing tumor characteristics.

Target:

0 → Benign

1 → Malignant

🔎 Exploratory Data Analysis (EDA)

Key insights:

There is no missing  values in the dataset

Dataset is balanced (more benign cases, but malignant also well represented).

Features such as radius_worst, texture_worst, and concavity_mean are strong predictors.

High correlation exists among features like radius, area, and perimeter.

Visualizations used:

Class distribution plot

Histograms & boxplots

Scatter plots between important features

Correlation heatmap

⚙️ Methodology

Data Preprocessing

Encoded target (M=1, B=0)

Standardized features with StandardScaler

Train-test split (80%-20%)

Model Training

Logistic Regression with class_weight='balanced' to handle slight imbalance

Evaluation Metrics

Accuracy

Precision

Recall (prioritized for medical diagnosis)

F1 Score

ROC-AUC

Visualizations

Confusion Matrix

ROC Curve

Precision-Recall Curve

Feature Importance (odds ratios)

📈 Results

Logistic Regression achieved high accuracy (>90%).

ROC-AUC curve showed excellent separation of classes.

Recall was strong, which is critical in cancer detection (avoiding false negatives).

Key influential features:

texture_worst

radius_worst

concavity_mean

🔮 Predictive System

This project also includes a predictive system that allows you to input new patient data (30 tumor features) and get a prediction of whether the tumor is Benign (0) or Malignant (1).

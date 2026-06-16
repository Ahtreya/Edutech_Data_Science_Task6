# Edutech_Data_Science_Task6
## K-Nearest Neighbors (KNN) Classifier on Iris Dataset

## Project Overview
This repository contains the complete implementation for Task 6 of the Edutech Solution Data Science Internship. The objective of this project is to build an optimised K-Nearest Neighbors (KNN) classification model using Scikit-Learn to identify flower species from the Iris dataset accurately.

### 🛠️ Workflow Steps Covered
1. **Data Preprocessing**: Loaded raw `Iris.csv`, removed the unnecessary `Id` column, and separated features from target variables.
2. **Data Splitting**: Divided the dataset into training (80%) and testing (20%) sets.
3. **Feature Scaling**: Implemented `StandardScaler` on the training features and applied the ruleset to the test data to prevent data leakage.
4. **Hyperparameter Tuning**: Utilised `GridSearchCV` with 5-fold cross-validation to automatically determine the absolute best mathematical value for K.
5. **Model Training**: Trained the final KNN classifier using the optimal K parameter.
6. **Evaluation Metrics**: Generated full performance profiles using global accuracy scores and multi-class classification reports.
7. **Model Saving**: Exported the final trained model into a production-ready `.joblib` file format.

### 💬 Interview Questions Answers

#### Q1: What is KNN?
- KNN stands for K-Nearest Neighbours. It is a supervised, non-parametric, and distance-based machine learning algorithm used for both classification and regression tasks. It functions on the core principle that similar data points exist in proximity within a multi-dimensional feature space.

#### Q2: How to choose the value of K?
- **Square Root Heuristic**: Setting $K = \sqrt{N}$ where $N$ is the sample size.
- **Odd Number Rule**: Choosing an odd number prevents tie votes when working with multi-class targets.
- **Elbow Method**: Plotting error rates across a spectrum of values to look for stabilising points.
- **Cross-Validation (Best Practice)**: Utilising tools like `GridSearchCV` to automatically measure and select the parameter setting that maximises validation accuracy.

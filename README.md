# Heart Disease Prediction Using k-NN  

## Overview  
This project aims to predict heart disease presence using a **k-Nearest Neighbors (k-NN) model**. It involves **data preprocessing, feature selection, hyperparameter tuning, and evaluation** to optimize predictive performance.  

## How to Run  
- Open the latest version of the project in **NBViewer**:  
  [View in NBViewer](https://nbviewer.org/github/dimitar-m/predicting-heart-disease/blob/master/predicting-heart-disease-v1.3.ipynb)  

## Dataset  
The dataset consists of patient records, including medical attributes such as **cholesterol, blood pressure, and exercise-induced angina**. The target variable indicates the presence of heart disease.  

## Methods & Techniques  
- **Exploratory Data Analysis (EDA)**: Examined distributions, correlations, and potential data issues.  
- **Data Cleaning & Preprocessing**:  
  - Replaced incorrect cholesterol values using the **mean**.  
  - Handled outliers in RestingBP and Oldpeak.  
  - Scaled numerical features using **MinMaxScaler**.  
- **Feature Selection**: Selected features with correlation > 0.1 to improve model performance.  
- **Model Optimization**:  
  - Tried **multiple train-test splits** (90/10, 80/20, 70/30).  
  - Compared **GridSearchCV vs. RandomizedSearchCV**.  
  - Tested different distance metrics (**Euclidean, Manhattan, Minkowski, Hamming**).  
- **Final Model Performance**:  
  - Best model: **k-NN (15 neighbors, Hamming distance, uniform weights)**  
  - **Train Accuracy:** 86.60%  
  - **Test Accuracy:** **88.77%**  

## Key Findings  
- Feature selection improved accuracy compared to using all features.  
- **Hamming distance** worked best for k-NN in this dataset.  
- **Hyperparameter tuning** significantly improved model performance.  

## Future Work  
- Test additional classifiers (e.g., **Random Forest, SVM, Neural Networks**).  
- Use **ensemble learning** to combine multiple models for better accuracy.  
- Experiment with **feature engineering** to create new informative variables.  

---

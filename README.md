# Project Title
Income Classification using Machine Learning (UCI Adult Dataset)
## Overview
The goal of the project is to predict whether a person's income is greater than or less than $50K based on demographic and employment data.
## Objective
To build and evaluate binary classification models using Logistic Regression, Random Forest, Decision Tree, and K-Nearest Neighbors.
## Dataset
-**Source**:UCI Machine Learning Repository-Adult Dataset(https://archive.ics.uci.edu/dataset/2/adult) 
 -Rows:48842 
 -columns:14+ target variable
## Tools & Libraries
- Python,NumPy,Pandas
- Matplotlib,Seaborn (for visualization)
- Scikit-learn (for model training and evaluation)
## Project Steps
### 1. Data Collection
 - Loaded the dataset from UCI repository
### 2. Data Cleaning
 - Handled missing values using forward fill method.
 - Dropped the columns :'fnlwgt','realtionship','native-country'.
### 3. Exploratory Data Analysis (EDA)
 - Used 'describe()' to understand basic statistics (e.g., mean age is 38.6)
 - plotted :
    - countplot of Income Distribution
    - Histogram of Age Distribution
    - Heatmap of Confusion matrix
### 4. Label Encoding
 - Converted categorical variable into numeric from using 'LabelEncoder'.
### 5.Feature Selection and Splitting
 - selected input features (x) and target variable (y='Income')
 - Performed train-test split (80/20) with 'stratify='y' to maintain class distribution.
### 6. Feature Scaling
 - Applied 'StandardScaler' to normalize numerical features for KNN and Logistic Regression.
### 7. Model Training
 - Logistic Regression
 - Random Forest
 - Decision Tree
 - K-Nearest Neighbors
### 8. Model Evaluation
 - Used Confusion Matrix Classification Report
 - Evaluated using:
    - Accuracy
    - Precision
    - Recall
    - F1 Score (Macro and Weighted)
### 9. Result Summary
| Model               | Accuracy | Weighted F1 Score |
|----------------------------------------------------|
| Logistic Regression | 0.85     | 0.84              |
| Random Forest       | 0.85     | 0.85              |
| Decision Tree       | 0.85     | 0.83              |
| K-Nearest Neighbors | 0.82     | 0.82              |
### 10. Insights
 - Most people earn <=50K.
 - Marital status and education are strong predictors.
 - Random Forest performed best.
## Conclusion
This project helped to develop a strong understanding of classification algorithms, preprocessing techniques, and model evaluation.
## Author
Silpa E S

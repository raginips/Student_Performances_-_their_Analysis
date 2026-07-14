# Student_Performances_-_their_Analysis
## Repository Description
A machine learning project that predicts student academic performance using demographic and educational attributes. It compares multiple regression models—Linear Regression, Decision Tree, and Random Forest—to determine the most effective algorithm.
------------------------------
## README.md## Student Performance Prediction
This repository contains a comprehensive data science project aimed at predicting student academic performance based on demographic data and educational backgrounds. The project covers data preprocessing, exploratory data analysis (EDA), feature engineering, and the training and evaluation of multiple machine learning regression models to find the most accurate predictor.
## Project Objectives

* Preprocess and clean student performance data.
* Conduct exploratory data analysis to identify trends and key features.
* Encode and scale data for machine learning algorithms.
* Train and evaluate multiple regression models.
* Identify the key factors that significantly affect student scores.

## Dataset Overview
The dataset contains 1,000 student records with 8 distinct features:

* Categorical Features: Gender, Race/Ethnicity, Parental Level of Education, Lunch Type, Test Preparation Course
* Numerical Features: Math Score, Reading Score, Writing Score

## Project Workflow## 1. Data Preprocessing & Cleaning

* Checked for missing and duplicate records.
* Engineered an Average_score feature combining all three subject marks.
* Created a binary Passed classification indicator for students scoring an average of 60 or above.

## 2. Feature Engineering & Encoding

* Label Encoding: Applied to binary categorical variables like Gender, Lunch, and Test Preparation Course.
* One-Hot Encoding: Applied to multi-class variables such as Race/Ethnicity.
* Ordinal Encoding: Applied to Parental Level of Education to preserve the hierarchical nature of degrees.
* Feature Scaling: Applied StandardScaler to normalize numerical subject scores.

## 3. Exploratory Data Analysis (EDA)

* Analyzed the impact of demographic features on average marks.
* Evaluated score distributions using histograms and pair plots.
* Generated a correlation heatmap to analyze relationships between features and academic outcomes.

## 4. Model Training & Selection
Three main regression algorithms were implemented to predict student scores:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor

## Model Evaluation Results
The models were evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² Score.

| Model | MAE | MSE | RMSE | R² Score |
|---|---|---|---|---|
| Linear Regression | 0.273 | 0.124 | 0.352 | 0.883 |
| Random Forest | 0.307 | 0.157 | 0.396 | 0.852 |
| Decision Tree | 0.416 | 0.298 | 0.546 | 0.719 |

## Key Insights

* Top Performer: Linear Regression delivered the highest prediction accuracy with an R² Score of 0.883.
* Cross-Validation: The Linear Regression model achieved a robust 5-fold cross-validation score of approximately 0.873.
* Feature Importance: Feature analysis indicates that a student's passing status along with reading and writing proficiencies are the strongest indicators of overall performance.

## Technologies Used

* Python
* NumPy & Pandas (Data Manipulation)
* Matplotlib & Seaborn (Data Visualization)
* Scikit-Learn (Machine Learning & Evaluation)

------------------------------
Would you like me to add a specific installation or usage guide section to the README based on how you plan to deploy or run your script?



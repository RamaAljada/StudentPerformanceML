# Student Performance Prediction
Predicting student **Performance Index** using **Linear Regression** based on study habits, previous academic performance, sleep hours, and extracurricular activities.

## Overview
- **Problem Type**: Regression  
- **Dataset**: 10,000 records, 6 features  
- **Target**: Performance Index (continuous score)  
- **Main Goal**: Build an accurate and interpretable model to predict student performance

## Dataset Description
| Column                              | Description                                      | Type    |
|-------------------------------------|--------------------------------------------------|---------|
| Hours Studied                       | Number of hours spent studying                   | int     |
| Previous Scores                     | Score in previous tests/exams                    | int     |
| Extracurricular Activities          | Yes / No                                         | binary  |
| Sleep Hours                         | Average hours of sleep per day                   | int     |
| Sample Question Papers Practiced    | Number of practice question papers solved        | int     |
| **Performance Index**               | **Target variable** (student performance score)  | float   |

## Project Workflow
1. Import libraries (pandas, numpy, matplotlib, seaborn, scikit-learn)  
2. Load and explore the dataset  
3. Handle missing values & data cleaning  
4. Encode categorical variable (Yes → 1, No → 0)  
5. Feature scaling using `StandardScaler`  
6. Exploratory Data Analysis (EDA):  
   - Boxplots to detect outliers  
   - Correlation matrix & feature importance  
7. Train/test split  
8. Train baseline **Linear Regression** model  
9. Hyperparameter tuning with **GridSearchCV**  
10. Model evaluation using **MAE**  
11. Interpret results & feature importance

## Key Results
- **Best Model**: Linear Regression  
- **Mean Absolute Error (MAE)**: **1.611** (very low error → strong predictive power)  
- **Most Important Feature**: Previous Scores (correlation = **0.915**)  
- Other features show much weaker correlation  
- No significant outliers detected in boxplots

## Project Strengths
- Clean, well-prepared dataset  
- Proper encoding and scaling  
- Hyperparameter tuning performed  
- Clear visualizations (boxplots, correlation analysis)  
- Strong interpretability of results

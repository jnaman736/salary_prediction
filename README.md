# Salary Prediction Analysis

This project aims to predict individual salaries based on demographic and professional attributes using machine learning regression techniques. By analyzing a dataset of over 6,700 professionals, we identify the key factors that influence compensation and compare the effectiveness of different predictive models.

## Dataset Overview
The dataset consists of 6,704 entries with the following features:
* Age: Age of the individual.
* Gender: Male, Female, or Other.
* Education Level: Categorized into High School, Bachelor's, Master's, and PhD.
* Job Title: Various professional roles across industries.
* Years of Experience: Total professional tenure.
* Salary: The target variable for prediction.

## Key Features
* Data Cleaning: Robust handling of missing values and data standardization.
* Exploratory Data Analysis (EDA): 
    * Visualizing top 10 highest-earning professions.
    * Analyzing the correlation between age, experience, and salary.
    * Distribution analysis of education levels and gender.
* Machine Learning: Implementation of multiple regression models with hyperparameter tuning via GridSearchCV.

## Model Performance
We evaluated three primary models to determine the most accurate predictor. The Random Forest Regressor significantly outperformed the others:

| Model | R-Squared (R2) | Performance Summary |
| :--- | :--- | :--- |
| **Random Forest** | **0.971** | **Best Accuracy**: Lowest error rates across MSE, MAE, and RMSE. |
| **Decision Tree** | 0.941 | Strong performance but slightly less precise than Random Forest. |
| **Linear Regression** | 0.833 | Good baseline, but struggles with non-linear patterns. |

## Installation and Setup
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/salary-prediction.git](https://github.com/your-username/salary-prediction.git)
   cd salary-prediction
2. **Run the Analysis:** Open the Jupyter Notebook for a step-by-step walkthrough:
   ```bash
   jupyter notebook "Salary Prediction.ipynb"

## Conclusion

The analysis reveals that **Years of Experience** and **Age** are the most influential factors in salary determination.  
The **Random Forest** model is the recommended choice for production use due to its high predictive accuracy (**R² = 0.971**).

This tool can be effectively utilized:
- By **HR departments** for salary benchmarking  
- By **individuals** for career planning and growth analysis  

## Requirements

- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  


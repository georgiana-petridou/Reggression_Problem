# Reggression_Problem
# Diabetes Progression Prediction using Regression Analysis

## Project Overview
This project aims to predict the quantitative measure of **diabetes progression** one year after baseline, based on ten physiological variables (age, sex, BMI, blood pressure, and six blood serum measurements). The project explores various **Regression** techniques to identify the most accurate predictive model for clinical data analysis.

## Key Methodology
* **Exploratory Data Analysis (EDA)**: Performed correlation analysis using Heatmaps to identify the strongest predictors of disease progression (e.g., BMI and S5) and visualized feature distributions.
* **Data Preprocessing**: 
    * Implemented **Standardization (Z-score scaling)** to ensure all features contribute equally to the model, which is critical for regularized algorithms.
    * Handled categorical variables and checked for multi-collinearity among blood serum features.
* **Model Selection & Tuning**: Utilized **Train-Test Splitting** and **Cross-Validation** to ensure the models generalize well to unseen patient data.
* **Regularization**: Applied $L_1$ and $L_2$ regularization techniques to prevent overfitting and perform automated feature selection.

## Models Evaluated
Six different regression algorithms were implemented and compared:
* **Multiple Linear Regression (OLS)**: Established as the baseline model.
* **Ridge Regression ($L_2$)**: Used to manage multi-collinearity issues.
* **Lasso Regression ($L_1$)**: Employed for feature selection by shrinking less important coefficients to zero.
* **ElasticNet**: A hybrid approach combining both $L_1$ and $L_2$ penalties.
* **Polynomial Regression**: Tested to capture potential non-linear relationships.
* **Stochastic Gradient Descent (SGD) Regressor**: Evaluated for optimization efficiency.

## Performance Metrics
The models were evaluated using the following metrics:
* **R-squared ($R^2$)**: To measure the proportion of variance explained by the model.
* **Mean Squared Error (MSE) / RMSE**: To quantify the average squared difference between estimates and actual outcomes.
* **Mean Absolute Error (MAE)**: To assess the average magnitude of errors in predictions.

## Tech Stack
* **Language**: Python 3.x
* **Libraries**: Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
* **Environment**: Google Colab / Jupyter Notebook

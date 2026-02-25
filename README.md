# Insurance-Regression-Analysis
# Medical Insurance Cost Analysis

This repository contains a Python project designed to analyze and predict healthcare costs. By utilizing a dataset of medical insurance records, the project explores how factors like age, BMI, and lifestyle choices influence annual charges.

## Project Structure
The analysis follows a logical flow to ensure data integrity and model accuracy:
1. **Data Inspection:** Reviewing data types and identifying the target variable.
2. **EDA:** Using statistical plots to find hidden patterns in health data.
3. **Data Cleaning:** Identifying and removing outliers via the Interquartile Range (IQR) method.
4. **Feature Normalization:** Applying Z-score scaling to ensure consistent feature ranges.
5. **Linear Regression:** Implementing the model both manually and through Scikit-Learn for verification.

## Methodology
The core of this project is the manual verification of the regression slope. We calculated the parameters using the following formulas:



- **Weight (Slope):** The ratio of the covariance of X and Y to the variance of X.
- **Bias (Intercept):** The difference between the mean of Y and the product of the slope and the mean of X.

## Results and Findings
The project highlights that lifestyle factors, particularly smoking status, are the strongest predictors of high medical costs. While the R-squared value is higher when including outliers, the Root Mean Squared Error (RMSE) improves significantly when extreme BMI values are removed, leading to a more stable prediction for the general population.

## Installation
To run this project, you will need:
- Python 3.x
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-Learn

Usage:
1. Place `insurance.csv` in the root directory.
2. Run `python insurance_analysis.py`.

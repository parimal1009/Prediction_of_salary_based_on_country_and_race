Prediction of salary based on country and race
Overview

This project aims to predict the salary of individuals from various countries and races based on demographic factors such as age, gender, education, occupation, and years of experience. The dataset used for this project contains salary and demographic information of employees, allowing us to explore the relationship between income and socio-demographic factors, including race, country, and years of experience. The dataset, sourced from Kaggle, has 32,561 rows and 15 columns, with 8 independent variables and 1 target variable, which is the salary.
Dataset Description

The dataset provides a comprehensive collection of salary and demographic information with attributes including:

    Age: Age of the employee
    Education Level: Education level of the employee
    Job Title: Job title of the employee
    Years of Experience: Total experience in the respective field
    Salary: Target variable (dependent) - the employee's salary
    Country: Country of the employee
    Race: Racial background of the employee

This dataset offers rich insights for analyzing salary disparities based on demographic factors and the effect of experience on income.
Data Preprocessing

Several preprocessing steps were applied to prepare the data for modeling:

    Grouping Job Titles: Simplified job titles into broader categories.
    Grouping Education Levels: Grouped education levels into higher-level categories.
    Label Encoding: Categorical variables such as Gender, Country, and Race were label-encoded.
    Normalization: Features were scaled to ensure proper fit for machine learning models.

Exploratory Data Analysis (EDA)

In the EDA, we analyzed the distribution and relationship of different variables with salary:

    Gender Distribution: The dataset includes 54.8% males, 45% females, and 0.2% other gender categories.
    Age Distribution: Most employees fall within the age group of 25-35, and salaries generally increase with age.
    Education Level: Employees with PhDs earn the highest median salary, followed by Master's and Bachelor's degree holders.
    Job Title: Software Developers, Data Analysts/Scientists, and Managerial roles tend to have higher demand and salary.
    Experience and Salary: Salary increases with experience, but other factors like job title, education, and gender also influence salary.
    Country and Race: Median salaries vary slightly between countries, with race also showing distinct salary patterns.

Correlation Analysis

We identified key correlations through a heatmap:

    Salary and Age
    Salary and Years of Experience
    Years of Experience and Age

Model Selection

For predicting salaries, two models were used:

    Decision Tree Regressor
    Random Forest Regressor

Model Evaluation

    Decision Tree Regressor: Initially trained with hyperparameter tuning. The predicted salary values were close to actual values, showing a good fit.
    Random Forest Regressor: Performed better than the Decision Tree with a higher accuracy of 94.6%.

Key Evaluation Metrics

    R² Score: Measures how well the predicted values match the actual salary values. A higher R² score indicates better predictive accuracy.

    Mean Squared Error (MSE): Measures the average squared difference between predicted and actual values. Lower MSE indicates better model performance.

    Mean Absolute Error (MAE): Represents the average of the absolute differences between predicted and actual values. It provides an intuitive measure of the model’s prediction error.

    Root Mean Squared Error (RMSE): This is the square root of the MSE and gives an estimate of the error in the same units as the target variable (salary). Lower RMSE indicates better fit.



Results and Conclusion

From the analysis, it’s clear that salary is strongly influenced by:

    Years of Experience: Employees with more experience generally earn higher salaries.
    Job Title: Roles such as Software Developer, Data Scientist, and Manager/Director tend to offer higher salaries.
    Education Level: Higher education levels (Master’s and PhD) correspond with higher salaries.

The Random Forest Regressor model performed the best, achieving an accuracy of 94.6%.
Future Work

    Including more detailed job-specific features and location-based cost of living adjustments.
    Experimenting with other regression models like XGBoost and Gradient Boosting Regressors for potentially better performance.


# Medical Cost Prediction

This repository contains an analysis and regression modeling project aimed at predicting medical costs based on various predictors such as age, BMI, smoking status, and more.

## Introduction
The goal of this project is to predict medical costs using various features. The analysis involves:
- Data exploration
- Correlation analysis
- Regression modeling
- Model evaluation

## Dataset
The dataset used in this project includes the following columns:
- age: Age of the individual
- sex: Gender of the individual
- bmi: Body Mass Index
- children: Number of children
- smoker: Smoking status (Yes/No)
- region: Geographic region
- medicalCost: Medical costs incurred

## Data Cleaning
Data cleaning steps included handling missing values, encoding categorical variables, and normalizing numerical variables.

## Exploratory Data Analysis
Exploratory data analysis (EDA) steps included:
1. Visualizing the distribution of ages
2. Counting males and females
3. Analyzing the distribution of BMI and identifying outliers
4. Counting the number of children

## Correlation Analysis
Correlation analysis was performed to identify the relationship between predictors and the target variable `medicalCost`. The strongest positive correlation was observed with the `smoker` variable.

## Regression Modeling
### Simple Linear Regression
Simple linear regression models were built using individual predictors:
- Smoker
- Age
- BMI

### Multiple Linear Regression
Two multiple regression models were built:
1. Using the three best predictors (smoker, age, bmi)
2. Using all predictors (age, sex, bmi, children, smoker, region)

## Model Evaluation
The models were evaluated using statistical performance measures such as R-squared, F-statistic, and p-values.

## Conclusion
- The `smoker` variable had a strong positive correlation with `medicalCost`.
- Models with more predictors generally performed better.
- The final choice of the model depends on the specific context and the trade-off between model complexity and predictive accuracy.

## How to Run
To run the analysis, follow these steps:
1. Clone this repository: `git clone https://github.com/yourusername/MedicalCostPrediction.git`
2. Navigate to the project directory: `cd MedicalCostPrediction`
3. Install the required packages: `pip install -r requirements.txt`
4. Run the analysis: `python main.py`

## References
- The dataset used in this project can be found in this repository.
- The analysis was conducted using Python with libraries such as pandas, seaborn, and statsmodels.

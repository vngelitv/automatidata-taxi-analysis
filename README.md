# Automatidata Taxi Data Analysis

## Project Overview

This educational project explores 2017 New York City taxi trip data using Python and pandas. The analysis was completed as part of the Google Advanced Data Analytics Professional Certificate on Coursera.

## Objective

The objective was to inspect the dataset, understand important variables, identify unusual values, and prepare the data for future predictive modeling.

## Dataset

The sample contains 22,699 taxi trip records and 18 variables, including:

- Trip distance
- Total trip amount
- Payment type
- Tip amount
- Passenger count
- Vendor ID

## Tools and Skills

- Python
- pandas
- Jupyter Notebook
- Exploratory data analysis
- Descriptive statistics
- Data filtering
- Grouping and aggregation
- Outlier identification
- NumPy
- Matplotlib
- Seaborn
- Tableau Public
- Data visualization
- Datetime feature engineering

## Key Findings

- Credit card was the most common recorded payment method.
- The average recorded credit-card tip was approximately $2.73.
- Cash tips were recorded as $0 because cash tips are not captured in the dataset.
- The two vendors had nearly identical average total trip amounts.
- Some total amounts were negative or unusually high and should be investigated before predictive modeling.
- Trip distance and total amount appear related, although tolls, tips, taxes, and surcharges also affect the final cost.

## Note

This is an educational project based on course materials from the Google Advanced Data Analytics Professional Certificate.

## Project Progression

### Course 1: Data Inspection and Organization

- Imported the NYC taxi dataset into pandas
- Reviewed column data types and missing values
- Calculated descriptive statistics
- Investigated payment types, vendors, fares, and tips
- Identified unusual and potentially invalid values

### Course 2: Exploratory Data Analysis and Visualization

- Converted pickup and drop-off columns to datetime
- Examined outliers in trip distance, total amount, and tip amount
- Analyzed taxi demand by month and day of the week
- Compared revenue by month and weekday
- Evaluated average tips by passenger count and vendor
- Examined mean trip distance by drop-off location
- Created a Tableau scatterplot of trip distance and total amount

## Key Course 2 Findings

- Most taxi trips were short, while a smaller number were unusually long.
- Trip distance, total fare, and tip amount were strongly right-skewed.
- Total amount included negative values and an extreme value above $1,200.
- March had the highest number of sampled rides.
- Thursday generated the highest total revenue in the sample.
- Trip distance was positively associated with total fare.
- Some trips had zero recorded distance but positive fares and should be investigated before modeling.

### Course 3: Statistical Analysis and A/B Testing

- Compared average taxi fare amounts by payment type
- Used descriptive statistics to examine credit card and cash payments
- Formulated null and alternative hypotheses
- Conducted a two sample t-test
- Used a 5% significance level
- Found a statistically significant difference in average fare amounts
- Interpreted results in the context of revenue and experimental assumptions

## Key Course 3 Finding

Credit card customers had a higher average fare amount than cash customers, and the difference was statistically significant (`p ≈ 6.80 × 10⁻¹²`).

Because this educational exercise assumes random assignment of payment type, the result can be interpreted causally within the scenario. In real-world taxi data, customers choose their payment method, so other factors could also explain the difference.

### Course 4: Multiple Linear Regression

- Performed additional EDA and prepared data for regression modeling
- Converted datetime variables and created trip-duration features
- Identified and handled outliers in trip distance, fare amount, and duration
- Engineered mean distance and mean duration features
- Created rush-hour and time-based variables
- Examined correlations between predictors and fare amount
- Built a multiple linear regression model
- Split data into training and testing sets
- Standardized predictor variables
- Evaluated model performance using R², MAE, MSE, and RMSE
- Analyzed residuals and regression coefficients

## Key Course 4 Findings

Mean trip distance and mean trip duration were among the strongest predictors of taxi fare amount.

The model achieved an R² of approximately `0.84` on the training data, meaning it explained about 84% of the variation in fare amount.

Residual analysis and coefficient interpretation were used to evaluate model performance and understand the influence of each predictor.

### Course 5: Machine Learning

- Evaluated ethical considerations surrounding predictive modeling
- Reframed the business objective to predict generous tippers
- Engineered the `tip_percent` and `generous` target variables
- Created day, month, and time-of-day features
- Prepared categorical variables through dummy encoding
- Built and tuned Random Forest and XGBoost classification models
- Used GridSearchCV and cross-validation for hyperparameter tuning
- Evaluated models using precision, recall, F1 score, and accuracy
- Compared model performance on held-out test data
- Selected Random Forest as the champion model
- Analyzed confusion-matrix errors and feature importance

## Key Course 5 Findings

The target variable was nearly balanced, with approximately 52.6% of customers classified as generous tippers.

Random Forest achieved the strongest test performance, with an F1 score of approximately `0.723`, compared with approximately `0.710` for XGBoost.

The Random Forest model was selected as the champion model. False positives were more common than false negatives, meaning the model more often predicted a generous tip when the actual tip was below the 20% threshold.

## Project Files

- `automatidata_taxi_analysis.ipynb` — Course 1 inspection notebook
- `course-2-eda/automatidata_course2_eda.ipynb` — Course 2 EDA notebook
- `course-2-eda/tableau_scatterplot.png` — Tableau visualization
- `course-3-statistics/automatidata_course3_statistics.ipynb` — statistical analysis and hypothesis testing notebook
- `course-3-statistics/README.md` — Course 3 project summary
- `course-4-regression/automatidata_course4_regression.ipynb` — multiple linear regression notebook
- `course-4-regression/README.md` — Course 4 project summary
- `course-5-machine-learning/automatidata_course5_machine_learning.ipynb` — Random Forest and XGBoost classification notebook
- `course-5-machine-learning/README.md` — Course 5 project summary

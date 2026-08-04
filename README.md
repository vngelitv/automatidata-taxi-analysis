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

## Project Files

- `automatidata_taxi_analysis.ipynb` — Course 1 inspection notebook
- `course-2-eda/automatidata_course2_eda.ipynb` — Course 2 EDA notebook
- `course-2-eda/tableau_scatterplot.png` — Tableau visualization

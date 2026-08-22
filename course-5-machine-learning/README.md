# Course 5 – Machine Learning

This folder contains the machine learning phase of the Automatidata NYC Taxi project completed as part of the Google Advanced Data Analytics Professional Certificate.

## Objective

The objective of this phase was to build and compare tree-based classification models to predict whether a taxi customer would be a generous tipper, defined as tipping at least 20%.

The original business request involved predicting customers who would not tip. Because that could create fairness and accessibility concerns, the modeling objective was reframed to identify especially generous tippers instead.

## Work Completed

- Considered ethical implications of the original modeling request
- Reframed the target to predict generous tippers
- Combined taxi data with engineered features from earlier project stages
- Filtered the dataset to credit-card transactions
- Engineered a `tip_percent` variable
- Created the binary target variable `generous`
- Engineered day, month, and time-of-day features
- Removed variables unavailable at prediction time
- Dummy encoded categorical variables
- Evaluated target class balance
- Split data into training and testing sets
- Built and tuned a Random Forest classifier
- Used GridSearchCV and cross-validation
- Built and tuned an XGBoost classifier
- Compared precision, recall, F1 score, and accuracy
- Selected the Random Forest model as the stronger model
- Evaluated the champion model with a confusion matrix
- Examined feature importance

## Key Findings

- The target classes were nearly balanced, with about 52.6% of customers classified as generous tippers.
- F1 score was selected as the primary evaluation metric because precision and recall were both important.
- The Random Forest model achieved an F1 score of approximately 0.72 on the test data.
- The XGBoost model performed slightly worse on F1 score.
- Random Forest was selected as the champion model.
- False positives occurred more often than false negatives, meaning the model was more likely to predict a generous tip when the actual tip was below the threshold.

## Tools & Skills

- Python
- pandas
- NumPy
- scikit-learn
- XGBoost
- Random Forest
- GridSearchCV
- Cross-validation
- Feature engineering
- Classification
- Hyperparameter tuning
- Precision
- Recall
- F1 score
- Confusion matrices
- Feature importance
- Model evaluation

## Files

- `automatidata_course5_machine_learning.ipynb` — completed Course 5 machine learning notebook

## Note

This is an educational project using synthetic/sample data as part of the Google Advanced Data Analytics Professional Certificate.

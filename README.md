Titanic Data Analysis – Project Summary

This project performs a complete preprocessing and analysis pipeline on the Titanic dataset to prepare it for machine learning tasks. The focus is on data cleaning, transformation, visualization, and outlier handling.

Steps Performed:

Data Loading & Exploration

Loaded the Titanic dataset using Pandas.

Explored data structure, types, and identified missing values.

Missing Value Treatment

Filled missing Age with median value.

Filled missing Embarked with mode.

Filled missing Fare (if any) with median.

Feature Cleaning

Dropped irrelevant columns: PassengerId, Name, Ticket, and Cabin (due to high nulls).

Categorical Encoding

Converted Sex to numeric (male=0, female=1).

Applied one-hot encoding to Embarked → Created Embarked_C, Embarked_Q, Embarked_S.

Feature Scaling

Applied standardization (Z-score) to Age and Fare using StandardScaler for uniform scale.

Outlier Detection & Removal

Visualized boxplots for Age and Fare (after scaling).

Detected outliers using IQR method and removed extreme values beyond the whiskers.

Visualization

Used boxplots for outlier detection.

Used histograms and bar charts (with original data) for age and fare distributions.



Key Techniques Used:
Handling missing data with median/mode imputation.

One-hot encoding for nominal categorical variables.

Standardization to improve model performance.

Boxplot + IQR for identifying and removing outliers.

Visualization using Seaborn and Matplotlib.

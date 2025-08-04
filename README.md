<h1> Titanic Data Analysis – Project Summary </h1>

This project performs a complete preprocessing and analysis pipeline on the Titanic dataset to prepare it for machine learning tasks. The focus is on data cleaning, transformation, visualization, and outlier handling.

<h3> Steps Performed: </h3>

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

<img width="623" height="404" alt="image" src="https://github.com/user-attachments/assets/118a2fe1-9060-4489-9561-d771324d88f3" />

<img width="604" height="386" alt="image" src="https://github.com/user-attachments/assets/fdbd0b8c-162c-47e3-9a81-d40298ad8124" />


<img width="998" height="708" alt="image" src="https://github.com/user-attachments/assets/c70f6c08-9847-44f7-88e5-6c3701620bbc" />

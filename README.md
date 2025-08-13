#  Titanic Data Analysis – Project Summary

This project implements a complete **data preprocessing and exploratory analysis pipeline** on the Titanic dataset to prepare it for machine learning.  
The workflow focuses on **data cleaning, transformation, visualization, and outlier handling**.

---

##  Steps Performed

### 1. **Data Loading & Exploration**
- Loaded the Titanic dataset using **Pandas**.
- Inspected dataset structure, data types, and identified missing values.

### 2. **Missing Value Treatment**
- Filled missing **Age** with **median** value.
- Filled missing **Embarked** with **mode**.
- Filled missing **Fare** (if any) with **median**.

### 3. **Feature Cleaning**
- Dropped irrelevant columns:
  - `PassengerId`
  - `Name`
  - `Ticket`
  - `Cabin` (due to high null percentage)

### 4. **Categorical Encoding**
- Converted `Sex` to numeric (`male`=0, `female`=1).
- Applied **one-hot encoding** to `Embarked`, creating:
  - `Embarked_C`
  - `Embarked_Q`
  - `Embarked_S`

### 5. **Feature Scaling**
- Standardized numerical features (`Age`, `Fare`) using **Z-score Standardization** (`StandardScaler`).

### 6. **Outlier Detection & Removal**
- Visualized **boxplots** for `Age` and `Fare` after scaling.
- Used **IQR method** to detect and remove extreme outliers.

### 7. **Visualization**
- Boxplots for outlier detection.
- Histograms and bar charts (using original values) for age and fare distributions.

  
<img width="623" height="404" alt="image" src="https://github.com/user-attachments/assets/118a2fe1-9060-4489-9561-d771324d88f3" />

<img width="604" height="386" alt="image" src="https://github.com/user-attachments/assets/fdbd0b8c-162c-47e3-9a81-d40298ad8124" />
---

##  **Key Techniques Used**
- **Median/Mode Imputation** for missing data.
- **One-Hot Encoding** for nominal categorical variables.
- **Standardization** for uniform feature scaling.
- **Boxplot + IQR** for detecting and removing outliers.
- **Seaborn** & **Matplotlib** for visualizations.

---

##  **Key Insights**
- Female passengers had a much higher survival rate than males.
- First-class passengers had the highest survival rate.
- Higher fares were strongly associated with survival.
- Children showed better survival chances than adults.



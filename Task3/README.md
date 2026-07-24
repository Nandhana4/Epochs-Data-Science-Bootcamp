# Used Car Price Prediction - Assignment 3

## Dataset Overview

This project focuses on performing Exploratory Data Analysis (EDA), Data Cleaning, and Feature Engineering on the **Used Car Price Prediction Dataset**. The dataset contains information about used cars, including their brand, model, manufacturing year, mileage, fuel type, engine specifications, transmission, exterior and interior colors, accident history, clean title status, and selling price.

The dataset consists of **4,009 records** and **12 features**.

---

## Data Quality Issues Identified

The following data quality issues were identified during the analysis:

- Missing values were found in the following columns:
  - `fuel_type`
  - `accident`
  - `clean_title`
- No duplicate records were found after checking the dataset.
- The `milage` column was stored as text with commas and the suffix `"mi."`.
- The `price` column was stored as text with the `$` symbol and commas.
- Most columns were categorical, requiring preprocessing before machine learning.

---

## Data Cleaning Techniques Applied

The following cleaning steps were performed:

- Removed duplicate records.
- Filled missing values in:
  - `fuel_type` using the mode.
  - `accident` using the mode.
  - `clean_title` using the mode.
- Converted the `milage` column into a numeric format by removing commas and `"mi."`.
- Converted the `price` column into a numeric format by removing `$` and commas.
- Verified data types after cleaning.
- Checked that no missing values remained after preprocessing.

---

## Feature Engineering Performed

The following new features were created:

1. **Car Age** = Current Year − Model Year
2. **Mileage Per Year** = Mileage ÷ Car Age
3. **Luxury Brand** (Binary feature indicating premium brands)
4. **Price Category** (Low, Medium, High)
5. **Car Age Group** (New, Mid-age, Old)

These engineered features can help improve the performance of future machine learning models.

---

## Five Key Insights

1. The dataset contains **4,009 used car records** with **12 features**.
2. Most features are categorical, while only `model_year` is initially numerical.
3. Missing values were present in the `fuel_type`, `accident`, and `clean_title` columns.
4. The vehicles range from **1974** to **2024** model years, with most cars being relatively recent.
5. The `milage` and `price` columns required conversion from text to numeric format before analysis.

---

## Files Included

- **task-3.ipynb** – Complete Exploratory Data Analysis, Data Cleaning, and Feature Engineering.
- **cleaned_used_cars.csv** – Cleaned dataset ready for machine learning.
- **README.md** – Project documentation.

---

## Tools and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Conclusion

This project demonstrates the essential preprocessing steps required before building a machine learning model. After cleaning the dataset and engineering meaningful features, the data is ready for further tasks such as model training, evaluation, and used car price prediction.

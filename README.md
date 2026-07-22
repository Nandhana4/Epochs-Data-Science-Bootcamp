# Google Play Store Apps Dataset Exploration

## Dataset Overview

The Google Play Store Apps dataset contains information about applications available on the Google Play Store. It includes details such as app category, rating, reviews, installs, size, type (Free/Paid), price, content rating, genres, and Android version requirements. This dataset helps analyze app characteristics and understand factors that influence app performance and user ratings.

---

## Business Problem(s)

Developers and businesses often struggle to understand the factors that contribute to an app's success. By analyzing this dataset, we can:

- Identify the characteristics of highly rated apps.
- Understand the distribution of apps across different categories.
- Analyze the relationship between app features and user ratings.
- Help developers make data-driven decisions to improve their applications.

---

## Machine Learning Problem

**Problem Type:** Regression

**Justification:**

The goal is to predict an app's **Rating**, which is a continuous numerical value ranging from 1 to 5. Since the target variable is numerical, this is a **Regression** problem.

---

## Target Variable

- **Rating**

---

## Key Features

The following features can be used to predict an app's rating:

- Category
- Reviews
- Size
- Installs
- Type
- Price
- Content Rating
- Genres
- Last Updated
- Current Version
- Android Version

---

## Dataset Exploration

The following exploratory analysis was performed using the Pandas library:

- Loaded the dataset
- Displayed the first few rows
- Checked the dataset shape
- Examined column names and data types
- Identified missing values
- Generated summary statistics
- Analyzed app categories
- Analyzed Free vs Paid applications

---

## Key Observations

1. The dataset contains **10,841 applications**, with the **Rating** column containing **1,474 missing values**, indicating that data preprocessing is necessary before model building.

2. The **FAMILY** category has the highest number of applications, followed by **GAME** and **TOOLS**, showing that these are the most common app categories in the dataset.

3. The majority of applications are **Free (10,039 apps)**, while only **800** are **Paid**, indicating that free apps dominate the Google Play Store.

---

## Technologies Used

- Python
- Google Colab
- Pandas

---

## Repository Structure

```
├── analysis.ipynb
├── README.md
└── googleplaystore.csv
```

---

## Author

**Nandhana S**

# Oasis Infobyte – Level 1 Task 3: Data Cleaning

## 📌 Project Overview

This project demonstrates professional-level data cleaning and preprocessing using Python, Pandas, NumPy, and Jupyter Notebook.

The objective was to take a deliberately messy Airbnb dataset and systematically transform it into a clean, analysis-ready dataset while documenting each cleaning decision.

## 🎯 Objectives

- Inspect and assess the quality of the raw dataset.
- Identify and handle missing values.
- Detect and remove duplicate records.
- Standardize inconsistent text formatting.
- Detect numerical outliers using the IQR method.
- Correct inappropriate data types.
- Compare the dataset before and after cleaning.
- Export the final cleaned dataset as a new CSV file.

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Jupyter Notebook

## 🔍 Data Cleaning Process

### 1. Data Quality Assessment

The dataset was initially inspected using:

- `df.head()`
- `df.shape`
- `df.info()`
- `df.describe()`
- Missing-value analysis
- Duplicate checks
- Data type inspection

The original dataset contained **48,895 rows and 16 columns**.

### 2. Missing Data Handling

Missing values were analyzed by column and treated according to the nature of each variable.

- `reviews_per_month`: Missing values were replaced with `0` because the affected listings had no reviews.
- `last_review`: Missing values were retained because listings with no reviews do not have a valid last-review date.
- `name` and `host_name`: Rows containing missing values in these fields were removed because the missing records could not be reliably reconstructed and represented a very small proportion of the dataset.

### 3. Duplicate Removal

Duplicate rows were checked using Pandas.

**Duplicate rows identified: 0**

Therefore, no rows were removed due to duplication.

### 4. Standardization

Text-based columns were inspected for inconsistent formatting. Leading and trailing whitespace was removed where necessary while preserving legitimate names and location values.

### 5. Outlier Detection

The **Interquartile Range (IQR)** method was used to identify potential outliers in numerical columns.

Outliers were identified in variables such as:

- Price
- Minimum nights
- Number of reviews
- Reviews per month
- Host listing count
- Latitude and longitude

The detected statistical outliers were retained because extreme values can represent legitimate Airbnb listings and were not automatically considered data errors.

### 6. Data Type Correction

Several data types were corrected to improve analytical accuracy:

| Column | Before | After |
|---|---|---|
| `id` | Integer | String |
| `host_id` | Integer | String |
| `price` | Integer | Float |
| `last_review` | String | Datetime |

Other columns already had appropriate data types and were retained.

## 📊 Before vs After

| Metric | Before Cleaning | After Cleaning |
|---|---:|---:|
| Rows | 48,895 | 48,858 |
| Total Missing Values | 20,141 | 10,037 |
| Duplicate Rows | 0 | 0 |

The final remaining missing values are in `last_review`, where no review date exists for listings with no reviews.

## 📁 Project Files

- `Level_1_Task_3_Data_Cleaning.ipynb` – Jupyter Notebook containing the complete cleaning process and documentation.
- `Level_1_Task_3_Data_Cleaned.csv` – Final cleaned dataset.

## ✅ Outcome

The raw dataset was successfully transformed into a cleaner, more consistent, and analysis-ready dataset while documenting the decisions made throughout the cleaning process.

**Internship:** Oasis Infobyte  
**Task:** Level 1 – Task 3  
**Project:** Data Cleaning
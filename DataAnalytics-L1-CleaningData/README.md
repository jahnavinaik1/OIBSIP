
# Data Cleaning and Preprocessing

## Project Overview

This project demonstrates a systematic data cleaning and preprocessing workflow using Python, Pandas, NumPy, and Jupyter Notebook.

A deliberately messy customer dataset was created to simulate common real-world data quality problems. The dataset was inspected, cleaned, standardised, and transformed into an analysis-ready dataset.

## Objective

The objective of this project is to demonstrate professional data cleaning practices, including:

- Identifying missing values
- Detecting duplicate records
- Correcting inconsistent data formats
- Fixing incorrect data types
- Detecting and treating outliers
- Standardising categorical values
- Comparing dataset quality before and after cleaning
- Exporting the cleaned dataset as a new CSV file

## Technologies Used

- Python
- Pandas
- NumPy
- Jupyter Notebook

## Dataset

The dataset contains customer-related information such as:

- Customer ID
- Name
- Age
- Gender
- Email
- Join Date
- City
- Annual Income
- Purchase Amount

The original dataset was intentionally created with missing values, duplicate records, inconsistent formatting, invalid values, and outliers for data cleaning practice.

## Data Quality Issues Identified

The following issues were identified:

1. Missing values in multiple columns
2. Duplicate customer records
3. Inconsistent Gender values such as `Male`, `male`, `M`, `Female`, `female`, and `F`
4. Inconsistent city capitalization and spacing
5. Invalid age values
6. Different date formats and invalid dates
7. Monetary values stored in inconsistent formats
8. An extreme purchase amount outlier
9. Incorrect or inconsistent data types

## Cleaning Process

### 1. Missing Values

- Missing Age values were replaced using the median.
- Missing Email values were replaced with `Not Provided`.
- Invalid or unavailable Join Date values were converted to missing datetime values.

### 2. Duplicate Removal

Duplicate rows were identified and removed using Pandas `drop_duplicates()`.

### 3. Standardisation

Gender values were standardised to:

- Male
- Female

City names were stripped of unnecessary spaces and converted to a consistent title-case format.

### 4. Data Type Correction

- Customer ID was converted to string format.
- Age was converted to numeric format.
- Annual Income was converted to numeric format.
- Purchase Amount was converted to numeric format.
- Join Date was converted to datetime format.

### 5. Outlier Treatment

The Interquartile Range (IQR) method was used to detect outliers in Purchase Amount.

Extreme values were capped using the calculated lower and upper IQR limits instead of deleting the corresponding customer records.

### 6. Final Validation

The cleaned dataset was checked again for:

- Missing values
- Duplicate records
- Data types
- Valid ranges
- Consistent categorical values

## Before vs After Cleaning

A summary table was created in the Jupyter Notebook to compare:

- Number of rows
- Number of columns
- Missing values
- Duplicate records

This comparison demonstrates the improvement in overall data quality after preprocessing.

## Project Files

```text
DataAnalytics-L1-CleaningData
│
├── Data_Cleaning.ipynb
├── messy_customer_data.csv
├── cleaned_customer_data.csv
├── README.md
│
└── screenshots
    ├── data_quality_report.png
    ├── before_after_summary.png
    └── cleaned_data_check.png

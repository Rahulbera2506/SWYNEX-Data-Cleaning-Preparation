# SWYNEX - Data Cleaning & Preparation

## Project Overview

This project was completed as part of the SWYNEX Technologies Data Cleaning & Preparation task.

The goal of this project was to clean and prepare a public Retail Store Sales dataset using Microsoft Excel Power Query.

## Dataset

**Dataset:** Retail Store Sales - Dirty for Data Cleaning

The dataset contains retail transaction information such as:

- Transaction ID
- Customer ID
- Category
- Item
- Price Per Unit
- Quantity
- Total Spent
- Payment Method
- Location
- Transaction Date
- Discount Applied

## Tool Used

- Microsoft Excel
- Power Query

## Data Cleaning Steps

### 1. Missing Values

Missing values were checked using Power Query Column Quality.

- Missing Item values were replaced with `Unknown`.
- Missing Price Per Unit values were replaced with '0'.
- Missing Quantity values were replaced with `0`.
- Other columns were checked for empty values.

### 2. Duplicate Records

Duplicate records were checked using the transaction information.

No duplicate records requiring removal were identified.

### 3. Data Types

Data types were reviewed and corrected where required.

The `Discount Applied` column was kept as **Text** because it contains:

- `true`
- `false`
- `unknown`

Keeping this column as Text prevents errors caused by converting `unknown` into a Boolean value.

### 4. Inconsistent Values

Categorical columns were checked for inconsistent values, including:

- Category
- Payment Method
- Location
- Discount Applied

No inconsistent values requiring correction were identified.

### 5. Error Check

After cleaning, Power Query Column Quality showed:

- 100% valid values
- 0% errors
- 0% empty values in the cleaned data

## Final Dataset

The cleaned dataset is available in:

`retail_store_sales_cleaned.xlsx`

## Conclusion

The dataset was cleaned and prepared using Power Query by checking missing values, duplicate records, data types, inconsistent values, and errors. The final dataset is ready for further analysis and visualization.

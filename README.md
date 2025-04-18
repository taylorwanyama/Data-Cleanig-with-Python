# Data Cleaning Project 

## Overview

This project focuses on cleaning a cafe sales dataset containing 10,000 entries. The goal is to prepare the dataset for further analysis by handling issues such as missing values, invalid data types, outliers, and duplicates.

---

## Dataset Summary

The dataset includes the following fields:

- **Transaction ID** – Unique ID for each transaction  
- **Item** – Product purchased  
- **Quantity** – Number of units purchased  
- **Price Per Unit** – Unit price of the item  
- **Total Spent** – Total amount spent per transaction  
- **Payment Method** – Method of payment used  
- **Location** – Store location  
- **Transaction Date** – Date when the transaction occurred  

---

##  Data Cleaning Steps

1.**Understanding the Quality of the Data**
  -Detected Missing Values.
  -Confirmed the Data types.
  -Detected Duplictes.
  -Confirmed the Shape of the Data.
2. **Invalid Value Replacement**
   - Replaced erroneous entries such as `"ERROR"` and `"UNKNOWN"` with null (`NaN`) values.

3. **Data Type Conversion**
   - Converted `Quantity`, `Price Per Unit`, and `Total Spent` to numeric types.
   - Converted `Transaction Date` to datetime format.

4. **Handling Missing Values**
   - Identified and retained or replaced missing values based on context and relevance.

5. **Duplicate Removal**
   - Checked for and removed duplicate rows.

6. **Outlier Treatment**
   - Identified outliers in numeric columns using the IQR method.
   - Applied capping to bring extreme values within acceptable range.

7. **Validation**
   - Verified:
     - Row count after cleaning
     - Remaining missing values
     - Presence of duplicates
     - Data retention percentage

---

## Cleaning Results

| Metric                  | Value     |
|-------------------------|-----------|
| Rows After Cleaning     | 10,000    |
| Missing Values Remaining| 0         |
| Duplicate Rows          | 0         |
| Data Loss Percentage    | 0.0%      |

---
## Next Steps

This cleaned dataset can now be used for:
- Exploratory Data Analysis (EDA)
- Dashboard creation
- Predictive modeling

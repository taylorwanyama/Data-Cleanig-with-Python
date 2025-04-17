# 🧼 Data Cleaning Project – Retail Transactions

## 📋 Overview

This project focuses on cleaning a retail transaction dataset containing 10,000 entries. The goal is to prepare the dataset for further analysis by handling issues such as missing values, invalid data types, outliers, and duplicates.

---

## 📂 Dataset Summary

The dataset includes the following fields:

- **Transaction ID** – Unique ID for each transaction  
- **Item** – Product purchased  
- **Quantity** – Number of units purchased  
- **Price Per Unit** – Unit price of the item  
- **Total Spent** – Total amount spent per transaction  
- **Payment Method** – Method of payment used  
- **Location** – Store location  
- **Transaction Date** – Date when transaction occurred  

---

## 🔧 Data Cleaning Steps

1. **Invalid Value Replacement**
   - Replaced erroneous entries such as `"ERROR"` and `"UNKNOWN"` with null (`NaN`) values.

2. **Data Type Conversion**
   - Converted `Quantity`, `Price Per Unit`, and `Total Spent` to numeric types.
   - Converted `Transaction Date` to datetime format.

3. **Handling Missing Values**
   - Identified and retained or replaced missing values based on context and relevance.

4. **Duplicate Removal**
   - Checked for and removed duplicate rows.

5. **Outlier Treatment**
   - Identified outliers in numeric columns using the IQR method.
   - Applied capping to bring extreme values within acceptable range.

6. **Validation**
   - Verified:
     - Row count after cleaning
     - Remaining missing values
     - Presence of duplicates
     - Data retention percentage

---

## 📊 Cleaning Results

| Metric                  | Value     |
|-------------------------|-----------|
| Rows After Cleaning     | 10,000    |
| Missing Values Remaining| 0         |
| Duplicate Rows          | 0         |
| Data Loss Percentage    | 0.0%      |

---

## 📁 Files in this Repo

- `Data Cleaning.ipynb` – Full notebook with step-by-step cleaning process  
- `README.md` – Project summary and documentation

---

## 💡 Key Learnings

- Always standardize unknown values before conversions.
- Capping outliers retains data integrity without losing volume.
- Even after cleaning, trace missing values and document reasons.

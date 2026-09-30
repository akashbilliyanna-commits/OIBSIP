# OIBSIP – Oasis Infobyte Data Analyst Internship





## Task 1: Retail Sales Analysis

This project was completed as part of the Oasis Infobyte Data Analyst Internship.

## Project Overview

The objective of this task is to analyze retail sales data and identify useful patterns and insights related to sales, customers, product categories, quantity, price, age, and gender.

## Dataset

The dataset contains 1,000 retail transactions with information including:

- Transaction ID
- Date
- Customer ID
- Gender
- Age
- Product Category
- Quantity
- Price per Unit
- Total Amount

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- GitHub

## Analysis Performed

- Data cleaning and validation
- Descriptive statistics
- Monthly and quarterly sales analysis
- Gender analysis
- Product category analysis
- Age-group analysis
- Quantity and price analysis
- Customer analysis
- Correlation analysis
- Data visualization

## Key Findings

- Total sales: ₹456,000
- Total transactions: 1,000
- Unique customers: 1,000
- Average transaction value: ₹456.00
- Electronics recorded the highest sales among the product categories.
- Q4 2023 recorded the highest sales among the complete quarters.
- Price per Unit showed a strong positive relationship with Total Amount.
- The dataset contained no missing values, duplicate records, or invalid non-positive values in the checked fields.

## Project File

The complete analysis notebook is available in this repository:

Oasis_Infobyte_Data_Analyst_Task_1_Retail_Sales_Analysis.ipynb

## Internship

Oasis Infobyte – Data Analyst Internship





# Oasis Infobyte – Data Analytics

## Level 1 – Task 2: Customer Segmentation Analysis

### 📌 Project Overview

This project focuses on **Customer Segmentation Analysis** using customer purchasing behaviour from an online retail dataset.

The objective is to segment customers into different groups based on their **Recency, Frequency, and Monetary (RFM)** values using the **K-Means clustering algorithm**. These segments can help businesses understand customer behaviour and develop targeted marketing strategies.

### 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Google Colab
* Jupyter Notebook

### 📊 Project Workflow

1. Loaded and inspected the Online Retail dataset
2. Handled missing customer information
3. Removed cancelled transactions
4. Removed transactions with invalid/zero unit prices
5. Calculated total purchase amount
6. Performed descriptive statistical analysis
7. Created RFM features:

   * Recency
   * Frequency
   * Monetary
8. Standardized the RFM features using `StandardScaler`
9. Used the Elbow Method to determine the number of clusters
10. Applied K-Means clustering
11. Visualized the customer segments
12. Profiled the resulting customer clusters
13. Developed marketing recommendations for each segment

### 📈 Customer Segments

The analysis identified **4 customer segments**:

| Cluster   | Customer Segment               | Description                                                   |
| --------- | ------------------------------ | ------------------------------------------------------------- |
| Cluster 0 | Regular Customers              | Moderate purchase frequency and spending                      |
| Cluster 1 | Inactive / Low-Value Customers | Low frequency, lower spending, and longer time since purchase |
| Cluster 2 | VIP Customers                  | Very high purchase frequency and spending                     |
| Cluster 3 | High-Value Frequent Customers  | Frequent purchases with high spending                         |

### 💡 Key Insight

RFM-based clustering helps identify groups of customers with different purchasing behaviours. Businesses can use these segments to create targeted strategies such as customer retention campaigns, loyalty programs, reactivation offers, and personalized promotions.

### 📁 Files

* `Oasis_Infobyte_Data_Analytics_Level_1_Task_2_Customer_Segmentation.ipynb` – Complete Google Colab/Jupyter Notebook containing the analysis.

### 🎯 Internship

**Organization:** Oasis Infobyte
**Domain:** Data Analytics
**Level:** Level 1
**Task:** Task 2 – Customer Segmentation Analysis






# Oasis Infobyte – Data Analytics Task 3: Data Cleaning

## 📌 Project Overview

This project is part of the **Oasis Infobyte Data Analytics Internship – Task 3**. The objective of this task was to take a messy dataset and systematically clean, standardize, and prepare it for further data analysis.

The dataset contains information about music tours, including artist names, tour titles, rankings, number of shows, actual gross, adjusted gross, average gross, years, and reference information.

## 🎯 Objectives

The main objectives of this task were to:

* Assess the quality of the dataset
* Identify missing values
* Check for duplicate records
* Identify data type issues
* Standardize inconsistent data
* Correct numerical and monetary data types
* Detect potential outliers
* Document cleaning decisions
* Compare the dataset before and after cleaning
* Save the final cleaned dataset as a new CSV file

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Google Colab / Jupyter Notebook**
* **CSV Dataset**

## 🔍 Data Quality Assessment

The initial dataset contained:

* **20 rows**
* **11 columns**
* **0 duplicate rows**
* Missing values in `Peak` and `All Time Peak`
* Several numerical and monetary columns stored as `object`
* Ranking values containing reference markers such as `[4]`
* Monetary values containing `$`, commas, and reference markers

A data quality report was created to understand these issues before cleaning.

## 🧹 Missing Data Handling

The `Peak` column contained **11 missing values**, while `All Time Peak` contained **14 missing values**.

Since these columns represent ranking information, filling the missing values with mean, median, or mode could create incorrect artificial rankings. Therefore, the missing values were retained as `NaN`, while the remaining useful information in those records was preserved.

## 🔄 Duplicate Removal

Duplicate records were checked using Pandas.

**Result:** 0 duplicate rows were found.

Therefore, no records were removed during duplicate handling.

## 📊 Data Standardization

Several columns contained inconsistent formatting and unnecessary reference markers.

The following cleaning operations were performed:

* Removed reference markers from `Peak`
* Removed reference markers from `All Time Peak`
* Removed reference markers from monetary values
* Removed `$` symbols
* Removed commas from monetary values
* Removed unnecessary leading and trailing spaces from text fields
* Standardized `Year(s)` as a string
* Stored `Ref.` as a string

## 🔢 Data Type Correction

The data types were corrected according to the purpose of each column.

| Column         | Final Data Type |
| -------------- | --------------- |
| Rank           | `int64`         |
| Peak           | `Int64`         |
| All Time Peak  | `Int64`         |
| Actual gross   | `float64`       |
| Adjusted gross | `float64`       |
| Artist         | `object`        |
| Tour title     | `object`        |
| Year(s)        | `string`        |
| Shows          | `int64`         |
| Average gross  | `float64`       |
| Ref.           | `string`        |

The monetary columns were converted to `float64` for proper numerical analysis.

## 📈 Outlier Detection

Potential outliers were identified using the **Interquartile Range (IQR) method**.

Outliers were found in:

* `Shows`
* `Average gross`
* `Actual gross`
* `Adjusted gross`

The identified values were reviewed and retained because they represented valid observations rather than obvious data-entry errors.

## 🔎 Before vs After Cleaning

After the cleaning process:

* Total rows remained **20**
* Total columns remained **11**
* Duplicate rows remained **0**
* Missing ranking values were intentionally retained
* Monetary columns were converted from text to `float64`
* `Year(s)` was converted to string
* `Ref.` was converted to string
* Inconsistent formatting was standardized
* Potential outliers were reviewed and documented

## 💾 Output

The cleaned dataset was saved separately so that the original dataset remained unchanged.

**Output file:**

`Oasis_Infobyte_Data_Analytics_Task_3_Cleaned_Dataset.csv`

## 📁 Project Files

* `Oasis_Infobyte_Data_Analytics_Task_3_Data_Cleaning_Akash_B.ipynb` – Complete Jupyter/Colab notebook
* `Oasis_Infobyte_Data_Analytics_Task_3_Cleaned_Dataset.csv` – Final cleaned dataset

## ✅ Final Result

The dataset was successfully transformed from a messy dataset into a clean, structured, and analysis-ready dataset. The cleaning process covered **data quality assessment, missing values, duplicate checking, standardization, data type correction, outlier detection, validation, and final CSV export**.

This project demonstrates practical use of **Python and Pandas for data cleaning and preparation**, which is an important part of the data analytics workflow.

**Thank you!**

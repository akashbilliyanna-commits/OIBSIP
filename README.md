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

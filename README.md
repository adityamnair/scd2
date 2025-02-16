SCD Type 2 Implementation in Databricks with PySpark
Overview
This project demonstrates how to implement Slowly Changing Dimensions Type 2 (SCD2) using Databricks and PySpark. SCD2 is a method used in data warehousing to track changes in dimension tables over time while preserving historical data.
Key Features
✅ Tracks historical changes in dimension tables
✅ Marks old records as inactive while inserting new records
✅ Uses is_active, start_date, and end_date columns for validity
✅ Scalable and optimized for big data processing in Databricks

/scd2-databricks
│── notebooks/
│   ├── scd2_databricks.ipynb   # Jupyter Notebook for SCD2 Implementation
│── data/
│   ├── customers_20220101.csv   # Old Dimension Data
│   ├── customers_20220108.csv   # Updated Dimension Data
│── scripts/
│   ├── scd2_pyspark.py          # SCD2 PySpark Implementation Script
│── README.md                    # Project Documentation


Installation & Setup
1️⃣ Prerequisites
Databricks Community or Enterprise Edition
Apache Spark & PySpark
Python 3.x
Output Example
<img width="677" alt="image" src="https://github.com/user-attachments/assets/0ccf4536-3658-49bb-8db9-c84b580ec10b" />



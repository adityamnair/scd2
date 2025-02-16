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
customer_id	name	email	address	is_active	start_date	end_date
1001	John Doe	john@email.com	NY, USA	0	2024-01-01	2024-02-01
1001	John Doe	john@new.com	NY, USA	1	2024-02-01	NULL
1002	Alice Doe	alice@email.com	LA, USA	1	2024-01-01	NULL

Superstore Sales — Exploratory Data Analysis (EDA)

📌 Project Overview

This project performs exploratory data analysis (EDA) on the Superstore Sales dataset, uncovering patterns in sales, customer segments, regions, and product categories. The goal is to demonstrate core data analysis skills: data cleaning, inspection, aggregation, and business insight generation using Python and Pandas.

📂 Dataset

Source: Superstore Sales dataset (retail orders)
Size: 9,800 rows × 18 columns
Key columns: Order Date, Ship Date, Category, Sub-Category, Region, Segment, Sales

🛠️ Tools Used

Python
Pandas
Jupyter Notebook

🔍 Workflow

1. Data Loading & Inspection

Loaded dataset using pandas.read_csv()
Checked shape, column data types, and structure using .head(), .shape, .info()

2. Data Cleaning

Identified 11 missing values in Postal Code → filled with placeholder
Converted Order Date and Ship Date from text to proper datetime format
Verified no duplicate rows in the dataset

3. Statistical Summary

Generated summary statistics for Sales (mean, median, std, min/max)
Reviewed value counts for categorical columns: Category, Segment, Region, Ship Mode

4. Business Analysis (Groupby Insights)

Total sales by Category, Region, and Ship Mode
Average sales by Customer Segment
Top 5 states by total sales


📊 Key Findings

The dataset is clean, with 0 duplicate rows and only minor missing data in Postal Code.
Sales distribution is right-skewed — the mean (230.77) is much higher than the median (54.49), driven by a small number of high-value transactions (max: 22,638.48).
Office Supplies has the highest order volume (5,909 orders), but Technology generates the highest total revenue (827,455.87) — showing that order volume and revenue don't always align.
The West region leads in total sales (710,219.68), while the South region has the lowest.
The Home Office segment has the highest average order value (243.40), even though Consumer has the most orders overall.
Standard Class is the most-used shipping method, both in order count and total sales.

💡 Business Insight

High order volume does not guarantee high revenue. Office Supplies sells frequently but in low-value transactions, while Technology sells less often but drives significantly more revenue — a critical distinction for prioritizing business strategy.

📁 Files

eda_superstore.ipynb — Full analysis notebook
train.csv — Dataset used (Superstore Sales)

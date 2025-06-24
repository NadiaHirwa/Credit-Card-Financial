# Credit-Card-Financial
project/
│ 
├── data/

│   ├── raw/               # Unprocessed original dataset files

│   └── processed/         # Cleaned and pre-processed datasets used for analysis

│
├── notebooks/

│   ├── cleaning          # Jupyter notebooks for data cleaning and preparation

│   └── data_analysis     # Jupyter notebooks with charts and insights

│
├── results/             # Exported charts (JPG, PNG, HTML) and final dashboard assets

│
└── docs/                  # Documentation including presentation slides and report files


# 📌 Project Overview
This project focuses on analyzing customer credit card data to uncover insights into user behavior, income distribution, credit limit usage, satisfaction levels, and more. It supports both exploratory analysis and dashboard visualization using tools like Plotly and Looker Studio.

# 🧼 Data Cleaning (notebooks/cleaning)
- Removed null values and standardized data types
- Cleaned and grouped categorical variables like Workclass, Card_Category, and Education_Level
- Created new features (e.g., Month for temporal analysis)
- Replaced inconsistent values using .replace() for better grouping

# 📊 Data Analysis Summary
We explored customer behavior through grouped metrics and visualizations:

- Average Income by Education Level
- Customer Distribution by Marital Status (horizontal bar)
- Average Credit Limit per Card Type
- Average Interest Earned per Card Type
- Usage Mode vs. Total Spend (e.g. chip usage)
- Total Transactions Over Time (smoothed time series)
- Spending by Expense Type
- Delinquent Accounts by State (horizontal bar, top 15)
- Customer Funnel by Satisfaction Score
- Occupation-wise Client Distribution
Each chart uses a clean layout with consistent styling (#002366), percentage labels, and is exported as .jpg, .png, and .html for reporting.

✅ Deliverables
- A complete visual dashboard for stakeholder presentation
- Jupyter notebooks with clean, modular code
- Processed dataset ready for modeling or further BI tools
- Reusable templates for similar credit data analysis projects

📌 Technologies Used
- Python (Pandas, Plotly, Numpy)
- Jupyter Notebook
- Looker Studio / Google Data Studio
- CSV data format
- Image export: .jpg, .png, .html

Looker Studio Dashboard: https://lookerstudio.google.com/u/0/reporting/d29f32ef-cbc1-4b61-91a4-120c2888e857/page/p_tgd5vudltd

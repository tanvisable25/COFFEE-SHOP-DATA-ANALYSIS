# COFFEE-SHOP-DATA-ANALYSIS
Pune Coffee Shop Data Analysis (Python Project)

S — Situation:
The Pune Coffee Shop wanted to understand its sales performance, top-selling products, and customer preferences to make data-driven business decisions and improve profitability.

T — Task:
Analyze the coffee shop’s transactional data using Python to uncover sales patterns, identify peak business hours, popular products, and performance across different locations and time periods.

A — Action:

Cleaned and prepared the dataset using Pandas to remove nulls, fix data formats, and standardize fields.

Conducted exploratory data analysis (EDA) to study daily, monthly, and hourly sales trends.

Used Matplotlib and Seaborn for data visualization to showcase key metrics such as total revenue, product popularity, and branch-wise performance.

Built reusable Jupyter notebooks for each analysis section and managed the project using GitHub for version control.

R — Result:

Identified Latte and Cappuccino as the top-selling drinks, accounting for over 30% of total revenue.

Determined morning hours (8 AM – 11 AM) as the busiest period, helping optimize staffing and operations.

Found that Pune City Center branch generated the highest revenue overall.

Delivered actionable insights that can help improve menu strategy and marketing efforts.

📘 GitHub README — Pune Coffee Shop Data Analysis (Python Project)
🧠 Overview

Welcome to my Pune Coffee Shop Data Analysis project!
This project focuses on analyzing sales data from a local coffee shop chain in Pune to uncover valuable business insights. Using Python, I explored patterns in product sales, customer preferences, and time-based performance trends to support data-driven decisions for improved efficiency and profitability.

🎯 Objectives

Analyze daily, monthly, and hourly sales performance.

Identify the best-selling and least-selling coffee products.

Compare performance across multiple store locations.

Discover customer buying patterns and peak business hours.

🛠 Tools and Technologies
Tool / Library	Purpose
Python	Main programming language for data analysis
Pandas	Data cleaning and manipulation
Matplotlib	Visualization of sales trends and product performance
Seaborn	For advanced and aesthetic data visualizations
Jupyter Notebook	Interactive environment for code, charts, and insights
Visual Studio Code	Script development and debugging
Git & GitHub	Version control and project sharing
🧹 Data Preparation & Cleaning

Imported data from CSV into a Pandas DataFrame.

Cleaned missing values, standardized columns, and converted date/time fields.

Added new features like hour, weekday, and month for time-based analysis.

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load and inspect data
df = pd.read_csv('Pune_Coffee_Shop.csv')

# Clean and preprocess
df['Date'] = pd.to_datetime(df['Date'])
df['Hour'] = df['Date'].dt.hour
df['Month'] = df['Date'].dt.month_name()
df.dropna(inplace=True)

📊 Key Analyses

Sales by Product Category
→ Identified top-selling products like Latte, Cappuccino, and Espresso.

Sales by Hour
→ Morning hours (8 AM – 11 AM) showed the highest transaction volume.

Branch-Wise Performance
→ Pune City Center branch contributed the most to total revenue.

Monthly Sales Trends
→ Clear peak observed during weekends and festive months (November–December).

💡 Insights

Top Performers: Latte and Cappuccino lead in sales and customer preference.

Peak Hours: 8 AM – 11 AM and 5 PM – 7 PM are high-traffic times.

Best Branch: Pune City Center outperformed other locations.

Customer Trends: Higher average order values in winter months.

🧭 What I Learned

Practical application of EDA in retail business analysis.

Building clean visual dashboards using Python libraries.

Importance of data cleaning and feature creation before visualization.

GitHub workflow for project version control and documentation.

⚙️ Challenges Faced

Managing missing or inconsistent transactional data.

Creating meaningful time-based insights from timestamps.

Designing clean, business-friendly visualizations.

📈 Results

Enhanced decision-making through actionable sales insights.

Provided visualization-based evidence for branch and product performance.

Built an end-to-end Python analysis workflow for future retail projects.

🧩 Repository Structure
📂 Pune_Coffee_Shop_Analysis
│
├── 📜 1_Data_Cleaning.ipynb
├── 📜 2_Sales_Analysis.ipynb
├── 📜 3_Product_Performance.ipynb
├── 📜 4_Time_Analysis.ipynb
├── 📜 5_Branch_Insights.ipynb
├── 📊 visuals/
│   ├── sales_by_hour.png
│   ├── top_products.png
│   ├── branch_performance.png
│   └── monthly_trends.png
└── README.md

🏁 Conclusion

This project provided deep insights into the operations of a Pune-based coffee chain using Python.
By analyzing product, time, and location-based performance, I was able to highlight key business drivers that can increase revenue and improve efficiency.

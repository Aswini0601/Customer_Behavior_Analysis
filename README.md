# Customer Shopping Behavior Analysis

## 📌 Overview

This project analyzes customer shopping behavior to identify purchasing patterns, customer segments, sales trends, and factors influencing customer purchases.

The project follows an end-to-end data analytics workflow:

**Python → Exploratory Data Analysis → Data Cleaning → MySQL → SQL Analysis → Power BI Dashboard**

The goal is to transform raw customer shopping data into meaningful business insights that can support data-driven decision-making.

---

## 🎯 Project Objectives

- Understand customer purchasing behavior
- Analyze customer segments and purchase patterns
- Identify trends in sales and purchase amounts
- Analyze the impact of discounts and other customer attributes
- Perform SQL-based business analysis
- Build an interactive Power BI dashboard
- Present insights in a clear and business-friendly format

---

## 📊 Dataset Used

**Dataset:** Customer Shopping Behavior Dataset

The dataset contains customer-level shopping information such as:

- Customer ID
- Age
- Gender
- Item Purchased
- Category
- Purchase Amount
- Location
- Size
- Color
- Season
- Review Rating
- Subscription Status
- Discount Applied
- Previous Purchases
- Shipping Type
- Payment Method
- Frequency of Purchases

The dataset was initially loaded and explored using Python before being cleaned and analyzed using SQL and Power BI.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Python** | Data loading, exploration and cleaning |
| **Pandas** | Data manipulation and preprocessing |
| **NumPy** | Numerical analysis |
| **Matplotlib / Seaborn** | Data visualization during EDA |
| **MySQL** | Database storage and SQL analysis |
| **SQL** | Business queries and customer analysis |
| **Power BI** | Interactive dashboard and visualization |
| **DAX** | Calculated measures and KPIs |
| **Power Query** | Data transformation in Power BI |

---

# 🔄 Project Workflow

## 1. Data Loading

The dataset was loaded into Python using Pandas.

```python
import pandas as pd

df = pd.read_csv("customer_shopping_behavior.csv")

df.head()
The initial dataset was inspected to understand:

Number of rows and columns
Data types
Missing values
Duplicate records
Unique values
Basic statistical information
2. Exploratory Data Analysis (EDA)

EDA was performed to understand the structure and distribution of the data.

Key areas analyzed included:

Customer demographics
Purchase amount distribution
Product categories
Customer segments
Discount usage
Subscription status
Purchase frequency
Payment methods
Seasonal purchasing behavior

Examples of Python operations used:

df.info()
df.describe()
df.isnull().sum()
df.nunique()

Visualizations were also created to identify patterns and trends in customer behavior.

3. Data Cleaning

The raw dataset was cleaned before performing SQL and Power BI analysis.

Major data-cleaning steps included:

Handling missing values
Removing duplicate records
Correcting data types
Standardizing categorical values
Renaming columns where required
Checking inconsistent values
Creating useful derived columns

The cleaned dataset was then prepared for database analysis.

4. MySQL Database

The cleaned dataset was imported into a MySQL database.

SQL was used to perform business-oriented analysis and answer questions such as:

How many customers belong to each segment?
What is the average purchase amount?
Which categories generate the most purchases?
How does discount usage affect purchasing behavior?
Which products are most frequently purchased?
What is the average purchase amount by customer segment?
Which categories have the highest average ratings?
What are the purchasing patterns of subscribed customers?

Example:

SELECT 
    category,
    COUNT(*) AS total_orders,
    AVG(purchase_amount) AS avg_purchase_amount
FROM customer
GROUP BY category
ORDER BY total_orders DESC;

Advanced SQL concepts used in the project include:

GROUP BY
Aggregate functions
WHERE
HAVING
CASE WHEN
Subqueries
CTEs (WITH)
Window functions
ROW_NUMBER()
PARTITION BY
ORDER BY
📈 5. Power BI Dashboard

The cleaned data was connected to Power BI to create an interactive dashboard.

The dashboard focuses on key customer and purchasing metrics.

Key KPIs
Total Customers
Total Purchases
Total Purchase Amount
Average Purchase Amount
Average Review Rating
Discount Usage
Subscription Status
Dashboard Analysis

The dashboard provides insights into:

Customer demographics
Purchase behavior
Product categories
Customer segmentation
Subscription patterns
Discount usage
Purchase frequency
Payment methods
Seasonal trends

Power BI features used include:

Power Query
Data transformation
Data modeling
DAX measures
KPI cards
Bar charts
Column charts
Donut charts
Slicers
Interactive filters
📌 Key Results

The analysis provides a consolidated view of customer shopping behavior across different dimensions.

The project helps identify:

- Analyzed 3,900+ customer purchase records
- Identified the highest-performing product categories
- Compared purchasing behavior between subscribed and non-subscribed customers
- Analyzed discount usage and its relationship with purchase behavior
- Built an interactive Power BI dashboard with customer.


The Power BI dashboard brings these insights together into an interactive business reporting solution.

💡 Business Value

This analysis can help businesses:

Better understand their customers
Identify important customer segments
Monitor purchasing trends
Evaluate discount usage
Understand subscription behavior
Identify frequently purchased products
Support data-driven marketing and sales decisions
📁 Project Structure
Customer-Shopping-Behavior-Analysis/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── python/
│   └── customer_behavior_analysis.ipynb
│
├── sql/
│   └── customer_behavior_queries.sql
│
├── powerbi/
│   └── customer_shopping_behavior.pbix
│
├── images/
│   └── dashboard.png
│
└── README.md
🚀 Skills Demonstrated

This project demonstrates practical experience in:

Data Cleaning
Exploratory Data Analysis
Python
Pandas
SQL
MySQL
Data Transformation
Data Analysis
Power BI
DAX
Data Visualization
Business Intelligence
Customer Analytics
📌 Conclusion

The Customer Shopping Behavior Analysis project demonstrates an end-to-end data analytics workflow, starting from raw data preparation in Python and progressing through SQL-based analysis in MySQL to interactive business reporting in Power BI.

The project showcases the ability to work with raw datasets, clean and transform data, perform analytical SQL queries, and communicate business insights through interactive dashboards.






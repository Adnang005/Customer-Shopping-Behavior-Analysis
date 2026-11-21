# Customer Shopping Behavior Analysis

## Project Overview

This project focuses on analyzing customer shopping behavior to identify purchasing patterns, understand customer preferences, evaluate sales performance, and generate actionable business insights.

The project follows an end-to-end data analytics workflow using **Python, Pandas, SQLite, SQL, Matplotlib, Seaborn, and Microsoft Power BI**.

The analysis explores customer demographics, product categories, purchasing frequency, seasonal trends, payment methods, shipping preferences, subscription status, discounts, and customer reviews.

## Business Objectives

- Analyze overall sales performance and purchasing behavior.
- Identify top-performing product categories.
- Understand customer purchasing patterns across different age groups and genders.
- Evaluate seasonal sales trends.
- Compare purchasing behavior of subscribed and non-subscribed customers.
- Analyze discount usage and customer spending.
- Identify popular payment methods and shipping preferences.
- Understand customer satisfaction through review ratings.
- Develop interactive dashboards to communicate business insights.

## Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Data cleaning and analysis |
| Pandas | Data manipulation and preprocessing |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualizations |
| SQLite | Database management |
| SQL | Business data analysis |
| SQLAlchemy | Python-SQLite connection |
| Microsoft Power BI | Interactive dashboard development |
| Jupyter Notebook | Project development environment |

## Dataset Information

**Dataset:** Customer Shopping Behavior

The dataset contains 3,900 customer purchase records.

The cleaned dataset used in the analysis contains 19 columns, including:

- customer_id
- age
- gender
- item_purchased
- category
- purchase_amount
- location
- size
- color
- season
- review_rating
- subscription_status
- shipping_type
- discount_applied
- previous_purchases
- payment_method
- frequency_of_purchases
- age_group
- purchase_frequency_days

*Note: The `promo_code_used` column was present in the original dataset but was not available in the final SQLite table and cleaned DataFrame used for the completed analysis.*

## Project Workflow

### 1. Data Loading and Exploration

- Imported the dataset using Pandas.
- Explored dataset dimensions and column information.
- Checked data types and missing values.
- Examined the overall structure of the dataset.

### 2. Data Cleaning and Preprocessing

- Handled missing values in the review_rating column.
- Checked for missing values after preprocessing.
- Prepared the dataset for further analysis.
- Ensured the cleaned dataset was suitable for SQL analysis and visualization.

### 3. Feature Engineering

Created two additional features:

- **Age Group:** Categorized customers into different age groups.
- **Purchase Frequency Days:** Converted purchasing frequency into a numerical representation for further analysis.

### 4. SQL Analysis Using SQLite

Stored the cleaned dataset in an SQLite database named `customer_behavior.db`, using a table called `customer`.

Performed business analysis using SQL queries, including:

- Overall business performance.
- Sales and purchases by age group.
- Sales by product category.
- Discount versus non-discount sales analysis.
- Average purchase amount.
- Customer purchasing behavior.

SQL functions and operations used:

`SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`, `COUNT()`, `SUM()`, `AVG()`, and `ROUND()`.

### 5. Exploratory Data Analysis and Visualization

Created 12 visualizations using Python, Matplotlib, and Seaborn.

The visualizations include:

1. Total Sales by Product Category.
2. Total Purchases by Age Group.
3. Customer Distribution by Gender.
4. Seasonal Sales Analysis.
5. Sales by Subscription Status.
6. Purchases by Payment Method.
7. Purchases by Shipping Type.
8. Discount versus Non-Discount Sales.
9. Average Review Rating by Category.
10. Customer Purchase Frequency Distribution.
11. Total Sales by Age Group.
12. Average Purchase Amount by Gender.

### 6. Power BI Dashboard

Developed an interactive Power BI dashboard to present key business metrics and customer insights.

**Key Performance Indicators (KPIs):**

- Total Sales: $233,081
- Total Purchases: 3,900
- Average Purchase Amount: $59.76
- Average Review Rating: 3.75

**Dashboard Pages:**

**Page 1 – Business Overview**
- Overall business KPIs.
- Sales by product category.
- Purchases by age group.
- Sales distribution by gender.
- Seasonal sales.
- Subscription sales analysis.

**Page 2 – Customer Insights**
- Payment method preferences.
- Shipping type analysis.
- Discount analysis.
- Average customer ratings.
- Purchase frequency.
- Sales by age group.
- Average purchase amount by gender.

Interactive slicers include:
- Age Group
- Gender
- Category
- Season

## Key Business Insights

- The Clothing category generated the highest sales, totaling $104,264.
- Accessories ranked second, generating $74,200 in sales.
- Young Adults recorded the highest number of purchases, with 1,028 transactions.
- Young Adults also generated the highest total sales among the analyzed age groups, at $62,143.
- Purchases without discounts generated higher total sales than purchases with discounts.
- The overall average purchase amount was $59.76.
- The average customer review rating was 3.75 out of 5.

These findings help identify customer segments, product categories, and purchasing patterns that can support better business decisions.

## Repository Structure

```text
Customer-Shopping-Behavior-Analysis/
│
├── data/
│   └── customer_shopping_cleaned.csv
│
├── notebooks/
│   └── customer_shopping_analysis.ipynb
│
├── database/
│   └── customer_behavior.db
│
├── powerbi/
│   └── customer_shopping_dashboard.pbix
│
├── visualizations/
│   └── charts/
│
├── README.md
│
└── requirements.txt
```

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Customer-Shopping-Behavior-Analysis.git
```

### 2. Install Required Libraries

```bash
pip install pandas matplotlib seaborn sqlalchemy jupyter
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

### 4. Run the Analysis

Open the project notebook and execute the cells in sequence to explore the data, perform preprocessing, conduct analysis, and generate visualizations.

### 5. Open the Power BI Dashboard

Open the `.pbix` file using Microsoft Power BI Desktop to explore the interactive dashboard.

## Conclusion

This project demonstrates an end-to-end data analytics process, from raw data exploration and preprocessing to SQL-based business analysis, data visualization, and interactive dashboard development.

It provided practical experience in transforming raw customer shopping data into meaningful insights that can help businesses understand customer behavior, evaluate sales performance, and make data-driven decisions.

## Author

**Your Name**

Aspiring Data Analyst

Skills: Python | SQL | SQLite | Pandas | Data Cleaning | Exploratory Data Analysis | Data Visualization | Power BI

---

*If you found this project useful, feel free to explore the repository and share your feedback.*

# Customer Shopping Behavior Analysis

## Overview

This project analyzes customer shopping behavior to identify purchasing patterns, customer segments, product trends, and factors influencing purchase decisions.

The project follows an end-to-end data analytics workflow using **Python, MySQL, and Power BI**, with the final insights presented through a project report and presentation.

## Business Objective

The objective is to leverage customer shopping data to:

* Identify customer and purchasing trends
* Understand customer segments and purchase behavior
* Analyze product and category performance
* Evaluate the impact of discounts, reviews, seasons, and payment preferences
* Generate actionable insights for customer engagement and marketing strategies

## Dataset

The project uses the **Customer Shopping Trends** dataset containing **3,900 customer records**.

Key attributes include:

* Customer ID
* Age
* Gender
* Item Purchased
* Category
* Purchase Amount
* Location
* Size
* Color
* Season
* Review Rating
* Subscription Status
* Shipping Type
* Discount Applied
* Promo Code Used
* Previous Purchases
* Payment Method
* Frequency of Purchases

## Tools & Technologies

* **Python** — Data loading, cleaning, and Exploratory Data Analysis
* **Pandas** — Data manipulation and analysis
* **MySQL Server** — Database storage and SQL analysis
* **MySQL Workbench** — Database management and query execution
* **Power BI** — Interactive dashboard and visualization
* **Gamma** — Project presentation
* **GitHub** — Project documentation and version control

## Project Workflow

### 1. Data Loading & Exploratory Data Analysis — Python

* Loaded the dataset using Pandas
* Inspected the dataset using `df.info()`
* Generated descriptive statistics using `df.describe()`
* Examined numerical and categorical variables
* Checked for missing values and potential data quality issues
* Analyzed distributions and basic customer purchasing patterns

### 2. Data Cleaning & Preparation — Python

* Checked and handled missing values
* Verified and corrected data types
* Standardized column names and categorical values
* Prepared the dataset for SQL analysis and visualization

### 3. SQL Analysis — MySQL

The cleaned dataset was imported into MySQL for business-oriented analysis.

SQL analysis covered:

* Customer demographics
* Revenue by gender and category
* Purchase frequency
* Customer loyalty segments
* Product popularity
* Average product ratings
* Discount and promotional behavior
* Payment method preferences
* Repeat purchasing patterns
* Top products within each category

SQL concepts used include:

* `SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`
* Aggregate functions
* `CASE WHEN`
* Subqueries
* Common Table Expressions (CTEs)
* Window functions
* `ROW_NUMBER()`

### 4. Power BI Dashboard

An interactive Power BI dashboard was developed to visualize the major findings from the analysis.

The dashboard covers:

* Total customers
* Total revenue
* Average purchase amount
* Average review rating
* Customer segments
* Category performance
* Purchase frequency
* Seasonal purchasing trends
* Payment preferences
* Discount usage
* Product performance

### 5. Report & Presentation

A project report was prepared to document:

* Business problem
* Dataset and methodology
* Data preparation
* Exploratory analysis
* SQL analysis
* Key findings
* Business recommendations

A presentation was also created using **Gamma** to communicate the findings and recommendations in a concise and visual format.

## Dashboard

The Power BI dashboard provides an interactive overview of customer shopping behavior and enables analysis across customer demographics, products, categories, seasons, and purchasing patterns.

![Power BI Dashboard](images/dashboard.png)

## Key Results

The analysis provides insights into:

* Customer segments based on previous purchase behavior
* Most frequently purchased products and categories
* Purchasing patterns across different demographics
* Preferred payment and shipping methods
* Impact of discounts and promotional offers
* Seasonal purchasing trends
* Product ratings and customer preferences
* Opportunities for improving customer retention and targeted marketing

## Project Structure

```text
Customer-Shopping-Behavior-Analysis/
│
├── data/
│   └── customer_shopping_trends.csv
│
├── python/
│   └── customer_analysis.ipynb
│
├── sql/
│   └── customer_analysis.sql
│
├── powerbi/
│   └── customer_shopping_dashboard.pbix
│
├── report/
│   └── project_report.pdf
│
├── presentation/
│   └── project_presentation.pdf
│
├── images/
│   └── dashboard.png
│
└── README.md
```

## How to Run

### Python

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run the analysis notebook to perform data exploration and cleaning.

### MySQL

Create the database:

```sql
CREATE DATABASE customer_shopping;
```

Select the database:

```sql
USE customer_shopping;
```

Import the cleaned dataset into MySQL and execute the SQL queries provided in:

```text
sql/customer_analysis.sql
```

### Power BI

1. Open the `.pbix` file using Power BI Desktop.
2. Update the MySQL connection if required.
3. Refresh the dataset.
4. Explore the interactive dashboard.

## Deliverables

* Python EDA and data-cleaning notebook
* Cleaned dataset
* MySQL database and SQL queries
* Power BI interactive dashboard
* Project report
* Gamma presentation
* GitHub repository

## Conclusion

This project demonstrates an end-to-end data analytics workflow, from **data preparation and exploratory analysis to SQL-based business analysis and interactive Power BI visualization**. The insights generated from customer shopping behavior can support data-driven decisions related to **customer segmentation, product strategy, promotions, and customer engagement**.

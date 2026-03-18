# Customer Shopping Behavior Analysis

## Overview

This project analyzes customer shopping behavior using transactional data from **3,900 purchases across multiple product categories**. The objective is to extract actionable insights related to customer preferences, spending patterns, and business performance.

The project follows an end-to-end analytics pipeline involving **Python (EDA), SQL (business analysis), and Power BI (visualization)**.

---

## Dataset Summary

* **Total Records:** 3,900
* **Features:** 18

### Key Attributes:

* Customer demographics (age, gender, location, subscription status)
* Purchase details (item, category, amount, season, size, color)
* Behavioral features (discount usage, purchase frequency, ratings, shipping type)

---

## Project Workflow

### 1. Data Preprocessing (Python)

* Loaded dataset using pandas
* Handled missing values using **median imputation (category-wise)**
* Standardized column names (snake_case)
* Created new features:

  * `age_group`
  * `purchase_frequency_days`
* Removed redundant columns (`promo_code_used`)
* Loaded cleaned data into PostgreSQL

---

### 2. Exploratory Data Analysis

* Analyzed feature distributions and summary statistics
* Identified patterns in customer behavior and spending
* Performed correlation and trend analysis

---

### 3. SQL-Based Business Analysis

Performed advanced queries in PostgreSQL to answer key business questions:

* Revenue comparison by gender
* High-spending customers using discounts
* Top-rated products based on reviews
* Shipping type impact on purchase amount
* Subscriber vs non-subscriber analysis
* Discount-heavy product identification
* Customer segmentation (New, Returning, Loyal)
* Revenue contribution by age group

---

### 4. Dashboard (Power BI)

Built an interactive dashboard to visualize insights:

* Customer distribution
* Revenue by category and age group
* Subscription status breakdown
* Sales trends

The dashboard highlights:

* ~3.9K customers
* Average purchase ≈ $59.76
* Average rating ≈ 3.75 

---

## Key Insights

* Express shipping customers spend more per transaction
* Loyal customers form the majority of the customer base
* Certain products (like accessories and clothing items) dominate sales
* Discount strategies influence high-value purchases
* Subscription status impacts revenue distribution

---

## Business Recommendations

* Promote subscription benefits to increase retention
* Introduce loyalty programs for repeat customers
* Optimize discount strategies to balance profit and sales
* Focus marketing on high-revenue age groups
* Highlight top-rated products in campaigns

---

## Tech Stack

* **Python:** Pandas, NumPy, Matplotlib, Seaborn
* **SQL:** PostgreSQL
* **Visualization:** Power BI
* **Tools:** Jupyter Notebook

---

## Repository Contents

* `Customer_Shopping_Behavior_Analysis.ipynb` → Data cleaning & EDA
* `customer_behavior_sql_queries.sql` → Business queries
* `customer_behavior_dashboard.pbix` → Power BI dashboard
* `customer_shopping_behavior.csv` → Dataset
* `Customer Shopping Behavior Analysis.pdf` → Detailed report
* `Customer-Shopping-Behavior-Analysis.pptx` → Presentation

---

## How to Run

```bash
git clone https://github.com/chaitanyakumarcodes/customer-analytics.git
cd customer-analytics
```

1. Run the Jupyter notebook for preprocessing and EDA
2. Execute SQL queries in PostgreSQL
3. Open `.pbix` file in Power BI to view dashboard

---

## Conclusion

This project demonstrates a complete data analytics workflow—from raw data processing to business insights and visualization. It showcases how data can be used to drive strategic decisions in a retail environment.

---

# 📊 Olist E-Commerce Sales & Customer Analytics Dashboard

## 🖥️ Dashboard Preview

![Olist E-Commerce Power BI Dashboard](dashboard.png)

---

## 📌 Project Overview

This project focuses on analyzing the Brazilian Olist E-Commerce Public Dataset using Microsoft Power BI.

The main objective is to transform raw e-commerce data into meaningful business insights through data cleaning, data transformation, data modeling, DAX calculations, and interactive visualizations.

The dashboard provides an overview of sales performance, customer distribution, product category performance, payment preferences, customer satisfaction, and delivery operations.

## 🎯 Business Problem

E-commerce businesses generate large amounts of data related to orders, customers, products, payments, and deliveries. Without proper analysis, it becomes difficult to identify business performance trends and improvement opportunities.

This project addresses three main business problems:

1. **Sales Performance Analysis:** Identify monthly sales trends, revenue performance, and top-performing product categories.
2. **Customer Behavior Analysis:** Understand customer distribution across states, payment preferences, and customer satisfaction.
3. **Delivery Performance Analysis:** Evaluate average delivery time and identify opportunities to improve delivery efficiency.

## 🎯 Project Objectives

- Analyze overall sales and revenue performance.
- Identify the highest revenue-generating product categories.
- Understand monthly sales trends.
- Analyze customer distribution across Brazilian states.
- Evaluate payment method preferences.
- Measure customer satisfaction through review scores.
- Analyze average order delivery time.

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Microsoft Power BI | Dashboard development |
| Power Query | Data cleaning and transformation |
| DAX | Measures and calculations |
| Data Modeling | Relationships between tables |
| CSV / Excel | Data source and handling |
| GitHub | Project documentation and version control |

## 📈 Key Performance Indicators (KPIs)

| KPI | Description |
|---|---|
| Total Sales | Total revenue from order items |
| Total Orders | Unique number of orders |
| Total Customers | Unique number of customers |
| Average Order Value | Average sales value per order |
| Total Items Sold | Total number of order items |
| Total Freight | Total freight charges |
| Average Delivery Days | Average time taken to deliver orders |
| Average Review Score | Average customer review rating |

### Dashboard KPI Highlights

| Metric | Result |
|---|---:|
| Total Sales | 13.59M |
| Total Orders | 99K |
| Total Customers | 96K |
| Average Order Value | 136.68 |
| Average Delivery Days | 12.50 Days |
| Average Review Score | 4.09 / 5 |

*Values are based on the current dashboard view.*

## 📊 Dashboard Features & Analysis

### 1. Sales Performance Analysis
- Monthly sales trend analysis.
- Overall sales revenue tracking.
- Identification of sales patterns over time.

### 2. Product Category Analysis
- Top 10 product categories by sales.
- Comparison of category-wise revenue.
- Identification of high-performing categories.

### 3. Customer Analysis
- Customer distribution by Brazilian state.
- Analysis of customer locations.
- Understanding customer reach.

### 4. Payment Method Analysis
- Payment distribution by payment type.
- Analysis of customer payment preferences.
- Comparison of payment methods.

### 5. Customer Review Analysis
- Distribution of customer review scores.
- Average customer review score.
- Customer satisfaction overview.

### 6. Delivery Performance Analysis
- Average delivery days.
- Evaluation of order delivery performance.

## 🔍 Key Business Questions

1. Which product categories generate the highest sales, and how do sales trends change over time?
2. Which states have the highest number of customers, and what are their preferred payment methods?
3. What is the average delivery time, and how satisfied are customers with their shopping experience?

## 🧮 DAX Measures

The following DAX measures were created for business analysis:

```dax
Total Sales =
SUM('olist_order_items_dataset'[price])

Total Orders =
DISTINCTCOUNT('olist_orders_dataset'[order_id])

Total Customers =
DISTINCTCOUNT('olist_customers_dataset'[customer_unique_id])

Average Order Value =
DIVIDE([Total Sales], [Total Orders], 0)

Total Items Sold =
COUNTROWS('olist_order_items_dataset')

Total Freight =
SUM('olist_order_items_dataset'[freight_value])

Average Review Score =
AVERAGE('olist_order_reviews_dataset'[review_score])
```

## 🗂️ Dataset Information

**Dataset:** Brazilian E-Commerce Public Dataset by Olist

**Source:** Kaggle

https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

The dataset contains information about:
- Orders
- Order Items
- Payments
- Customers
- Products
- Sellers
- Reviews
- Geolocation
- Product Category Translation

## 📁 Project Structure

All project files are maintained in a single folder:

```text
Olist-Ecommerce-PowerBI-Project/
│
├── Olist_Dashboard.pbix
├── dashboard.png
├── olist_orders_dataset.csv
├── olist_order_items_dataset.csv
├── olist_order_payments_dataset.csv
├── olist_customers_dataset.csv
├── olist_products_dataset.csv
├── olist_sellers_dataset.csv
├── olist_order_reviews_dataset.csv
├── olist_geolocation_dataset.csv
├── product_category_name_translation.csv
└── README.md
```

## 💡 Key Learnings

Through this project, I gained practical experience in:

- Data cleaning and transformation using Power Query.
- Creating relationships between multiple tables.
- Developing DAX measures for business KPIs.
- Designing interactive dashboards using Power BI.
- Analyzing business performance through data visualization.
- Converting business questions into meaningful insights.

## 🚀 Conclusion

This project demonstrates how Power BI can transform raw e-commerce data into an interactive business intelligence dashboard.

It provides insights into sales performance, customer behavior, product categories, payment preferences, customer satisfaction, and delivery efficiency to support data-driven decision-making.

---

## 👩‍💻 Project Details

**Project Name:** Olist E-Commerce Sales & Customer Analytics Dashboard

**Domain:** E-Commerce / Business Intelligence

**Tool:** Microsoft Power BI

**Project Type:** Data Analytics & Visualization

---

⭐ If you find this project useful, feel free to explore the repository and share your feedback!





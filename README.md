# Superstore Sales & Profit Analysis | Power BI

## Project Overview

An interactive Power BI dashboard built to analyze sales performance, profitability, customer behavior, product performance, and shipping trends using the Sample Superstore dataset.

The project transforms raw data into meaningful business insights through data modeling, data transformation, DAX measures, and interactive visualizations.

## Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Data Modeling
- Star Schema

## Data Model

Designed a Star Schema data model to organize transactional data and support efficient business analysis.

The model consists of one central fact table connected to four dimension tables.

### Fact Table

**fact sales**

Stores transactional data used for sales, profit, order, and shipping analysis.

Key fields include:
- Order ID
- Order Date
- Customer ID
- Product ID
- Sales
- Profit
- Quantity
- Discount
- Postal Code
- Lead-time Category

### Dimension Tables

**Dimcustomer**

Contains customer-related information:
- Customer ID
- Customer Name
- Segment

Used to analyze customer behavior and performance across different customer segments.

**Dimproduct**

Contains product-related information:
- Product ID
- Product Name
- Short Product Name
- Category
- Sub-Category

Used to analyze product performance and compare sales and profitability across categories and sub-categories.

**Dimdate**

Contains date-related attributes:
- Date
- Year
- Quarter
- Month
- Month Number
- Month Short

Used for time-based analysis, sales trends, and year-over-year comparisons.

**Dimcity**

Contains geographical information:
- City
- State
- Region
- Country
- Postal Code

Used to analyze sales performance across different geographical locations.

### Relationships

The dimension tables connect to the central fact table through one-to-many relationships:

- Dimcustomer → fact sales
- Dimproduct → fact sales
- Dimdate → fact sales
- Dimcity → fact sales

This structure separates transactional data from descriptive attributes and supports analysis across customers, products, time, and geography.

### Data Model Diagram

![Data Model](screenshots/data-model.png)

## Dashboard Pages

### 1. Sales Overview & Performance

Provides an overview of overall business performance through interactive KPIs and visualizations.

Key metrics and analyses:
- Net Sales
- Total Orders
- Net Profit
- Profit Margin
- Average Order Value
- Sales by Category
- Sales by Year
- Sales by Region
- Sales by State
- Sales vs. Profit by Year

The page includes interactive filters for customer segment, region, and year to explore business performance across different dimensions.

![Sales Overview & Performance](screenshots/sales-overview.png)

### 2. Product & Customer Analysis

Focuses on product performance, customer contributions, and shipping efficiency.

Key metrics and analyses:
- Total Quantity
- Total Customers
- Average Order Value
- Total Orders
- Average Shipping Days
- Top 5 Products by Sales
- Top 5 Sub-Categories by Profit
- Sales by Segment
- Orders by Lead Time
- Top 10 Customers

This page helps identify top-performing products, profitable sub-categories, valuable customers, and shipping lead-time patterns.

![Product & Customer Analysis](screenshots/product-customer-analysis.png)

## DAX Measures

Created 16 DAX measures to calculate key performance indicators and support business analysis.

### Sales Performance
- Total Sales
- Sales YTD
- Sales PY
- Sales YOY%

### Profitability Analysis
- Net Profit
- Profit Margin
- Profit YTD
- AVG Profit Per Order

### Customer Analysis
- Total Customers
- Sales per Customer

### Order Analysis
- Total Orders
- AVG Order Value
- Total Qty
- Unit per Order

### Shipping & Discounts
- AVG shipping days
- AVG discount

These measures support the analysis of sales trends, year-over-year performance, profitability, customer contributions, order metrics, shipping efficiency, and discount patterns.

## Key Skills Demonstrated

- Data Cleaning and Transformation
- Data Modeling and Star Schema Design
- DAX Measure Development
- KPI Development
- Sales and Profitability Analysis
- Customer and Product Performance Analysis
- Time-Based Analysis
- Geographical Analysis
- Interactive Dashboard Design
- Business Intelligence Reporting

## Dataset

The project uses the Sample Superstore dataset for educational and portfolio purposes.
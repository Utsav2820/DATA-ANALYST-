# Internet Sales Performance Dashboard

## Dashboard Link

https://bitmesra-my.sharepoint.com/:u:/g/personal/btech10618_23_bitmesra_ac_in/IQDcnXS0M5m6TbEJZHc6ehX_AVEzKtzEmcIkzX4YAgM7MUY?e=YsuFa8

---

# Problem Statement

This dashboard helps Sales Managers and Sales Representatives monitor Internet Sales performance across customers, products, and time periods. The dashboard provides visibility into overall sales performance, customer purchasing behavior, product performance, and budget achievement.

By using interactive visualizations and KPI tracking, stakeholders can identify high-performing customers and products, monitor sales trends, compare actual sales against budget targets, and make data-driven business decisions.

The dashboard addresses the following business requirements:

* Monitor overall Internet Sales performance.
* Compare Sales against Budget targets.
* Identify Top Customers contributing to revenue.
* Identify Top Products generating sales.
* Analyze customer-level sales performance.
* Analyze product-level sales performance.
* Track sales trends over time.
* Enable drill-down analysis through dynamic filters.

---

# Business Requirements

## Sales Manager

### Requirement 1

Obtain a dashboard overview of Internet Sales performance.

**Business Value**

* Understand overall sales performance.
* Identify top-performing products and customers.
* Track business growth.

**Acceptance Criteria**

* Dashboard refreshes daily.
* Interactive KPI tracking.
* Sales trends available over time.

---

### Requirement 2

Monitor Sales against Budget.

**Business Value**

* Track target achievement.
* Identify sales gaps.
* Improve forecasting and planning.

**Acceptance Criteria**

* Budget comparison KPIs.
* Sales vs Budget trend analysis.
* Variance tracking.

---

## Sales Representative

### Requirement 3

View customer-level sales performance.

**Business Value**

* Identify high-value customers.
* Improve customer follow-up activities.
* Discover upselling opportunities.

**Acceptance Criteria**

* Customer filtering functionality.
* Customer sales analysis page.
* Customer performance matrix.

---

### Requirement 4

View product-level sales performance.

**Business Value**

* Identify best-selling products.
* Monitor product demand.
* Support inventory and sales planning.

**Acceptance Criteria**

* Product filtering functionality.
* Product sales analysis page.
* Product performance matrix.

---

# Data Source

The dashboard utilizes Internet Sales transactional data and Budget data imported into Power BI.

### Data Sources

* Internet Sales Dataset
* Budget Planning Dataset (Excel)
* Customer Data
* Product Data
* Date Dimension

---

# Steps Followed

### Step 1

Loaded Sales, Customer, Product, and Budget datasets into Power BI Desktop.

### Step 2

Opened Power Query Editor and performed data profiling using:

* Column Quality
* Column Distribution
* Column Profile

### Step 3

Validated all data types including:

* Dates
* Currency fields
* Numerical fields
* Text attributes

### Step 4

Removed duplicate records and standardized data formats.

### Step 5

Handled missing and inconsistent values where applicable.

### Step 6

Created relationships between:

* Sales Table
* Customer Table
* Product Table
* Date Table
* Budget Table

### Step 7

Built a star schema data model to improve reporting performance.

### Step 8

Created Date Hierarchy for Year and Month analysis.

### Step 9

Created DAX Measures for key KPIs.

### Step 10

Developed Sales vs Budget KPI visual.

### Step 11

Created monthly Sales vs Budget trend analysis.

### Step 12

Built Product Category distribution analysis.

### Step 13

Created Top 10 Customer ranking visual.

### Step 14

Created Top 10 Product ranking visual.

### Step 15

Added slicers for:

* Year
* Month
* Customer City
* Category
* Sub Category
* Product Name

### Step 16

Designed Customer Details page with customer-level drill-down analysis.

### Step 17

Designed Product Details page with product-level drill-down analysis.

### Step 18

Created matrix visuals for detailed transactional analysis.

### Step 19

Applied formatting, color themes, and interactive navigation.

### Step 20

Published dashboard to Power BI Service and configured refresh schedules.

---

# Dashboard Pages

## Page 1 – Sales Overview

Provides a high-level summary of:

* Total Sales
* Total Budget
* Sales vs Budget Variance
* Sales Trend by Month
* Sales by Product Category
* Top 10 Customers
* Top 10 Products

---

## Page 2 – Customer Details

Provides customer-level analysis including:

* Customer Sales Matrix
* Monthly Sales Performance
* Budget Comparison
* Top Customers Analysis
* Customer Filters

---

## Page 3 – Product Details

Provides product-level analysis including:

* Product Sales Matrix
* Product Performance Tracking
* Monthly Product Sales Trends
* Product Ranking Analysis
* Product Filters

---

# DAX Measures Used

```DAX
Total Sales =
SUM(FactInternetSales[Sales Amount])

Total Budget =
SUM(Budget[Budget Amount])

Sales Variance =
[Total Sales] - [Total Budget]

Budget Achievement % =
DIVIDE([Total Sales],[Total Budget],0)

Total Customers =
DISTINCTCOUNT(Customer[Customer Key])

Total Products =
DISTINCTCOUNT(Product[Product Key])

Sales Rank =
RANKX(ALL(Customer), [Total Sales], , DESC)
```

---

# Key Insights

## Sales Performance

* Total Sales achieved: 16.35 Million
* Total Budget: 15.30 Million
* Sales exceeded budget by approximately 1.05 Million.

## Budget Achievement

* Sales performance remained above budget targets for most periods.
* Strong growth observed during the second half of the year.

## Customer Analysis

* Top customers contribute a significant share of overall revenue.
* Customer-level analysis helps identify key accounts for retention and upselling initiatives.

## Product Analysis

* Bikes category generates the highest proportion of sales revenue.
* Mountain Bike products dominate top-selling product rankings.

## Trend Analysis

* Sales steadily increased throughout the year.
* Highest sales performance observed during the final quarter.

---

# Business Recommendations

### 1. Focus on High-Value Customers

Develop targeted engagement strategies for top customers to maximize retention and repeat purchases.

### 2. Expand High-Performing Product Lines

Increase inventory and promotional efforts for best-selling bike products.

### 3. Improve Low-Performing Categories

Analyze underperforming product categories and introduce pricing or marketing initiatives.

### 4. Strengthen Forecasting

Leverage historical trends to improve budgeting and sales forecasting accuracy.

### 5. Monitor Budget Variance Monthly

Track monthly variances to proactively identify performance gaps and opportunities.

---

# Tools & Technologies

* Power BI Desktop
* Power Query
* DAX
* Microsoft Excel
* Data Modeling
* Data Visualization

---

# Skills Demonstrated

* Data Cleaning
* Data Transformation
* Data Modeling
* DAX Calculations
* KPI Development
* Budget vs Actual Analysis
* Customer Analytics
* Product Analytics
* Interactive Dashboard Design
* Business Intelligence Reporting
* Data Storytelling
* Sales Performance Analysis

---

# Dashboard Snapshot

## Sales Overview

https://github.com/user-attachments/assets/848ea786-730d-4268-ae23-e0a8997cc812 

## Customer Details

https://github.com/user-attachments/assets/bce57da1-7bdf-4c13-8939-64bc3a6133eb 

## Product Details

https://github.com/user-attachments/assets/a8ea5c9b-2a14-457e-a7e7-a2c09246cb99

---

# Conclusion

The Internet Sales Performance Dashboard provides a comprehensive view of sales operations by combining sales, customer, product, and budget data into a centralized reporting solution. The dashboard enables stakeholders to monitor performance, identify growth opportunities, and make informed business decisions through interactive and data-driven insights.



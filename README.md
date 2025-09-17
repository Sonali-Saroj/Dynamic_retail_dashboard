# **Dynamic_retail_dashboard In Excel**
## **Overview**
The **Dynamic Retail Dashboard** is an interactive and data-driven tool built in Excel to visualize and analyze retail data.
It connects to datasets hosted on GitHub, uses Power Query for data transformation, and presents insights through dynamic charts and KPIs.This dashboard solves key business questions and enables informed decision-making.
---

## Datasets Used

### 1. Orders Table

The Orders table contains details of customer orders, including product, shipping, and financial metrics.

#### ** Sample Data:**

Order ID	Returned	Order Date	Ship Date	Ship Mode	Customer Name	Segment	Country	Market	Sales	Profit	Discount
CA-2012-124891	No	31-07-2020	31-07-2020	Same Day	Rick Hansen	Consumer	United States	US	2309.65	762.18	0
IN-2013-77878	Yes	05-02-2021	07-02-2021	Second Class	Justin Ritter	Corporate	Australia	APAC	3709.40	-288.77	0.1
IN-2013-71249	No	17-10-2021	18-10-2021	First Class	Craig Reiter	Consumer	Australia	APAC	5175.17	919.97	0.1

### 2. Returns Table

Tracks orders that have been returned, along with associated markets.

#### ** Sample Data:**

Returned	Order ID	Market
Yes	MX-2013-168137	LATAM
Yes	US-2011-165316	LATAM
Yes	ES-2013-1525878	EU
Yes	CA-2013-118311	United States


### 3. People Table

Contains details about sales representatives and their respective regions.

#### ** Sample Data:**

Person	Region
Anna Andreadi	Central
Chuck Magee	South
Kelly Williams	East
Matt Collister	West
Deborah Brumfield	Africa

*** 

## Problem Statements Solved with Steps
1. Key Performance Indicators (KPIs)

**Objective:** Calculate and display Total Sales, Total Profit, Total Quantity, Number of Orders, and Profit Margin dynamically.

**Steps:**

1.Import the Orders Table into Excel using Power Query.
2.Create calculated columns:
 ```Profit Margin = Profit / Sales.```

Profit Margin = Profit / Sales

Total Orders = Count of Order ID

Use Excel formulas:

Total Sales = SUM(Sales)

Total Profit = SUM(Profit)

Total Quantity = SUM(Quantity)

Build a dynamic KPI table with symbols for better visualization.

📊 Example Output:

Total Sales: ₹1,26,42,501.91

Total Profit: ₹14,67,457.29

Total Quantity: 1,78,312

No of Orders: 51,290

Profitability: 11.61%

2. Sales and Profit Analysis

Objective: Visualize sales and profit trends over time to identify patterns.

Steps:

Create a Pivot Table with Order Date grouped by Year and Month.

Add Sales and Profit as values.

Create a Line Chart for trends.

Apply slicers for filtering (Category, Market, Region).

3. Category-Wise Profit

Objective: Analyze profitability across product categories.

Steps:

Pivot Table with Category as rows, Profit as values.

Sort by descending Profit.

Create a Bar Chart for visualization.

4. Segment-Wise Sales Share (%)

Objective: Display the proportion of sales by customer segment.

Steps:

Pivot Table with Segment as rows, Sales as values.

Calculate percentage share:
Sales % = Sales / Total Sales * 100

Create Pie/Donut Chart with dynamic labels.

5. Sales by Country

Objective: Analyze sales performance by country.

Steps:

Pivot Table with Country as rows, Sales as values.

Sort in descending order.

Apply conditional formatting (Heatmap).

6. Top 5 Subcategories

Objective: Identify top 5 performing subcategories.

Steps:

Pivot Table with Sub-Category as rows, Sales as values.

Sort descending by Sales.

Filter top 5 subcategories.

Use a Column Chart for visualization.

✨ Dynamic Features

Dynamic Charts – update in real-time with slicers.

Power Query Integration – automated data cleaning & transformation.

KPI Table – highlights critical metrics at a glance.

🔮 Next Steps for Extension

Return Analysis by market/category.

Top & Bottom Customers.

Market-Wise Comparisons.

Product Contribution Analysis.

📈 Significance

This dashboard empowers retail businesses to:
✔ Track performance through KPIs.
✔ Understand category, segment, and geographic trends.
✔ Make data-driven decisions to optimize operations.

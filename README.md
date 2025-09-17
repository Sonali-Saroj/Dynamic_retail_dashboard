# 🛍️ Dynamic Retail Dashboard in Excel  

## 📌 Overview  
The **Dynamic Retail Dashboard** is an interactive and data-driven tool built in **Excel** to visualize and analyze retail data.  
It connects to datasets hosted on GitHub, uses **Power Query** for data transformation, and presents insights through dynamic charts and KPIs.  

This dashboard solves key business questions and enables **data-driven decision-making**.  

---

## 📊 Datasets Used  

### **1. Orders Table**  
Contains details of customer orders, including product, shipping, and financial metrics.  

**Sample Data:**  

| Order ID       | Returned | Order Date | Ship Date | Ship Mode   | Customer Name | Segment   | Country       | Market | Sales   |  
|----------------|----------|------------|-----------|-------------|---------------|-----------|---------------|--------|---------|  
| CA-2012-124891 | No       | 31-07-2020 | 31-07-2020| Same Day    | Rick Hansen   | Consumer  | United States | US     | 2309.65 |  
| IN-2013-77878  | Yes      | 05-02-2021 | 07-02-2021| Second Class| Justin Ritter | Corporate | Australia     | APAC   | 3709.40 |  
| IN-2013-71249  | No       | 17-10-2021 | 18-10-2021| First Class | Craig Reiter  | Consumer  | Australia     | APAC   | 5175.17 |  

---

### **2. Returns Table**  
Tracks orders that have been returned, along with associated markets.  

**Sample Data:**  

| Returned | Order ID       | Market        |  
|----------|----------------|---------------|  
| Yes      | MX-2013-168137 | LATAM         |  
| Yes      | US-2011-165316 | LATAM         |  
| Yes      | ES-2013-1525878| EU            |  
| Yes      | CA-2013-118311 | United States |  

---

### **3. People Table**  
Contains details about sales representatives and their respective regions.  

**Sample Data:**  

| Person            | Region  |  
|-------------------|---------|  
| Anna Andreadi     | Central |  
| Chuck Magee       | South   |  
| Kelly Williams    | East    |  
| Matt Collister    | West    |  
| Deborah Brumfield | Africa  |  

---

## 1. Key Performance Indicators (KPIs)  

**Objective:** Calculate and display **Total Sales, Total Profit, Total Quantity, Number of Orders, and Profit Margin** dynamically.  

**Steps:**  

1. Import the **Orders Table** into Excel using Power Query.  
2. Create calculated columns for:  
   - `Profit Margin = Profit / Sales`  
   - `Total Orders = Count of Order ID`  
3. Use Excel formulas to calculate:  
   - `Total Sales = SUM(Sales)`  
   - `Total Profit = SUM(Profit)`  
   - `Total Quantity = SUM(Quantity)`  
4. Build a dynamic KPI table and use symbols to enhance visual appeal.  

<img width="933" height="137" alt="image" src="https://github.com/user-attachments/assets/7bca3e0f-41cc-43b6-8778-ccf803531bb5" />

---

## 2. Sales and Profit Analysis  

**Objective:** Visualize sales and profit trends over time to identify patterns.  

**Steps:**  

1. Create a **Pivot Table** with `Order Date` grouped by Year and Month.  
2. Add `Sales` and `Profit` as values.  
3. Create a **Line Chart** to display trends for Sales and Profit.  
4. Apply **Slicers** to filter by category, market, or region dynamically.  



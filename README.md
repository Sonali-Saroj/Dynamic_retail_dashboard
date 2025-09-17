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

## Problem Statements Solved with Steps  

### **1. Key Performance Indicators (KPIs)**  
> **Objective:** Calculate and display **Total Sales, Total Profit, Total Quantity, Number of Orders, and Profit Margin** dynamically.  

**Steps:**  
1. Import the **Orders Table** into Excel using Power Query.  
2. Create calculated columns:  
   ```excel
   Profit Margin = Profit / Sales
   Total Orders = COUNT(Order ID)

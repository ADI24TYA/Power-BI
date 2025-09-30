# 📊 Super-Store Sales Dashboard (Power BI)

## 🔎 Project Overview
This project is an **interactive Power BI dashboard** built on Superstore sales data.  
The main objective is to analyze **sales performance, profit trends, shipping costs, and customer behavior** to uncover actionable business insights.

---

## 📂 Data Modeling
A **Star Schema** was designed for efficient data analysis:
- **Fact Table:** Orders Fact (Sales, Profit, Quantity, Shipping Cost, Discount)
- **Dimension Tables:** Date, Customer, Product, Return, Ship Mode

This modeling approach simplifies DAX calculations and supports better filtering/slicing.

---

## 📈 Dashboard Features
### 🔹 KPIs
- **Avg Shipping Cost**  
- **Total Profit**  
- **Total Sales**  
- **Profit Margin %**  
- **Total Orders**

### 🔹 Visuals
- **Monthly Sales Analysis:** Line chart tracking sales over time.  
- **Sales by Region:** Map visualization highlighting geographical performance.  
- **Sales/Profit by Category:** Bar chart with profit overlay.  
- **Sub-Category Analysis:** Horizontal bar chart for granular product insights.  
- **Sales by Ship Mode:** Pie chart showing distribution across delivery methods.

### 🔹 Filters & Slicers
- **Year Filter:** 2012, 2013, 2014, 2015  
- **Customer Segment Filter:** Consumer, Corporate, Home Office  

---

## 🧮 DAX Measures
- `Total Sales = SUM(SalesFact[Sales])`
- `Total Profit = SUM(SalesFact[Profit])`
- `Profit Margin % = DIVIDE([Total Profit], [Total Sales])`
- `Avg Shipping Cost = AVERAGE(SalesFact[ShippingCost])`
- `Total Orders = COUNTROWS(SalesFact)`

---

## 💡 Key Insights
- Technology generates the highest profit, while furniture has lower profitability despite high sales.  
- Standard Class shipping contributes the largest share of sales.  
- Certain regions outperform others, highlighting geographical opportunities.  
- Customer segments show different spending behaviors, useful for targeted strategies.  

---

## 🚀 How to Use
1. Open the `.pbix` file in **Power BI Desktop**.  
2. Explore the dashboard using slicers and filters.  
3. Drill down into category, region, or ship mode for deeper insights.  

---

## 📌 Conclusion
This dashboard provides a **comprehensive view of Superstore’s performance**, making it easier to track KPIs, identify trends, and support data-driven decision-making.  

---

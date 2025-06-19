
# 🧾 Retail Sales Performance Dashboard
📊 *A Power BI Dashboard for Strategic Retail Insights*  
🗓 *Data Period: Jan 2022 – Jan 2024*

## 🧠 Overview
This project presents an interactive, multi-page Power BI dashboard built using Walmart retail sales data. It is designed to help **executives, analysts, and decision-makers** monitor performance across sales, inventory, product categories, and regions.

The dashboard turns raw data into actionable insights that support strategic planning, sales optimization, inventory control, and category management.

## 🎯 Objectives
- Track sales and inventory trends over time  
- Identify top-selling products and high-performing regions  
- Evaluate category-wise profitability  
- Optimize inventory and reduce stock surplus  
- Enable export-ready reporting for strategic reviews

## 📂 Dataset
- **Source:** `Walmart_Retail_Data.csv`  
- **Time Period:** Jan 2022 – Jan 2024  
- **Fields:** Date, Store ID, Product ID, Category, Region, Units Sold, Inventory Level, Price, Discount, Competitor Pricing, Holiday/Promotion flag

## 🛠 Tools & Techniques
- Power BI Desktop  
- Power Query for data cleaning  
- DAX for KPIs & calculations  
- Slicers & navigation buttons for interactivity  
- Matrix, donut, scatter, bar, and time-series visualizations

## 📊 Dashboard Pages & Visuals

### 1. Inventory & Sales Analysis
- **Line Chart:** Inventory vs Units Sold (Time Series)
- **Scatter Plot:** Product-wise Inventory vs Sales
- **Matrix:** Units Sold by Category & Region
- **Donut Chart:** Sales Distribution by Region  
🔍 *Insight:* Seasonal inventory alignment, stock surplus, stable grocery sales

### 2. Sales Performance Overview
- **KPI Cards:** Net Profit, Gross Profit, Profit Margin
- **Line Chart:** Total Sales Value trend
- **Pie & Column Charts:** Sales/Profit by Category & Region  
🔍 *Insight:* Strong profitability in Furniture, high sales in East/South regions

### 3. Product Insights
- **KPI Cards:** Avg Sales/Product, Top Product, Top Category
- **Bar Chart:** Top Products by Sales
- **Donut Chart:** Category-wise Sales Share
- **Line Chart:** Regional Sales Trends  
🔍 *Insight:* Product `P0020` is the top-seller; Electronics leads in revenue

### 4. Detailed Sales & Profit Table
- **Matrix Table:** Net Profit & Sales by Region/Category
- **Stacked Bar Chart:** Sales vs Profit by Region  
🔍 *Insight:* Toys & Clothing deliver high profit margins; groceries perform steadily

## 📸 Dashboard Preview

### 📊 Main Overview
![Main Page](main-page.png)

### 📦 Inventory & Sales Analysis
![Inventory and Sales](Inventory%20and%20Sales%20Analysis.png)

### 💰 Sales Performance
![Sales Performance](Sales%20Performance.png)

### 🧩 Product Insights
![Product Insights](Product%20Insights.png)

### 📋 Detailed Profit Breakdown
![Detailed Breakdown](Detailed%20Sales%20%26%20Profit%20Breakdown.png)

## 🧮 DAX Example
```DAX
Net Profit =
SUMX(Retail_updateddata,
    [Units Sold] * [Price]
    - ([Units Sold] * [Price] * 0.6)
    - ([Units Sold] * [Price] * [Discount] / 100)
)
```

## 🔍 Key Takeaways
- **Sales vs Inventory:** Closely aligned trends; optimize stock to reduce loss  
- **Top Products & Regions:** Electronics & Groceries dominate; East/South perform best  
- **Profitability:** Toys, Clothing, and Furniture offer highest margins  
- **Business Value:** Empowers retailers to make **data-driven decisions** across operations

## 👥 Contributors
- Abu Saleh  
- Baalqasim Alshehri  
- Ali Al-Fatlawi  
- Professor: Qing Zhang  
- Gannon University – *Business Intelligence Course*

## 🏁 Conclusion
This project showcases the power of **Power BI and DAX** to transform complex datasets into dynamic dashboards that support **real-world retail strategies**. From tracking inventory and analyzing profitability to identifying top performers, this dashboard delivers deep, executive-level insight.

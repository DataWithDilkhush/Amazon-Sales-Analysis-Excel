# Amazon-Sales-Analysis-Excel
# 🛒 Amazon Sales Performance Dashboard — Excel

[![Excel](https://img.shields.io/badge/Built%20with-Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://www.microsoft.com/excel)
[![Pivot Table](https://img.shields.io/badge/Pivot%20Tables-FF6B35?style=for-the-badge&logo=microsoftexcel&logoColor=white)]()
[![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

---

## 🖼️ Dashboard Preview

![Amazon Sales Dashboard](https://github.com/DataWithDilkhush/Amazon-Sales-Analysis-Excel/blob/main/Amazon%20Sales%20Dashboard%20Image/Amazon%20Sales%20Dashboard.png)

> *A dynamic Excel dashboard featuring KPI cards, category-wise revenue breakdown, country analysis, monthly trends, order status distribution, and top product rankings — all powered by Pivot Tables and Excel formulas.*

---

## 📌 Project Overview

The **Amazon Sales Performance Dashboard** is a complete end-to-end data analysis project built entirely in **Microsoft Excel**. This project simulates a real-world e-commerce analytics scenario — analyzing 2 years of Amazon sales data across 6 product categories, 5 countries, 50 products, and 10 brands.

This dashboard helps **e-commerce managers and business analysts** to:
- 💰 Track **total revenue, orders, and average order value** at a glance
- 📦 Compare **category-wise performance** — Electronics vs Books vs Clothing
- 🌍 Analyze **country-wise sales contribution** across 5 countries
- 📈 Spot **monthly revenue trends** and seasonal patterns over 2 years
- 🚚 Monitor **order status** — Delivered, Shipped, Pending, Cancelled, Returned
- 💳 Understand **payment method preferences** of customers

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Complete dashboard creation |
| **Pivot Tables** | Data summarization and aggregation |
| **Excel Charts** | Bar charts, pie charts, line graphs |
| **Excel Formulas** | KPI calculations — SUM, COUNTIF, AVERAGEIF, VLOOKUP |
| **Data Validation** | Interactive dropdown filters |
| **Conditional Formatting** | Color-coded KPI highlights |

---

## 📂 Data Source

> 🔗 **Dataset sourced from [Kaggle](https://www.kaggle.com/datasets)** — publicly available Amazon e-commerce sales dataset, cleaned and structured for Excel analysis.

| Property | Detail |
|---|---|
| **Source** | Kaggle (Public Dataset) |
| **Files** | `Amazon_Sales_Data.xlsx` (raw) + `Amazon_Dashboard.xlsx` (dashboard) |
| **Total Records** | 39,966 orders |
| **Time Period** | January 2023 – December 2024 (2 full years) |
| **Sheets in Raw Data** | Order_date, Products, Customers, Orders |
| **Sheets in Dashboard** | Dashboard, Pivot Table, Amazon |

---

## 📋 Dataset Description

### Raw Data — `Amazon_Sales_Data.xlsx`

| Sheet | Description |
|---|---|
| **Orders** | Main fact table — all 39,966 order records |
| **Products** | 50 unique products with Category and Brand |
| **Customers** | 27,484 unique customers with City, State, Country |
| **Order_date** | Date dimension — Year, Quarter, Month, Day |

### Key Columns in Orders Sheet

| Column | Description |
|---|---|
| OrderID | Unique order identifier |
| OrderDate | Date of purchase |
| CustomerID / CustomerName | Customer details |
| ProductName / Category / Brand | Product information |
| Quantity | Units purchased |
| UnitPrice | Price per unit ($) |
| GrossRevenue | Quantity × UnitPrice |
| DiscountAmount | Discount applied |
| NetRevenue | After discount |
| Tax / ShippingCost | Additional charges |
| FinalRevenue | Final amount paid |
| PaymentMethod | Credit Card, Debit Card, UPI, Amazon Pay, etc. |
| OrderStatus | Delivered / Shipped / Pending / Cancelled / Returned |
| City / State / Country | Customer location |
| SellerID | Seller identifier (1,999 unique sellers) |

---

## 📊 Dashboard Walkthrough

### 💼 Business Problem

E-commerce companies like Amazon process thousands of orders daily. Without clear visibility into performance metrics, business managers cannot quickly answer:
- Which product category is driving maximum revenue?
- Which country contributes the most to total sales?
- What percentage of orders are being cancelled or returned?
- How does revenue compare month-over-month across 2 years?
- Which payment method do most customers prefer?

Raw order data in Excel alone cannot answer these questions quickly.

---

### 🎯 Goal of the Dashboard

To build a **single-sheet, interactive Excel dashboard** using **Pivot Tables and Charts** that gives e-commerce analysts a complete view of Amazon sales performance — from overall KPIs down to product-level and country-level breakdowns.

---

![Amazon Sales Dashboard](https://github.com/DataWithDilkhush/Amazon-Sales-Analysis-Excel/blob/main/Amazon%20Sales%20Dashboard%20Image/Amazon%20Dashboard%20Excel.png)

### 🔍 Walkthrough of Key Visuals

#### 1. 💰 KPI Summary Cards (Top Row)
Four headline metrics displayed as bold KPI cards:

| KPI | Value |
|---|---|
| 💰 Total Revenue | **$36.68M** |
| 📦 Total Orders | **39,966** |
| 👥 Unique Customers | **27,484** |
| 🛒 Avg Order Value | **$917.78** |

#### 2. 📊 Revenue by Category — Bar Chart
All 6 categories perform remarkably evenly — showing a well-balanced product portfolio:

| Category | Revenue |
|---|---|
| 🥇 Electronics | $6.21M |
| 🥈 Books | $6.19M |
| 🥉 Toys & Games | $6.15M |
| Home & Kitchen | $6.07M |
| Sports & Outdoors | $6.05M |
| Clothing | $6.02M |

#### 3. 🌍 Revenue by Country — Pie / Bar Chart
United States dominates with 70% of total revenue:

| Country | Revenue | Share |
|---|---|---|
| 🇺🇸 United States | $25.65M | **70%** |
| 🇮🇳 India | $5.61M | 15.3% |
| 🇨🇦 Canada | $2.13M | 5.8% |
| 🇬🇧 United Kingdom | $1.84M | 5.0% |
| 🇦🇺 Australia | $1.46M | 4.0% |

#### 4. 📈 Monthly Revenue Trend — Line Chart
Consistent monthly revenue between **$2.8M – $3.2M** with peak in May ($3.23M). No extreme seasonal spikes — stable, healthy e-commerce performance.

#### 5. 🚚 Order Status Breakdown — Donut Chart

| Status | Count | % |
|---|---|---|
| ✅ Delivered | 29,795 | **74.6%** |
| 📦 Shipped | 6,138 | 15.4% |
| ⏳ Pending | 1,648 | 4.1% |
| ❌ Cancelled | 1,193 | 3.0% |
| 🔄 Returned | 1,192 | 3.0% |

#### 6. 💳 Payment Method Distribution

| Payment Method | Orders |
|---|---|
| 💳 Credit Card | 14,061 (35.2%) |
| 🏧 Debit Card | 8,021 (20.1%) |
| 📱 UPI | 6,000 (15.0%) |
| 🛒 Amazon Pay | 5,929 (14.8%) |
| 🏦 Net Banking | 3,928 (9.8%) |
| 💵 Cash on Delivery | 2,027 (5.1%) |

#### 7. 🏆 Top 5 Products by Revenue

| Rank | Product | Revenue |
|---|---|---|
| 🥇 1 | Dress Shirt | $805,945 |
| 🥈 2 | Memory Card 128GB | $783,553 |
| 🥉 3 | Smartphone Case | $783,259 |
| 4 | Phone Tripod | $779,571 |
| 5 | Action Camera | $777,538 |

---

## 📐 Key Excel Formulas Used

```excel
-- Total Revenue
=SUM(Amazon[NetPayable])

-- Total Unique Customers
=COUNTA(UNIQUE(Amazon[CustomerID]))

-- Average Order Value
=AVERAGE(Amazon[NetPayable])

-- Delivery Rate %
=COUNTIF(Amazon[OrderStatus],"Delivered")/COUNTA(Amazon[OrderID])

-- Revenue by Category (used in Pivot)
=SUMIF(Amazon[Category],B2,Amazon[NetPayable])

-- YoY Revenue Change
=(SUM_2024 - SUM_2023) / SUM_2023
```

---

## 📈 Key Business Insights

| 📌 Metric | 📊 Value |
|---|---|
| 💰 Total Revenue (2 Years) | $36.68M |
| 📅 Period | Jan 2023 – Dec 2024 |
| 📦 Total Orders | 39,966 |
| 👥 Unique Customers | 27,484 |
| 🛍️ Unique Products | 50 |
| 🏷️ Brands | 10 |
| 🏪 Sellers | 1,999 |
| 🛒 Avg Order Value | $917.78 |
| ✅ Delivery Success Rate | **74.6%** |
| ❌ Cancellation Rate | 3.0% |
| 🔄 Return Rate | 3.0% |
| 🌍 Top Country | USA ($25.65M — 70%) |
| 📦 Top Category | Electronics ($6.21M) |
| 🏆 Top Product | Dress Shirt ($805K) |
| 🏷️ Top Brand | ReadMore ($3.83M) |
| 💳 Top Payment | Credit Card (35.2%) |
| 📅 Peak Month | May ($3.23M) |

---

## 💡 Business Insights & Recommendations

**1. 🌍 USA Market Dominance**
United States contributes 70% of revenue — the company should heavily invest in US market retention strategies while growing India (15.3%) which shows strong second-market potential.

**2. ⚖️ Balanced Category Performance**
All 6 categories generate between $6.0M–$6.2M — no single category dominates. This is a sign of a healthy, diversified product portfolio. Strategy: focus on upselling within high-margin categories like Electronics.

**3. 💳 Credit Card Preferred**
35.2% customers prefer Credit Cards — offering EMI options or cashback on credit card payments could boost average order value.

**4. 📦 3% Cancellation + 3% Return Rate**
Combined 6% loss rate is within industry norms, but addressing the top return reasons (size issues for Clothing, defects for Electronics) could recover ~$2.2M annually.

**5. 📈 Consistent Monthly Revenue**
No sharp seasonal peaks — revenue is stable month-over-month. This suggests the business doesn't rely on festive sales alone, which is a positive sign of organic demand.

---

## 🚀 How to Use This Project

### Step 1 — Download Files
```
Click "Code" → "Download ZIP"
OR
git clone https://github.com/DataWithDilkhush/amazon-sales-dashboard-excel.git
```

### Step 2 — Open Raw Data
- Open `dataset/Amazon_Sales_Data.xlsx`
- Explore 4 sheets: Orders, Products, Customers, Order_date

### Step 3 — Open Dashboard
- Open `dashboard/Amazon_Dashboard.xlsx`
- Go to **Dashboard** sheet — all visuals are here
- Use **dropdown filters** to slice by Year, Category, Country

### Step 4 — Explore Pivot Tables
- Go to **Pivot Table** sheet to see raw aggregations
- Refresh pivot: Right-click → **Refresh All**

---

## 🎓 What I Learned Building This

- ✅ Building a **complete Excel dashboard** from raw data to final visuals
- ✅ Creating **Pivot Tables** for multi-dimensional data aggregation
- ✅ Using **SUMIF, COUNTIF, AVERAGEIF** for KPI calculations
- ✅ Designing **professional charts** — bar, line, donut, pie in Excel
- ✅ Applying **Conditional Formatting** for color-coded KPI cards
- ✅ Structuring a **star schema** — fact + dimension tables in Excel
- ✅ Cleaning and transforming **39,966 rows** of raw e-commerce data
- ✅ Deriving **business insights** from data patterns

---

## 🗂️ More Projects

| Project | Tools | Status |
|---|---|---|
| Telesales Performance Dashboard | Power BI + DAX + Excel | ✅ Completed |
| HR Analytics Dashboard | Power BI + Excel | 📅 Coming Soon |
| SQL Sales Analysis | SQL Server / PostgreSQL | 📅 Coming Soon |
| Python EDA Project | Python + Pandas + Matplotlib | 📅 Coming Soon |

---

## ❓ Frequently Asked Questions

**Q1. Where did you get this dataset?**
> Sourced from **Kaggle** — a public data science platform. The raw data was cleaned, structured into dimension/fact tables, and modeled for Excel Pivot analysis.

**Q2. Why Excel and not Power BI for this project?**
> Excel is the most widely used tool in the industry — especially in SMEs, banks, and financial firms. Building a dashboard in Excel demonstrates core data analysis skills without relying on specialized BI tools.

**Q3. What was the biggest challenge?**
> Managing formula references across 39,966 rows without Excel slowing down. Used structured Table references (`Amazon[Column]`) instead of range references to keep formulas dynamic and efficient.

**Q4. How is Avg Order Value calculated?**
> `Avg Order Value = Total NetPayable ÷ Total Orders = $36.68M ÷ 39,966 = $917.78`

**Q5. Why does USA dominate 70% of orders?**
> The dataset is Amazon-focused — Amazon's primary market is USA. The India segment (15.3%) likely represents Amazon.in customers, which aligns with Amazon's strong India growth.

---

## 📬 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/your-profile)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/DataWithDilkhush)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/)

---

## 🛡️ License

Licensed under the [MIT License](LICENSE) — free to use, modify, and share with proper credit.

---

## ⭐ Support

Agar yeh project helpful laga toh **Star** ⭐ zaroor karo!
*Your support motivates me to build more real-world data projects!* 🙏

---

*Made with ❤️ by **Dilkhush** | Aspiring Data Analyst | Excel · Power BI · SQL · Python*

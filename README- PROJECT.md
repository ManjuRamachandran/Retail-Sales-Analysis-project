# 🛒 Retail Store Sales Analysis
### End-to-End Data Analysis | Python · SQL · Power BI · GitHub

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python) ![SQL](https://img.shields.io/badge/SQL-MySQL-orange?logo=mysql) ![PowerBI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi) ![Dataset](https://img.shields.io/badge/Records-9%2C994-green)

---

## 📌 Project Overview

An end-to-end data analysis project on the **US Retail Superstore dataset** covering 9,994 transactions across 4 regions, 3 product categories, and 3 customer segments.

The project follows a complete analyst workflow:
**Python (EDA)** → **SQL (Business Questions)** → **Power BI (Dashboard)**

---

## 📊 Key Metrics

| Metric | Value |
|---|---|
| 💰 Total Sales | $2.30M |
| 📈 Total Profit | $286K |
| 🛍️ Total Orders | 9,994 |
| 🎯 Profit Margin | 12.5% |
| 🏷️ Avg Discount | 15.6% |
| 🌍 Regions | 4 (West, East, Central, South) |

---

## 🗂️ Dataset

**Source:** US Retail Superstore (Kaggle)
**Size:** 9,994 rows · 13 columns · 0 null values · 0 duplicates

| Column | Type | Description |
|---|---|---|
| Ship Mode | Text | Standard / First / Second / Same Day |
| Segment | Text | Consumer / Corporate / Home Office |
| City / State | Text | Geographic location |
| Region | Text | West, East, Central, South |
| Category | Text | Furniture, Office Supplies, Technology |
| Sub-Category | Text | 17 unique sub-categories |
| Sales | Decimal | Revenue per order |
| Quantity | Integer | Items ordered |
| Discount | Decimal | Discount applied (0.0 – 0.8) |
| Profit | Decimal | Net profit (can be negative) |

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Python (Pandas) | Data cleaning & exploratory analysis |
| SQL (MySQL) | Answering 10 business questions |
| Power BI | 3-page interactive dashboard |
| GitHub | Version control & portfolio |

---

## ❓ 10 Business Questions Answered

| # | Question | Key Finding |
|---|---|---|
| Q01 | Which region has the highest sales & profit? | West leads — $725K sales, 14.9% margin |
| Q02 | Which category is most/least profitable? | Technology 17.4% vs Furniture only 2.5% |
| Q03 | Which sub-categories are causing losses? | Tables (-$17,725), Bookcases (-$3,472) |
| Q04 | How does discount affect profit? | 20%+ discounts result in average losses |
| Q05 | Top 10 cities by total sales? | NYC #1 at $256K; Philadelphia top 5 but -$13K profit |
| Q06 | Ship mode preference by segment? | All segments prefer Standard Class (60%+) |
| Q07 | Most profitable sub-categories? | Copiers $55K profit; Paper 43.4% margin |
| Q08 | Which segment contributes most revenue? | Consumer = 50.6% of all sales |
| Q09 | Which states have the highest losses? | Texas -$25,729 on $170K sales |
| Q10 | Does discount drive more quantity? | Correlation = -0.219. No — discounts just kill profit |

---

## 📉 Key Business Insights

- 🟢 **West Region** is the top performer with $725K sales and 14.9% profit margin
- 🔴 **Central Region** has only 7.9% margin — needs urgent investigation
- 🟢 **Technology** is the most profitable category (17.4% margin)
- 🔴 **Furniture** earns only 2.5% margin despite $742K in sales
- 🔴 **Tables sub-category** alone loses **-$17,725** — biggest loss maker
- ⚠️ Discounts above **20% always result in losses** — business should cap at 20%
- 🔴 **Texas** loses -$25,729 despite generating $170K in revenue
- 🟢 **Consumer segment** drives 50.6% of total revenue — most valuable group

---

## 📁 Repository Structure

```
retail-sales-analysis/
│
├── data/
│   └── archive.csv                    # Raw dataset
│
├── sql/
│   ├── 01_region_sales.sql
│   ├── 02_category_profit.sql
│   ├── 03_loss_subcategories.sql
│   ├── 04_discount_impact.sql
│   ├── 05_top_cities.sql
│   ├── 06_shipmode_segment.sql
│   ├── 07_top_subcategories.sql
│   ├── 08_segment_contribution.sql
│   ├── 09_loss_states.sql
│   └── 10_discount_quantity.sql
│
├── python/
│   ├── 01_data_cleaning.py
│   └── 02_analysis.py
│
├── powerbi/
│   ├── dashboard_page1.png            # Sales Overview
│   ├── dashboard_page2.png            # Profitability Analysis
│   ├── dashboard_page3.png            # Customer & Geographic
│   └── retail_dashboard.pbix
│
└── README.md
```

---

## 🖥️ Power BI Dashboard — 3 Pages

### Page 1 — Sales Overview
- 5 Cards: Total Sales, Total Profit, Total Orders, Profit Margin %, Avg Order Value
- Clustered Bar: Sales & Profit by Region
- Donut Chart: Sales by Category
- Horizontal Bar: Top 10 Cities by Sales

### Page 2 — Profitability Analysis
- 3 Cards: Total Profit, Profit Margin %, Profit per Order
- Waterfall Chart: Profit by Sub-Category (RED = loss, GREEN = profit)
- 100% Stacked Bar: Profit Margin by Category
- Scatter Plot: Discount vs Profit (with trend line)

### Page 3 — Customer & Segment Analysis
- 4 Cards: Consumer Sales %, Top Region, Worst Loss State, Avg Discount
- Donut Chart: Sales % by Segment
- 100% Stacked Bar: Ship Mode by Segment
- Bar Chart: Top Loss States by Profit

---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/retail-sales-analysis.git

# 2. Run Python cleaning script
python python/01_data_cleaning.py

# 3. Import archive.csv into MySQL and run SQL files in order

# 4. Open Power BI file
# → Open powerbi/retail_dashboard.pbix in Power BI Desktop
```

---

---

*Dataset: US Retail Superstore · 9,994 Records · 13 Columns · Built with Python · SQL · Power BI*

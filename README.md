<div align="center">

# -- ! Asian Paints Sales Performance Dashboard ! --
### *Interactive Power BI Dashboard for Revenue, Product, Regional & Dealer Analytics*

[![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![DAX](https://img.shields.io/badge/DAX-Measures%20%26%20KPIs-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://learn.microsoft.com/en-us/dax/)
[![Pages](https://img.shields.io/badge/Report-5%20Pages-4CAF50?style=for-the-badge&logo=databricks&logoColor=white)](https://powerbi.microsoft.com/)
[![Domain](https://img.shields.io/badge/Domain-Paints%20%26%20Coatings-E91E63?style=for-the-badge&logo=googleanalytics&logoColor=white)](https://powerbi.microsoft.com/)

<br/>

> *"Every litre sold is a data point — a good dashboard shows where the colour comes from."*

</div>

---

## 📋 Table of Contents

- [📌 Overview](#-overview)
- [🎯 Problem Statement](#-problem-statement)
- [✨ Key Features](#-key-features)
- [🏗️ Project Structure](#️-project-structure)
- [🔄 Project Workflow](#-project-workflow)
- [🏠 Part A — Executive Overview](#-part-a--executive-overview)
- [📍 Part B — Regional Performance](#-part-b--regional-performance)
- [🎨 Part C — Product Analytics](#-part-c--product-analytics)
- [🤝 Part D — Dealer Performance](#-part-d--dealer-performance)
- [📈 Part E — Trends & Forecasting](#-part-e--trends--forecasting)
- [🛠️ Tech Stack](#️-tech-stack)
- [📈 Results & Insights](#-results--insights)
- [🏆 Advantages](#-advantages)
- [📄 License](#-license)
- [👤 Author](#-author)
- [🙏 Acknowledgements](#-acknowledgements)

---

## 📌 Overview

The **Asian Paints Sales Performance Dashboard** is an interactive, five-page **Power BI** report that tracks revenue, profit, orders, products, regions and dealers for a paints business in India. It covers the financial year **April 2023 to March 2024**, shows every value in **₹ Crores**, and compares each KPI with the **previous year (PY)**. The report uses a dark-blue navigation panel, KPI cards with icons, slicers, maps and a reset button on every page.

This project is designed to:
- Track **revenue**, **profit**, **profit margin** and **orders** against the previous year
- Compare performance by **region**, **zone**, **state** and **city**
- Analyze **products** and **categories** by revenue, profit and inventory turnover
- Evaluate **dealers** by revenue, visits and dealer type
- Show **monthly trends**, a **6-month forecast** and an **executive summary**

---

## 🎯 Problem Statement

> **Objective:** Build an interactive dashboard that helps sales and management teams understand where revenue and profit come from, and how they are trending.

Sales data is usually spread across products, regions and dealers. This dashboard brings it together on five linked pages, with a common set of slicers, so any KPI can be drilled down by category, geography or dealer type.

| 📂 Page | 📄 Focus | 🔍 Description |
|---------|----------|----------------|
| Overview | Executive | Headline KPIs, revenue trend, category mix, scorecard |
| Regional Performance | Geography | Region > Zone > State > City revenue, target and margin |
| Product Analytics | Products | Category > Sub Category > Product revenue, profit and stock |
| Dealer Performance | Dealers | Top dealers, dealer types, visits and locations |
| Trends & Forecasting | Outlook | Monthly trends, YTD, YoY growth, forecast and summary |

The goal is to demonstrate **end-to-end BI skills** — from KPI design to drill-down navigation to a polished, consistent report.

---

## ✨ Key Features

| Feature | Description |
|--------|-------------|
| 📑 **5 Report Pages** | Overview, Regional, Product, Dealer, and Trends & Forecasting |
| 🧭 **Side Navigation** | Dark-blue panel with page buttons and a filters section on every page |
| 🔢 **KPI Cards** | Revenue, Profit, Profit Margin %, Orders, Target Achievement, Products, Dealers and more, each with a vs-PY change |
| 📅 **Date Range Filter** | Start and end date selector at the top of each page |
| 🎛️ **Slicers** | Category, Sub Category, Product, Price Tier, Region, Zone, State, City, Dealer Type |
| 🔄 **Reset Button** | Clears all filters in one click |
| 🗺️ **Maps** | Filled map by region and bubble map of dealer locations |
| 🔽 **Drill Hierarchies** | Category > Sub Category > Product and Region > Zone > State > City |
| 🔮 **Forecast** | Revenue forecast for the next 6 months |
| 💡 **Executive Summary** | Four written takeaways on growth, profitability, targets and outlook |

---

## 🏗️ Project Structure

```
📦 asian-paints-dashboard/
│
├── 📄 AsianPaints_Dashboard.pbix   ← Power BI report (data model + 5 pages)
│
└── 📄 README.md                    ← Project documentation
```

---

## 🔄 Project Workflow

```
Raw Sales Data (Orders · Products · Regions · Dealers · Targets)
      │
      ▼
┌─────────────────────────────┐
│   Load & Clean Data         │
└────────────┬────────────────┘
             │
             ▼
┌─────────────────────────────┐
│   Build Data Model & DAX    │  ← Revenue, Profit, Margin, YoY, Achievement
└────────────┬────────────────┘
             │
   ┌─────────┼─────────┬──────────┬───────────┐
   ▼         ▼         ▼          ▼           ▼
┌────────┐┌────────┐┌─────────┐┌────────┐┌─────────┐
│Overview││Regional││ Product ││ Dealer ││ Trends &│
│        ││        ││Analytics││        ││Forecast │
└───┬────┘└───┬────┘└────┬────┘└───┬────┘└────┬────┘
    └─────────┴──────────┴─────────┴──────────┘
                         │
                         ▼
┌─────────────────────────────┐
│  Slicers + Date Range       │
└────────────┬────────────────┘
             │
             ▼
   KPI Cards + Charts Update
             │
             ▼
   Insights for Management ✅
```

---

## 🏠 Part A — Executive Overview

### 📝 1. What does this page show?

<img src="page img/Overview page 1.png">

The **Executive Overview** page answers: *how is the business doing overall, and how does it compare with last year and with target?*

| Visual | Type | Details |
|--------|------|---------|
| 🔢 Total Revenue (₹ Cr) | KPI Card | With change vs PY |
| 🔢 Total Profit (₹ Cr) | KPI Card | With change vs PY |
| 🔢 Profit Margin % | KPI Card | With change in percentage points vs PY |
| 🔢 Total Orders | KPI Card | With change vs PY |
| 🎯 Target Achievement % | KPI Card | With change vs PY |
| 📈 Revenue Trend (Monthly) | Line Chart | Monthly total revenue |
| 📊 Profit, Revenue Target & Achievement % | Combo Chart | Profit and target columns with achievement % line |
| 🟦 Revenue by Category | Treemap | Revenue share of each product category |
| 🗺️ Revenue by Region | Filled Map | Revenue across India |
| 🧾 Executive Scorecard (vs Target) | Table | Revenue achievement %, profit achievement %, profit margin % and revenue growth % by category |

**Filters:** Date Range, Region, Product Category, Dealer Type, State, Zone

---

## 📍 Part B — Regional Performance

### 🔍 2. What does this page show?

<img src="page img/Regional Performance page 2.png">

The **Regional Performance** page answers: *which regions and states bring in the most revenue and the best margins?*

| Visual | Type | Details |
|--------|------|---------|
| 🔢 Revenue, Profit, Target Achievement %, Orders, Profit Margin % | KPI Cards | Each with change vs PY |
| 🗺️ Revenue by Region | Filled Map | Revenue intensity by region |
| 🏆 Revenue by Region (Ranking) | Table | Region rank, revenue and % of total |
| 🏆 Revenue by State (Top 10) | Table | State rank, revenue and % of total |
| 📊 Revenue vs Target by Region | Combo Chart | Profit, revenue target and revenue achievement % by zone |
| 🟥 Profit Margin % Heatmap | Matrix | State by Region, colour-scaled |

**Filters:** Date Range, Region, Zone, State, City

---

## 🎨 Part C — Product Analytics
 
### 🔍 3. What does this page show?


<img src="page img/Product Analytics page 3.png">

The **Product Analytics** page answers: *which categories and products drive revenue and profit, and how fast does stock move?*

| Visual | Type | Details |
|--------|------|---------|
| 🔢 Revenue, Profit, Profit Margin % | KPI Cards | Each with change vs PY |
| 🔢 Total Products | KPI Card | Count across all categories |
| 🔢 Avg Closing Stock | KPI Card | With change vs PY |
| 📊 Product Revenue (Top 10) | Bar Chart | Top 10 products by revenue |
| 📊 Product Profit (Top 10) | Bar Chart | Top 10 products by profit |
| 🍩 Product Revenue by Category | Donut + Table | Revenue and share of each category |
| 📊 Inventory Turnover by Category | Column Chart | Turnover for each category |
| 🧾 Top Products by Revenue | Table | Rank, product, category, revenue and profit margin % |
| 🔵 Revenue vs Profit Scatter | Scatter | Total revenue against total profit for each product |

**Filters:** Date Range, Category, Sub Category, Product, Price Tier

---

## 🤝 Part D — Dealer Performance

### 🔍 4. What does this page show?

<img src="page img/Dealer Performance page 4.png">

The **Dealer Performance** page answers: *which dealers and cities perform best, and how active is the dealer network?*

| Visual | Type | Details |
|--------|------|---------|
| 🔢 Total Dealer Revenue, Profit | KPI Cards | Each with change vs PY |
| 🔢 Total Dealers, Total Orders | KPI Cards | Each with change vs PY |
| 🔢 Avg Revenue per Dealer, Avg Revenue per Visit | KPI Cards | Each with change vs PY |
| 🏆 Top 10 Dealers by Revenue | Table | Rank, dealer name and revenue |
| 📊 Revenue per Dealer (Distribution) | Column Chart | Number of dealers in each revenue band |
| 📈 Dealer Visits Trend (Monthly) | Line Chart | Total orders and total visits by month |
| 🍩 Dealer Visits by Type | Donut + Table | Sales Visit, Training, Collection and Demo visits |
| 📊 Revenue by Dealer Type | Combo Chart | Revenue and profit with profit margin % line for Distributor, Retail, Silver, Premium and Gold |
| 🗺️ Dealer Location Map | Bubble Map | Dealer locations across India |
| 🏙️ Top 5 Cities by Dealer Revenue | Bar Chart | Highest revenue cities |

**Filters:** Date Range, Dealer Type, Region, Zone, State, City

---

## 📈 Part E — Trends & Forecasting

### 🔍 5. What does this page show?

<img src="page img/Trends & Forecasting page 5.png">


The **Trends & Forecasting** page answers: *how are revenue and profit moving over time, and what is the outlook?*

| Visual | Type | Details |
|--------|------|---------|
| 🔢 YTD Revenue, YTD Profit | KPI Cards | Each with change vs PY |
| 🔢 Profit Margin %, Total Orders | KPI Cards | Each with change vs PY |
| 🔢 YoY Revenue Growth, YoY Profit Growth | KPI Cards | Growth % with change in ₹ Cr |
| 📈 Revenue Trend (Monthly) | Line Chart | Current year compared with PY |
| 📈 Profit Trend (Monthly) | Line Chart | Profit and revenue by month |
| 📈 YTD Revenue (Cumulative) | Area Chart | Cumulative revenue against PY |
| 🔮 Revenue Forecast (Next 6 Months) | Line Chart | Forecast of monthly revenue |
| 🧾 Executive Scorecard (vs Target) | Table | Actual, target, achievement % and change vs PY for revenue, margin, profit and orders |
| 📉 YoY Growth Trend (%) | Line Chart | Revenue growth % and profit growth % by month |
| 💡 Executive Summary | Text Panel | Four takeaways: revenue growth, profitability, targets, outlook |

**Filters:** Date Range, Compare With (Previous Year), Region, Zone, Category, Dealer Type

---

## 🛠️ Tech Stack

| Tool | Version | Purpose |
|------|---------|---------|
| 📊 **Power BI Desktop** | Latest | Report authoring and data modeling |
| 🧮 **DAX** | Built-in | Measures such as Total Revenue, Total Profit, Profit Margin %, YoY Growth, Target Achievement %, YTD |
| 🗺️ **Map Visuals** | Built-in | Filled map and bubble map |
| 🔮 **Forecasting** | Built-in | 6-month revenue forecast |
| 🧭 **Navigation & Buttons** | Built-in | Page navigation, filter reset |
| 🖼️ **Custom Icons & Images** | PNG | Logo, KPI icons and decorative images |

---

## 📈 Results & Insights

The dashboard shows the following for the period **4 April 2023 to 31 March 2024** (data as on 31-Dec-2025):

- 💰 **Revenue:** ₹175.2 Cr, up 1.6% from ₹172.4 Cr in the previous year
- 📈 **Profit:** ₹57.0 Cr, up 2.0% from ₹55.9 Cr; profit margin is 32.56%
- 🧾 **Orders:** About 75K, up 1.3% from 73,914
- 📍 **Regions:** West leads with ₹42.93 Cr (24.50%), followed by Central, East, North and South
- 🏔️ **States:** Mizoram (₹14.08 Cr), Himachal Pradesh (₹12.82 Cr) and West Bengal (₹10.62 Cr) top the state ranking
- 🎨 **Categories:** Putty (₹28.82 Cr) and Interior Emulsion (₹28.46 Cr) lead; Waterproofing is the lowest (₹20.42 Cr)
- 📦 **Products:** 501 products across 8 categories; all earn nearly the same margin (about 32.5%), so **revenue is the main driver of profit** (R² = 0.96)
- 🤝 **Dealers:** About 5K dealers; Dewan Inc (₹18.53 Cr) and Kala LLC (₹18.51 Cr) are the top two
- 🏙️ **Cities:** Jamnagar, Ghaziabad and Burhanpur lead by dealer revenue
- 🔮 **Outlook:** YTD revenue ₹176.7 Cr (up 1.6%); forecast shows about ₹15 Cr per month over the next 6 months, a flat outlook

---

## 🏆 Advantages

| Advantage | Detail |
|-----------|--------|
| 🎓 **Complete Sales View** | Overview, regions, products, dealers and trends in one report |
| 🎛️ **Flexible Filtering** | Date range plus category, region, zone, state, city and dealer type slicers |
| 🔽 **Drill Down** | Category > Sub Category > Product and Region > Zone > State > City |
| 📊 **Always vs PY** | Every KPI shows its change against the previous year |
| 🎯 **Target Tracking** | Scorecards compare actuals with targets |
| 🔮 **Forward Looking** | 6-month revenue forecast and an executive summary |
| 🔄 **One-click Reset** | Clears all filters on every page |
| 🖥️ **Consistent Design** | Same header, navigation panel and footer on all five pages |

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for full details.

```
MIT License — Free to use, modify, and distribute with attribution.
```

---

## 👤 Author

<div align="center">

### Divyesh Jadav

[![GitHub](https://img.shields.io/badge/GitHub-yourhandle-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/yourhandle)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/your-profile/)

> *"Every dashboard starts with a question — and ends with a better decision."*

**🎓 Role:** Data Analyst | Power BI Enthusiast \
**📍 Location:** India\
**🛠️ Skills:** Power BI · DAX · Data Modeling · Dashboard Design · Data Visualization

</div>

---

## 🙏 Acknowledgements

Special thanks to the following resources and communities that made this project possible:

- 📚 [Power BI Documentation](https://learn.microsoft.com/en-us/power-bi/) — Official Power BI reference
- 🧮 [DAX Guide](https://dax.guide/) — Complete DAX function reference
- 🎨 [Power BI Report Design Guidance](https://learn.microsoft.com/en-us/power-bi/guidance/) — Layout and design best practices
- 🖥️ [Microsoft Learn — Power BI](https://learn.microsoft.com/en-us/training/powerplatform/power-bi) — Beginner to advanced courses
- 💬 [Power BI Community](https://community.fabric.microsoft.com/) — Problem-solving support
- 📖 [Kaggle Learn](https://www.kaggle.com/learn) — Data and analytics courses

---

<div align="center">

---

*Made with ❤️ and ☕ — Last updated: 8 November, 2026*

</div>

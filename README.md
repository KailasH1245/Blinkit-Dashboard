# 🛒 Blinkit Grocery Sales & Outlet Performance Analytics

[![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-F2C811?style=flat&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Excel](https://img.shields.io/badge/Microsoft%20Excel-Data%20Source-217346?style=flat&logo=microsoft-excel&logoColor=white)](https://www.microsoft.com/en-us/microsoft-365/excel)
[![DAX](https://img.shields.io/badge/DAX-KPI%20Modeling-0078D4?style=flat&logo=microsoft&logoColor=white)](https://learn.microsoft.com/en-us/dax/)

An end-to-end quick-commerce retail analytics solution built on **Blinkit's grocery sales dataset**. This project transforms raw outlet and product transaction records from Excel into an interactive **Power BI executive dashboard** backed by **Power Query data cleaning** and dynamic **DAX KPIs** to evaluate outlet performance, product category demand, and customer ratings.

---

## 🎯 Business Problem & Objectives
Quick-commerce grocery platforms must optimize inventory mix and outlet footprint across diverse urban tiers while maintaining high customer ratings. Using Blinkit's historical outlet and product sales records, this project answers four core business questions:
1. **Core Retail KPIs:** What are the overall Total Sales, Average Sales per transaction, Number of Items sold, and Average Customer Rating?
2. **Outlet Footprint & Location Tiers:** How does revenue performance compare across **Tier 1, Tier 2, and Tier 3** cities, as well as different outlet sizes and outlet types?
3. **Product & Fat Content Preferences:** Which product categories and fat content segments (`Low Fat` vs. `Regular`) drive the highest revenue share?
4. **Outlet Expansion Trajectory:** How has outlet establishment growth over the years influenced total sales volume?

---

## 📊 Key Analytical Dimensions

| Focus Area | Tracked Metrics & Breakdowns | Business Purpose |
| :--- | :--- | :--- |
| **Core Sales KPIs** | `Total Sales`, `Average Sales`, `Number of Items`, `Average Rating` | Monitors top-line revenue, order basket value, item volume, and customer satisfaction in real time. |
| **Outlet Tier & Size** | `Tier 1` vs. `Tier 2` vs. `Tier 3` & `Small` / `Medium` / `High` | Evaluates how store scale and city tier impact total revenue generation and customer ratings. |
| **Outlet Format** | `Supermarket Type 1–3` & `Grocery Store` | Compares sales efficiency across different physical and dark-store outlet formats. |
| **Product & Fat Mix** | Top Item Categories & `Low Fat` vs. `Regular` | Identifies high-revenue grocery categories and shopper dietary preferences for inventory planning. |
| **Establishment Trend** | Yearly Outlet Establishment (`Outlet Establishment Year`) | Tracks historical store expansion waves and their ongoing revenue contribution. |

---

## 🏗️ Data Pipeline & Architecture

```text
┌─────────────────────────────┐     ┌──────────────────────────────────┐     ┌──────────────────────────────┐
│  Blinkit Grocery Data.xlsx  │ ──► │  Power Query & DAX Data Model    │ ──► │  Interactive Power BI Report │
│ • Raw Outlet & Item Records │     │ • Standardized Fat Content Labels│     │ • Executive KPI Cards        │
│ • Sales, Ratings & Tier Data│     │ • Dynamic KPI Measures (DAX)     │     │ • Tier, Size & Format Splits │
└─────────────────────────────┘     │ • Multi-Attribute Slicers        │     │ • Category & Trend Visuals   │
                                    └──────────────────────────────────┘     └──────────────────────────────┘

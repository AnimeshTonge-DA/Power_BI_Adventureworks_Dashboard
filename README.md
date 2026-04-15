
# 📊 AdventureWorks Sales Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)


A fully interactive **business intelligence dashboard** built in Power BI for **AdventureWorks Shop** — a fictional retail company. This project demonstrates end-to-end BI development: data modeling, DAX measures, and visual storytelling.

---

## 🖼️ Dashboard Preview

<img width="1282" height="718" alt="Dashboard Meaven" src="https://github.com/user-attachments/assets/c9bbe3fb-56de-4d0e-a26d-369e45ea33ea" />

---

## 📌 Key Metrics

| Metric | Value |
|---|---|
| Total Revenue | ₹ 24.9M |
| Total Profit | ₹ 10.5M |
| Total Orders | 25.2K |
| Return Rate | 2.2% |

---

## 📈 Features

- **Revenue Trend** — Monthly revenue line chart with trend line (Jan 2020 – Jan 2022)
- **Orders by Category** — Horizontal bar chart across Accessories, Bikes, and Clothing
- **Top 10 Products Table** — Ranked by orders with revenue and return rate indicators
- **Monthly KPI Cards** — Revenue, Orders, and Returns with MoM comparisons
- **Most Ordered & Most Returned** — Product type callouts (Tires and Tubes / Shorts)
- **Date Range Slicer** — Dynamic filtering across the full timeline

---

## 🗂️ Dataset

This project uses the **AdventureWorks** sample dataset, adapted for Power BI. It includes:

- AdventureWorks Calendar Lookup
- AdventureWorks Customer Lookup
- AdventureWorks Product Categories
- AdventureWorks Product
- AdventureWorks Subcategories
- AdventureWorks Returns data
- Sales transactions data
- AdventureWorks Territory Lookup

---

## 🛠️ Tools & Technologies

- **Power BI Desktop** — report development
- **DAX** — custom measures (YTD, MoM %, return rate)
- **Power Query** — data transformation and cleaning
- **AdventureWorks Dataset** — source data

---

## 📐 DAX Measures Used

```dax
Total Revenue = SUMX(Sales, Sales[OrderQuantity] * RELATED(Products[ProductPrice]))

Total Profit = [Total Revenue] - [Total Cost]

Return Rate = DIVIDE([Total Returns], [Total Orders], 0)

MoM Revenue % = DIVIDE([Total Revenue] - [Last Month Revenue], [Last Month Revenue], 0)
```

---

## 🚀 How to Use

1. Clone or download this repository
2. Open `AdventureWorks_Dashboard.pbix` in **Power BI Desktop**
3. Refresh the data source if prompted
4. Interact using the date slicer and category filters

---

## 🧠 What I Learned

- Building star-schema data models in Power BI
- Writing DAX for time intelligence (MoM, YTD)
- Designing executive-level dashboards for non-technical stakeholders
- Using conditional formatting to highlight KPI thresholds

---

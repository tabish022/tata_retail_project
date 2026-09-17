# Tata Group — Data Visualisation Job Simulation
### Online Retail Sales Dashboard (Power BI)

[![Forage](https://img.shields.io/badge/Forage-Job%20Simulation-1f883d?style=for-the-badge)](https://www.theforage.com/simulations/tata/data-visualisation-p5xo)
[![Certificate](https://img.shields.io/badge/View-Completion%20Certificate-blue?style=for-the-badge)](https://www.theforage.com/completion-certificates/ifobHAoMjQs9s6bKS/MyXvBcppsW2FkNYCX_ifobHAoMjQs9s6bKS_6aa921d527fafa67962ced8b_1789655290891_completion_certificate.pdf)
[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](./bi_tata_retail_dashboard.pbix)

## 📌 Overview

This project was completed as part of **Tata Group's Data Visualisation Job Simulation on Forage**, where I stepped into the role of a data analyst intern at **Tata Insights and Quants (Tata iQ)**. The task was to translate raw e-commerce transaction data into clear, decision-ready visualizations for two stakeholders — the **CEO** and the **CMO** — using Power BI.

🎓 **Certificate of completion:** [View certificate](https://www.theforage.com/completion-certificates/ifobHAoMjQs9s6bKS/MyXvBcppsW2FkNYCX_ifobHAoMjQs9s6bKS_6aa921d527fafa67962ced8b_1789655290891_completion_certificate.pdf)

---

## 🧾 Scenario

Tata iQ works with businesses to turn raw data into visual stories that drive decisions. For this simulation, I was given an online retail transaction dataset and asked to:
1. Frame the business questions a CEO and CMO would realistically ask.
2. Clean and prepare the raw dataset for analysis.
3. Build Power BI visuals answering those questions.
4. Present the findings back to leadership in a short video.

---

## 📂 Repository contents

| File | Description |
|---|---|
| `bi_tata_retail_dashboard.pbix` | Final Power BI dashboard file containing all visuals, slicers, and KPI cards |
| `online_retail_dataset.xlsx` | Original, raw dataset (541,909 transaction rows, Dec 2010–Dec 2011, 38 countries) |
| `cleaned_retail_dataset.xlsx` | Cleaned dataset used to build the dashboard |
| `icons/` | Icon assets used for dashboard styling |

---

## 🧹 Data cleaning process

The raw dataset required several cleaning steps before analysis:

- **Removed duplicate rows** to avoid double-counting transactions.
- **Separated cancelled orders** (invoices prefixed with "C", ~9,300 rows) from genuine sales.
- **Removed invalid rows**: negative quantities not tied to a cancellation (~1,300 rows) and zero/negative unit prices (~2,500 rows), which were data-entry errors or write-offs.
- **Handled missing CustomerIDs** (~25% of rows, mostly guest checkouts) — retained for revenue/product analysis, excluded from customer-level analysis.
- **Standardized text fields** — trimmed whitespace, fixed inconsistent country names and mismatched product code casing.
- **Added a calculated `Revenue` field** (`Quantity × Unit Price`) used across every visual.

---

## 📊 Dashboard contents

Built in Power BI, the dashboard answers four core stakeholder questions:

1. **Monthly revenue trend (2011)** — line chart, for the CEO, to reveal seasonality and plan around peak periods.
2. **Revenue & quantity by country (Top 10, excl. UK)** — clustered bar chart, for the CMO, to identify strongest international markets.
3. **Top 10 customers by revenue** — column chart, for the CMO, to assess customer concentration and retention priorities.
4. **Units sold by country (excl. UK)** — map visual, for the CEO, to support expansion strategy.

Additional visuals: orders by day of week, and top-selling products, to round out the analysis beyond the minimum requirements.

The dashboard also includes a date-range slicer and country slicer for interactive filtering.

---

## 🛠️ Tools used

- **Power BI Desktop** — dashboard build, DAX measures, data modeling
- **Microsoft Excel** — initial data inspection and cleaning
- **Power Query** — data transformation

---

## 🎯 Key insights delivered

- 2011 total revenue: **~£9.85M**, peaking in **November** at ~£1.5M.
- The **UK accounts for ~84.6%** of total revenue; **Netherlands and Ireland** are the strongest markets outside the UK.
- The **top 10 customers** account for **~14.4%** of total revenue — a meaningful but not majority concentration.
- International demand is currently concentrated in **Western Europe**, informing where expansion efforts could focus first.

---

## 📝 About this simulation

This project was completed via [Forage](https://www.theforage.com/), a platform offering free, self-paced job simulations from real companies. It reflects simulated project work designed to build and demonstrate practical data analytics and visualization skills — not paid client or employment work.

---

## 🙋 About Me

Built by **Tabish Afzal** as a hands-on Power BI project to practice the real workflow of a Data Analyst end to end: auditing raw transactional data for quality issues, cleaning and structuring it, and building stakeholder-facing dashboards that turn 540K+ raw retail records into business insights for leadership.

· 🔗 [LinkedIn](https://www.linkedin.com/in/tabish-afzal/) · 💼 [Portfolio](https://github.com/tabish022)

---

⭐ If you found this useful, consider starring the repo!

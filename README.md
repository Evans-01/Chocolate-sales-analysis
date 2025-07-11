# 🍫 Chocolate Works - Sales Dashboard 📊

This project provides an interactive Power BI dashboard that visualizes sales performance, profit analytics, shipment volume, and product distribution across regions for the fictional chocolate brand **Chocolate Works**.

---

## 📌 Project Overview

This dashboard is designed to help business stakeholders and sales managers gain insights into the performance of chocolate sales across different countries, teams, and product categories.

Key metrics covered:
- **Total Sales**: $34M
- **Total Profit**: $21M
- **Total Cost**: $14M
- **Total Shipments**: 6,000
- **LBS Count**: 624
- **Profit %**: 60.3%
- **LBS %**: 10.2%

---

## 🖼️ Dashboard Preview

> _Insert your dashboard image here_

![Sales Dashboard for Chocolates](<INSERT IMAGE PATH HERE>)

---

## 📈 Key Features

### 💡 High-Level KPIs:
- **Total Sales** and **Profit** cards show high-level business performance.
- **Cost**, **Shipments**, and **LBS Count** summarize logistics and expenditure.
- **Profit %** and **LBS %** represented via modern gauge visuals.

### 📊 Visuals Included:
- **Monthly Sales Trend**: Line chart showing sales fluctuations month-wise.
- **Shipments by Boxes (bins)**: Histogram visualizing the distribution of shipments.
- **Sales Performance by Salesperson**:
  - Ranked list of top 10 salespeople.
  - Profit %, LBS %, and indicators to benchmark efficiency.

### 🧭 Filters & Interactions:
- **Country** filter: Australia, Canada, India, etc.
- **Team** filter: Delish, Jucies, Tempo, Yummies.
- **Category** filter: Bars, Bites, Other.
- **Month** slicer for temporal exploration.

---

## 🗃️ Data Model

> _Insert your data model image here_

![Data Model Diagram](<INSERT IMAGE PATH HERE>)

The dashboard is powered by a star schema model structured as follows:

### 🎯 Central Fact Table:
- **Shipments**: Contains transactional metrics including `Boxes`, `Costs`, `Date`, `Geography`, and `Product`.

### 🧩 Dimension Tables:
- `calendar`: Provides date granularity.
- `people`: Contains salesperson details (`Picture`, `Sales person`, `Team`).
- `locations`: Includes `Geo` and `Region` fields.
- `products`: Contains product metadata like `Category`, `Cost per box`, and `Product`.

### 🔗 Relationships:
- One-to-many relationships link dimensions to the `shipments` fact table.
- The model ensures efficient slicing and dicing across various dimensions for intuitive analysis.

---

## 🛠️ Tools Used

- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Data Modeling using Star Schema**

---

## 📌 How to Use

1. Download the `.pbix` file (if included).
2. Open with **Power BI Desktop**.
3. Use slicers to explore insights by month, region, team, and category.
4. Observe real-time changes in KPIs and charts based on filters.

---

## ✨ Insights

- **Van Tuxwell** had the highest profit % at **64.7%**.
- **Brien Boise** achieved both high profit and a balanced LBS %.
- Some salespeople like **Beverie Moffet** lag behind in profit-to-LBS efficiency.
- Sales peaked during **Jan 2024**, highlighting a possible seasonality trend.

---

## 📥 Contributions

Feel free to fork, modify, or submit improvements via Pull Requests.

---



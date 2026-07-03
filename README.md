# 🛒 E-Commerce End-to-End Analytics | Power BI Project

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black">
  <img src="https://img.shields.io/badge/DAX-Advanced-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Star%20Schema-Data%20Model-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Power%20Query-ETL-orange?style=for-the-badge">
</p>

---

# 🌟 Executive Summary

This project demonstrates an end-to-end **Business Intelligence solution** built using **Power BI**. It transforms raw e-commerce transaction data into interactive dashboards through **Power Query**, **Star Schema data modeling**, and **DAX calculations**, enabling data-driven business decisions.

---

# 📊 Business KPIs

- 💰 Total Sales
- 📈 Total Profit
- 🛒 Total Orders
- 📦 Total Quantity Sold
- 👥 Active Customers
- 💳 Average Order Value (AOV)
- 🌍 Region-wise Sales
- ⭐ Top Performing Products
- 🏬 Store Performance
- 📅 Year-over-Year Sales Growth

---

# 📸 Dashboard Preview

## 📈 Executive Sales Dashboard

<p align="center">
<img src="Year_Wise_Analysis.png" width="90%">
</p>

---

## 👥 Customer & Product Dashboard

<p align="center">
<img src="Customer_and_Product_Insights.png" width="90%">
</p>

---

# 🏗️ Project Architecture

```text
Raw Excel Data
      │
      ▼
Power Query (ETL)
      │
      ▼
Star Schema Model
      │
      ▼
DAX Measures
      │
      ▼
Interactive Power BI Dashboard
      │
      ▼
Business Insights
```

---

# ⭐ Star Schema Model

<p align="center">
<img src="Model_View.png" width="85%">
</p>

The project follows a **Star Schema** consisting of one Fact Table connected to multiple Dimension Tables for efficient reporting and optimized DAX calculations.

---

# ⚡ DAX Measures

### Total Sales

```DAX
TOTAL SALES =
SUM(fact_table[total_price])
```

### Year-over-Year Sales Growth

```DAX
% YOY SALES =
VAR A = DIVIDE([TOTAL SALES],[PY SALES]) - 1
VAR LABEL = FORMAT(A,"#0.0%")
RETURN LABEL & IF(A>0,"⬆️","⬇️")
```

### Active Customers

```DAX
ACTIVE CUSTOMERS =
DISTINCTCOUNT(customer_dim[coustomer_key])
```

---

# 📈 Key Business Insights

- Analyze sales performance across multiple years.
- Identify top-performing products.
- Compare regional sales performance.
- Monitor customer purchasing behaviour.
- Evaluate store-wise performance.
- Measure Year-over-Year business growth.

---

# 🛠️ Tech Stack

- Microsoft Power BI
- Power Query
- DAX
- Microsoft Excel
- Power BI Service

---

# 🚀 Future Enhancements

- Real-time SQL Database Integration
- Predictive Sales Forecasting
- Advanced Customer Segmentation
- Automated Dashboard Refresh
- Drill-through Reports

---

# 📬 Connect With Me

**Gargi Kundu**

📧 gargikundu211@gmail.com

💼 LinkedIn: https://www.linkedin.com/in/gargi-kundu

🐙 GitHub: https://github.com/Gargik283

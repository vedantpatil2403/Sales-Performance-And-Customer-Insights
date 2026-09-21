# 📊 Retail Sales Performance & Customer Insights Analysis

## 📌 Executive Summary
This project delivers an end-to-end data analytics workflow modeling over **100,000+ retail transactions** across 6 relational datasets. Using **Python (`pandas`, `numpy`, `matplotlib`, `seaborn`)**, the analysis transforms raw transactional records into actionable business intelligence—evaluating total revenue drivers, product category performance, discount strategies, and regional sales distribution.

The goal is to provide data-driven recommendations for revenue optimization, customer retention strategies, and inventory planning.

---

## 💡 Key Business Insights & Findings

### 1. Revenue & Profitability Core Dynamics
* **Top Revenue Drivers:** High-end electronics and core product categories generate over **60%** of total revenue.
* **Profit Margin Analysis:** The overall profit margin sits at **26.17%**, driven primarily by high-volume orders with low discount rates.
* **Discount Impact:** Average discounts are maintained at **3.38%**; higher discount tiers (>10%) show diminishing returns on net profit margins without significantly boosting volume.

### 2. Customer Purchasing Behavior
* **Customer Base:** 13,937 unique active customers out of 15,000 registered profiles.
* **Order Frequency:** Average order value (AOV) stands at **₹4,229.10**, with repeat customers accounting for the majority of total lifetime value (LTV).

---

## 📈 High-Level Business KPIs

| Metric | Value |
| :--- | :--- |
| **Total Revenue** | ₹169,163,902.87 |
| **Total Profit** | ₹44,270,425.29 |
| **Profit Margin** | 26.17% |
| **Total Orders** | 40,000 |
| **Total Active Customers** | 13,937 |
| **Total Units Sold** | 301,358 |
| **Average Order Value (AOV)** | ₹4,229.10 |
| **Average Discount** | 3.38% |

---

## 🗂️ Data Architecture & Relational Model

The project models and joins data across 6 primary datasets:

```text
               +-------------------+
               |  Customers_Large  |
               +---------+---------+
                         |
                         | (1 : N)
                         v
+-------------------+  (1:N)  +-------------------+  (N:1)  +-------------------+
|   Regions_Large   | <------ |   Orders_Large    | ------> |    Sales_Reps     |
+-------------------+         +---------+---------+         +-------------------+
                                        |
                                        | (1 : N)
                                        v
                              +-------------------+
                              |   Order_Details   |
                              +---------+---------+
                                        |
                                        | (N : 1)
                                        v
                              +-------------------+
                              |  Products_Large   |
                              +-------------------+
---

## 🛠️ Tech Stack & Skills
- **Language:** Python
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib`, `seaborn`
- **Analytics:** Data Profiling, Feature Engineering, Relational Merging, KPI Analysis

---


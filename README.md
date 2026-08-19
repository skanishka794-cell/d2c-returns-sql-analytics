# 📦 D2C E-Commerce Logistics & Margin Recovery SQL Engine

An end-to-end relational SQL analytics project executed in MySQL to isolate reverse logistics cost leakages, identify regional return hotspots, and evaluate SKU-level defect concentrations.

---

## 📌 Executive Summary & Key Findings
* **Channel Exposure:** Cash on Delivery (COD) orders produce a **9.68% return rate**, generating disproportionate dead freight loss compared to prepaid channels like Net Banking (4.29%) and Credit Cards (5.84%).
* **Product Defect Concentration:** *Hair Growth Actives Serum* (7 returns) and *Oat Extract Gentle Cleanser* (6 returns) ranked #1 in returns within their categories.
* **Geographic Risk:** *West Bengal* (12.77%), *Delhi* (8.89%), and *Madhya Pradesh* (8.44%) were categorized as *High Risk Hubs*.
* **Root Cause Breakdown:** *Skin irritation* was the single largest return driver for Cleansers (41.67%) and Body Care (33.33%).
* **Customer Segmentation:** Identified a segment of 10 chronic returners (2+ returns) averaging 4.30 orders per user.

---

## 🛠️ Advanced SQL Techniques Demonstrated
* **Window Functions:** `DENSE_RANK() OVER (PARTITION BY ...)` for category SKU rankings and windowed aggregations for root cause percentages.
* **Common Table Expressions (CTEs):** Multi-level subqueries for customer cohort segmentation.
* **Conditional Logic:** `CASE WHEN` statements for risk tiering and customer behavior classification.
* **Defensive Calculations:** Normalized ratios and rate multipliers for dead freight cost modeling (₹110/return).

---

## 📂 Database Schema Overview
* **`customers`**: Customer geographic mapping (`customer_id`, `state`, `city`).
* **`orders`**: Transaction records, order dates, and payment channels (`order_id`, `payment_method`, `order_date`).
* **`order_items`**: Order-level SKU links (`order_id`, `product_id`, `quantity`).
* **`products`**: Catalog attributes and categories (`product_id`, `category`, `product_name`).
* **`returns`**: Defect root causes and return dates (`order_id`, `return_reason`).

---

## 🚀 How to Run
Execute `analysis.sql` against MySQL, PostgreSQL, SQLite, or Snowflake using the provided CSV datasets.

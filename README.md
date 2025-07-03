# 🏬 KULTRA MEGA STORES Inventory SQL Analysis

This project performs detailed data analysis using SQL on the inventory and sales data of **KULTRA MEGA STORES (KMS)**. The goal is to help stakeholders gain actionable insights from the store's performance dataset.

---

## 📄 Project Overview

The SQL queries answer critical business questions such as:
- Top-performing product categories and regions
- Customer behavior and segmentation
- Shipping cost efficiency
- Recommendations for increasing revenue

The analysis is divided into two main case scenarios to guide business decisions using data-driven insights.

---
## 🧠 Tools Used
+ Microsoft SQL Server / PostgreSQL

+ SQL (T-SQL syntax)

+ GitHub for version control

---
## 📁 Files

- SQL Dsa Project Query.sql: Main SQL query file

- KMS_File.csv (assumed): Raw dataset

- README.md: Project documentation

## 📦 Dataset

**Table Name**: `KMS_File`  
**Additional Table**: `Order_Status` (for return status)  
Imported from a CSV file into a relational database.

---

## ⚙️ Preprocessing Steps

Before analysis, the following columns were formatted to two decimal places:
- `Sales`, `Discount`, `Profit`, `Unit_Price`, `Shipping_Cost`, `Product_Base_Margin`

```sql
ALTER TABLE KMS_File
ALTER COLUMN Sales DECIMAL(10,2);
-- Repeated for other relevant columns

---

# 📊 Case Scenario 1: Sales & Revenue Optimization

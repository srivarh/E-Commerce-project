# E-Commerce Customer Segmentation Using RFM and Decile Analysis

## Project Overview

This project focuses on **customer segmentation and revenue contribution analysis** for an e-commerce business using **Python, PostgreSQL/SQL, and Power BI**.

The goal of this project is to analyze customer purchase behavior, identify high-value and low-value customers, understand revenue concentration, and recommend targeted marketing strategies based on customer value.

The analysis uses:

- **Exploratory Data Analysis (EDA)** to understand sales trends, product performance, country-level revenue, and customer purchase frequency.
- **RFM Analysis** to segment customers based on Recency, Frequency, and Monetary value.
- **Decile Analysis** to rank customers by revenue contribution and identify the most valuable customer groups.
- **Power BI Dashboards** to visualize insights and support business decisions.

---

## Business Problem

E-commerce businesses generate large volumes of transactional data, but without proper customer segmentation, marketing teams may treat all customers the same.

This can lead to:

- Inefficient marketing budget allocation
- Missed customer retention opportunities
- Poor targeting of high-value customers
- Wasted campaigns on low-return customer groups

This project solves that problem by using customer transaction data to identify which customers should be prioritized for retention, upselling, cross-selling, and reactivation campaigns.

---

## Objectives

The main objectives of this project are:

1. Clean and prepare raw e-commerce transaction data.
2. Perform exploratory data analysis to understand overall business performance.
3. Calculate RFM metrics at the customer level.
4. Segment customers into meaningful groups.
5. Rank customers into deciles based on monetary value.
6. Analyze revenue contribution by customer decile.
7. Build interactive Power BI dashboards.
8. Provide actionable marketing recommendations.

---

## Tools and Technologies Used

| Tool | Purpose |
|---|---|
| Python | Data cleaning and preprocessing |
| Pandas / NumPy | Data manipulation |
| PostgreSQL / SQL | EDA, RFM, and decile analysis |
| Power BI | Dashboard creation and visualization |
| Excel / CSV | Source data and cleaned data handling |

---

## Dataset Description

The dataset contains e-commerce transaction records.

### Original Columns

| Column | Description |
|---|---|
| InvoiceNo | Unique transaction/invoice number |
| StockCode | Product/item code |
| Description | Product description |
| Quantity | Quantity purchased |
| InvoiceDate | Transaction date and time |
| UnitPrice | Price per unit |
| CustomerID | Unique customer identifier |
| Country | Customer country |

### Created Columns

| Column | Description |
|---|---|
| TotalSales | Quantity × UnitPrice |
| IsCancelled | Identifies cancelled invoices |
| IsValidSale | Identifies valid completed sales |

---

## Dataset Size

| Dataset | Rows | Columns | Purpose |
|---|---:|---:|---|
| Raw Dataset | 541,909 | 8 | Original transaction data |
| Cleaned Dataset | 536,641 | 11 | Cleaned master transaction table |
| Valid Sales Dataset | 524,874 | 11 | Used for EDA |
| RFM Dataset | 392,688 | 11 | Used for customer segmentation |
| RFM Customer Output | 4,338 | Customer-level | Used for RFM and decile analysis |

---

## Project Workflow

```text
Raw Data
   ↓
Python Data Cleaning
   ↓
Cleaned Dataset
   ↓
SQL-Based EDA
   ↓
RFM Customer Segmentation
   ↓
Decile Analysis
   ↓
Power BI Dashboards
   ↓
Business Insights and Recommendations

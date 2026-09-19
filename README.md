# Analysis-using-SQL-and-Pandas-

# 🛍️ Retail Consumer Behavior Analytics Project

An end-to-end data analytics project analyzing customer shopping patterns to optimize retail sales, customer engagement, and product strategies. Developed step-by-step using **Python (Jupyter Lab)**, **SQLite (SQL)**, and **Power BI**.

---

## 📋 Business Problem Statement
A leading retail company wanted to better understand consumer shopping behavior across demographics, product categories, and sales channels (online vs. offline) to improve sales, satisfaction, and long-term loyalty. 

**Overarching Business Question:**  
*"How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?"*

---

## 🚀 Project Workflow & Milestones f

### Milestone 1: Data Preparation & Cleaning (Python / Jupyter Lab)
**Dataset:** $3,900$ customer transactions with $18$ raw attributes.
**Data Cleaning:** Handled missing review ratings by imputing median values.
**Feature Engineering:** 
  * Created **`Age Group`** (`Young Adult`, `Adult`, `Middle-Aged`, `Senior`).
  * Created **`Spending Tier`** (`Low`, `Medium`, `High`) using quantile-based bucketing.


## Milestone 2: SQL Data Analysis & Database Simulation (SQLite / Jupyter Lab)
**Database Setup** & Integration: Initialized an enterprise-grade in-memory SQLite database environment directly inside Jupyter Lab and loaded the feature-engineered dataset into a structured relational table named customer_transactions.

**Relational Querying:** Simulated production-level database queries using SQL statements (SELECT, GROUP BY, ORDER BY, and aggregate functions like SUM and AVG) to extract targeted business insights.

**Segment & Channel Aggregations:** Executed multi-column groupings and filtering commands to evaluate performance across geographical regions, product categories, payment methods, and customer subscription statuses.






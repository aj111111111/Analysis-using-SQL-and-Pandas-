# Analysis-using-SQL-and-Pandas-

# 🛍️ Retail Consumer Behavior Analytics Project

An end-to-end data analytics project analyzing customer shopping patterns to optimize retail sales, customer engagement, and product strategies. Developed step-by-step using **Python (Jupyter Lab)**, **SQLite (SQL)**, and **Power BI**.

---

## 📋 Business Problem Statement
A leading retail company wanted to better understand consumer shopping behavior across demographics, product categories, and sales channels (online vs. offline) to improve sales, satisfaction, and long-term loyalty. 

**Overarching Business Question:**  
*"How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?"*

---

## 🚀 Project Workflow & Milestones

### Milestone 1: Data Preparation & Cleaning (Python / Jupyter Lab)
* **Dataset:** $3,900$ customer transactions with $18$ raw attributes.
* **Data Cleaning:** Handled missing review ratings by imputing median values.
* **Feature Engineering:** 
  * Created **`Age Group`** (`Young Adult`, `Adult`, `Middle-Aged`, `Senior`).
  * Created **`Spending Tier`** (`Low`, `Medium`, `High`) using quantile-based bucketing.

```python
import pandas as pd
import numpy as np

# Load and clean dataset
df = pd.read_csv('customer_shopping_behavior.csv')
df['Review Rating'] = df['Review Rating'].fillna(df['Review Rating'].median())

# Feature Engineering
labels = ['Young Adult', 'Adult', 'Middle-Aged', 'Senior']
df['Age Group'] = pd.cut(df['Age'], bins=bins, labels=labels)
df['Spending Tier'] = pd.qcut(df['Purchase Amount (USD)'], q=3, labels=['Low', 'Medium', 'High'])

# Export cleaned data
df.to_csv('updated_dataset.csv', index=False)

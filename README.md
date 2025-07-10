# 🛒 Instacart Customer Behavior Analysis

## 📌 Project Summary

This bootcamp project explores and analyzes real-world grocery order data from **Instacart**, a same-day delivery service. The goal is to clean the dataset and extract insights about customer ordering habits, product trends, and purchasing patterns through exploratory data analysis (EDA).

---

## 🧠 Objectives

- Perform **data cleaning**: handle missing values, duplicates, and fix data types.
- Conduct **EDA** to uncover patterns in order frequency, reorder rates, and customer behavior.
- Visualize results using clear, labeled plots.
- Generate actionable business insights based on customer behavior.

---

## 🗃️ Dataset Overview

This project uses **five CSV files**, each representing a part of Instacart’s database:

| File Name             | Description |
|-----------------------|-------------|
| `instacart_orders.csv` | Information about each customer order (date, time, user, etc.) |
| `order_products.csv`   | Items in each order, including order of addition and reorders |
| `products.csv`         | List of products and their categories |
| `aisles.csv`           | Grocery aisle categories |
| `departments.csv`      | Higher-level departments grouping products |

> ⚠️ The dataset has been intentionally modified (missing values and duplicates) to practice cleaning skills.

---

## 🔧 Project Workflow

### Step 1: Load and Inspect Data

- Use `pd.read_csv()` with correct parameters due to non-standard file formatting.
- Understand structure, size, and content of each table.

### Step 2: Preprocess Data

- Check and correct data types (e.g., integer IDs).
- Identify and handle:
  - **Missing values** (with appropriate justification).
  - **Duplicates** (and why they may occur).
- Document all preprocessing decisions clearly in Markdown cells.

### Step 3: Exploratory Data Analysis (EDA)

#### ✅ Section A – Basic Order Patterns

- Validate ranges for `order_hour_of_day` (0–23) and `order_dow` (0–6).
- Plot:
  - Orders per hour of day.
  - Orders per day of week.
  - Distribution of `days_since_prior_order`.

#### ✅ Section B – Customer Behavior Insights

- Compare order times on **Wednesday vs. Saturday** using overlapping histograms.
- Plot distribution of **total orders per customer**.
- Identify the **top 20 most frequently ordered products**.

#### ✅ Section C – Reordering and Cart Patterns

- Analyze:
  - Average items per order.
  - Top 20 most **reordered** products.
  - **Reorder rate per product**.
  - **Reorder ratio per user**.
  - Top 20 products **most frequently added first to carts**.

---

## 📊 Tools & Technologies

- Python
- Pandas
- Jupyter Notebook
- Matplotlib / Seaborn for visualizations

---

## 📈 Key Insights to Discover

- When do customers place orders most frequently?
- What are the most reordered products and which users reorder the most?
- How many items do users typically buy per order?
- Which products tend to be the first added to the cart?


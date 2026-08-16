# Zepto E-Commerce Inventory & Sales Analysis

## 📌 Project Overview

This project analyzes an e-commerce inventory dataset inspired by **Zepto**, using **PostgreSQL and Supabase**.

The goal of this project is to practice real-world SQL data analysis, including data exploration, data cleaning, inventory analysis, pricing analysis, discount analysis, and business-focused problem solving.

The project follows a complete data-analysis workflow:

**Raw Data → Database Setup → Data Exploration → Data Cleaning → Business Analysis → Insights**

---

## 🛠️ Tools & Technologies

* **SQL**
* **PostgreSQL**
* **Supabase**
* **GitHub**

---

## 📊 Dataset

The dataset contains product-level information from an e-commerce inventory system.

### Main columns

| Column                   | Description                    |
| ------------------------ | ------------------------------ |
| `sku_id`                 | Unique identifier for each SKU |
| `Category`               | Product category               |
| `name`                   | Product name                   |
| `mrp`                    | Maximum Retail Price           |
| `discountPercent`        | Discount percentage            |
| `availableQuantity`      | Available inventory quantity   |
| `discountedSellingPrice` | Selling price after discount   |
| `weightInGms`            | Product weight in grams        |
| `outOfStock`             | Stock availability status      |
| `quantity`               | Product quantity               |

The original dataset was obtained from a publicly available Zepto inventory dataset.

---

## 🔍 Project Objectives

The main objectives of this project are:

* Understand the structure of an e-commerce inventory dataset
* Explore product categories and inventory
* Identify missing and inconsistent data
* Clean pricing data
* Analyze discounts and product pricing
* Estimate potential revenue by category
* Analyze out-of-stock products
* Segment products based on weight
* Calculate inventory weight by category
* Answer practical business questions using SQL

---

## 🗂️ Project Workflow

### 1. Database Setup

Created a PostgreSQL table in Supabase to store the Zepto inventory data.

The table contains product information such as category, price, discount, quantity, weight, and stock status.

### 2. Data Exploration

Performed exploratory analysis to understand the dataset.

Analysis included:

* Total number of records
* Sample records
* NULL-value checks
* Product categories
* In-stock vs out-of-stock products
* Products appearing multiple times

### 3. Data Cleaning

Performed data-quality checks and cleaning.

The cleaning process included:

* Identifying products with zero MRP
* Identifying products with zero selling price
* Removing products with zero MRP
* Converting prices from **paise to rupees**
* Verifying the cleaned pricing data

### 4. Business Analysis

Used SQL to answer business-related questions involving:

* Product discounts
* Product pricing
* Inventory availability
* Estimated revenue
* Category performance
* Product value
* Product weight segmentation

---

## 💼 Business Questions

### Q1. What are the top 10 best-value products based on discount percentage?

Identifies products offering the highest discounts.

### Q2. Which products have a high MRP but are out of stock?

Helps identify potentially important products that are currently unavailable.

### Q3. What is the estimated revenue for each category?

Calculates estimated inventory revenue using:

`Discounted Selling Price × Available Quantity`

### Q4. Which products have an MRP greater than ₹500 and a discount below 10%?

Identifies expensive products that provide relatively low discounts.

### Q5. Which 5 categories offer the highest average discount?

Compares discount strategies across product categories.

### Q6. What is the price per gram for products weighing at least 100g?

Helps compare product value based on weight.

### Q7. How can products be grouped into Low, Medium, and Bulk weight categories?

Uses a SQL `CASE` statement to create product weight segments.

| Weight      | Segment |
| ----------- | ------- |
| < 1000g     | Low     |
| 1000g–4999g | Medium  |
| ≥ 5000g     | Bulk    |

### Q8. What is the total inventory weight for each category?

Calculates the total physical inventory weight available within each category.

---

## 🧠 SQL Concepts Used

This project demonstrates practical use of:

* `CREATE TABLE`
* `SELECT`
* `WHERE`
* `DISTINCT`
* `GROUP BY`
* `HAVING`
* `ORDER BY`
* `LIMIT`
* `COUNT()`
* `SUM()`
* `AVG()`
* `ROUND()`
* `CASE`
* `DELETE`
* `UPDATE`
* Aggregate functions
* Conditional filtering
* Data cleaning
* Calculated columns

---

## 📁 Project Structure

```text
zepto-ecommerce-sql-analysis/
│
├── README.md
│
└── sql/
    └── zepto_analysis.sql
```

---

## 📈 Key Analysis Areas

The analysis focuses on several important e-commerce metrics:

### Product Pricing

Comparison of MRP and discounted selling price to understand product pricing.

### Discount Analysis

Identification of products and categories offering high discounts.

### Inventory Analysis

Analysis of available quantities and out-of-stock products.

### Revenue Estimation

Estimation of potential revenue based on selling price and available inventory.

### Product Segmentation

Classification of products into Low, Medium, and Bulk weight categories.

### Category Analysis

Comparison of categories based on discounts, revenue, and inventory weight.

---

## 🎯 Key Takeaways

This project demonstrates how SQL can be used to transform raw e-commerce inventory data into business-oriented analysis.

The analysis provides insights into:

* Product pricing and discounts
* Inventory availability
* Potential revenue by category
* Product value based on price and weight
* Category-level inventory distribution
* High-value products that may require inventory attention

---

## 📚 Learning Reference

This project was created as a learning exercise based on a publicly available SQL data-analysis tutorial.

The tutorial was used as a learning reference, while the project was implemented and practiced using **PostgreSQL and Supabase**.

**YouTube Tutorial:**
[Build SQL Data Analyst Portfolio Project Step-by-Step Guide with Real Zepto Data](https://youtu.be/x8dfQkKTyP0)

The project was adapted to practice SQL data exploration, data cleaning, inventory analysis, and business-oriented analysis.

The purpose of this project is to demonstrate practical SQL and data-analysis skills through a real-world e-commerce dataset.
.

---

## 🚀 Skills Demonstrated

* SQL Data Analysis
* PostgreSQL
* Supabase
* Data Cleaning
* Exploratory Data Analysis
* Inventory Analysis
* E-commerce Analytics
* Business Problem Solving
* Data Aggregation
* GitHub Portfolio Development

---

## 👤 Author

**SQL Data Analysis Portfolio Project**

Built as part of a practical SQL and data-analysis learning journey.

# Zepto E-Commerce Inventory & Sales Analysis

## Project Overview

This project analyzes an e-commerce inventory dataset inspired by Zepto using PostgreSQL and Supabase.

The project focuses on data exploration, data cleaning, inventory analysis, pricing, discounts, estimated revenue, and product segmentation.

The goal is to use SQL to answer practical business questions that can help understand product pricing, inventory levels, discounts, and category performance.

---

## Tools & Technologies

- PostgreSQL
- Supabase
- SQL
- GitHub

---

## Dataset

The project uses a Zepto e-commerce inventory dataset containing product-level information such as:

- Product category
- Product name
- MRP
- Discount percentage
- Available quantity
- Discounted selling price
- Product weight
- Stock status
- Quantity

The original dataset was obtained from Kaggle.

---

## Project Workflow

### 1. Database Setup

Created a PostgreSQL table in Supabase to store the Zepto inventory data.

### 2. Data Exploration

Performed exploratory analysis to understand:

- Number of records
- Sample data
- Missing values
- Product categories
- Stock availability
- Repeated product names

### 3. Data Cleaning

Performed data-quality checks and cleaning, including:

- Identifying products with zero prices
- Removing products with zero MRP
- Converting prices from paise to rupees
- Checking for missing values

### 4. Business Analysis

Used SQL to answer business questions related to:

- Product discounts
- Out-of-stock products
- Estimated category revenue
- High-MRP products
- Average category discounts
- Price per gram
- Product weight segmentation
- Total inventory weight

---

## Business Questions

### Q1. What are the top 10 best-value products based on discount percentage?

### Q2. Which products have a high MRP but are out of stock?

### Q3. What is the estimated revenue for each category?

### Q4. Which products have an MRP greater than ₹500 and a discount below 10%?

### Q5. Which 5 categories offer the highest average discount?

### Q6. What is the price per gram for products weighing at least 100g?

### Q7. How can products be grouped into Low, Medium, and Bulk weight categories?

### Q8. What is the total inventory weight for each category?

---

## SQL Concepts Used

- CREATE TABLE
- SELECT
- WHERE
- DISTINCT
- GROUP BY
- HAVING
- ORDER BY
- LIMIT
- COUNT
- SUM
- AVG
- ROUND
- CASE statements
- DELETE
- UPDATE
- Aggregate functions
- Conditional filtering

---

## Project Structure

```text
zepto-ecommerce-sql-analysis/
│
├── README.md
│
└── sql/
    └── zepto_analysis.sql
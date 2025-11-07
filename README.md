# 🍕 Pizza Sales Analysis

_Analyzing transactional sales data to drive strategic decisions for marketing, operations, and inventory using Python (Pandas, Matplotlib, Seaborn) in Google Colab._

---

## 📌 Table of Contents
- <a href="#overview">Overview</a>
- <a href="#business-problem">Business Problem</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-preparation">Data Preparation</a>
- <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
- <a href="#research-questions--key-findings">Research Questions & Key Findings</a>
- <a href="#key-visualizations">Key Visualizations</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#final-recommendations">Final Recommendations</a>
- <a href="#author--contact">Author & Contact</a>

---
<h2><a class="anchor" id="overview"></a>Overview</h2>

This project analyzes a year's worth of transactional sales data from a pizza store. The goal is to evaluate sales performance, identify key trends, and provide actionable insights to management. This analysis serves as a complete workflow, starting from a Business Requirements Document (BRD) and ending with data-driven recommendations to optimize sales, marketing, and operations.

---
<h2><a class="anchor" id="business-problem"></a>Business Problem</h2>

The pizza store management wanted to move from guesswork to a data-driven strategy. The project was designed to answer several key business questions:
- What are our busiest days and times?
- Which pizzas should we promote, and which ones are underperforming?
- How can we optimize our menu and inventory?
- What are our key performance indicators (KPIs) for sales?

---
<h2><a class="anchor" id="dataset"></a>Dataset</h2>

- **Source:** `pizza_sales.csv`
- **Rows:** 48,620
- **Timeframe:** One year of transactions.
- **Key Fields:**
    - `order_id`: Unique identifier for each order.
    - `pizza_name`: Name of the pizza.
    - `quantity`: Number of pizzas sold in the transaction.
    - `total_price`: Total revenue for the transaction.
    - `order_date`: Date the order was placed.
    - `order_time`: Time the order was placed.
    - `pizza_size`: Size of the pizza (S, M, L, XL, XXL).
    - `pizza_category`: Category of the pizza (Classic, Supreme, Veggie, Chicken).
    - `pizza_ingredients`: List of ingredients for each pizza.

---
<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

- **Google Colab:** The cloud-based notebook environment for analysis.
- **Python:** The core language for analysis.
- **Pandas:** For data loading, cleaning, and manipulation.
- **NumPy:** For numerical operations.
- **Matplotlib & Seaborn:** For data visualization.

---
<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

# 📈 Pizza Sales Analysis

## 📌 Project Overview
This project analyzes transactional sales data from a pizza store to identify key business insights, trends, and Key Performance Indicators (KPIs). The goal is to help management make informed, data-driven decisions related to sales, marketing, and operations.

---

## 🎯 Business Objectives
* Identify overall revenue, total pizzas sold, and total number of orders.
* Determine sales distribution by pizza category, size, and type.
* Analyze time-based trends in sales (daily, monthly, and hourly).
* Highlight best-selling and least-selling pizzas by revenue and quantity.
* Understand customer purchasing behavior through Average Order Value (AOV) and Average Pizza per Order.
* Provide visualization dashboards for effective decision-making.

---

## 📊 Key Performance Indicators (KPIs)
1.  **Total Revenue:** The sum of all `total_price`.
2.  **Total Pizzas Sold:** The sum of all `quantity`.
3.  **Total Orders:** The count of unique `order_id`.
4.  **Average Order Value (AOV):** Total Revenue / Total Orders
5.  **Average Pizzas per Order:** Total Pizzas Sold / Total Orders

---

## 💾 Data Source
The analysis is based on the `pizza_sales.csv` dataset, which contains transactional data.

* **Key Fields:**
    * `order_id`: Unique identifier for each order.
    * `pizza_name`: Name of the pizza sold.
    * `quantity`: Number of pizzas sold per order.
    * `total_price`: Total revenue for the transaction.
    * `order_date`, `order_time`: Timestamps for time-based analysis.
    * `pizza_category`, `pizza_size`: Attributes for classification.
    * `pizza_ingredients`: List of ingredients for each pizza.

---

## 🔧 Tools & Libraries
* **Python**
* **Pandas:** For data manipulation and analysis.
* **Matplotlib & Seaborn:** For data visualization.
* **Numpy:** For numerical operations.
* **Jupyter Notebook:** For interactive analysis and reporting.

---

## 💡 Analysis & Key Findings

### 1. Ingredient Analysis
* The most frequently used ingredients across all pizzas are **Garlic, Tomatoes, and Red Onions**. This insight is crucial for inventory management.

### 2. Time-Based Trends
* **Daily:** Sales revenue peaks towards the end of the week, with **Fridays, Saturdays, and Sundays** being the strongest sales days.
* **Hourly:** Sales show a clear peak during the evening rush hour, typically between **5:00 PM and 7:00 PM**.
* **Monthly:** Sales data indicates fluctuations throughout the year, with **July** showing the highest revenue and order volumes, likely due to promotional campaigns.



### 3. Sales by Category & Size
* **Category:** The **"Classic"** pizza category is the best-seller in terms of quantity sold (14,888), followed by "Supreme" (11,987), "Veggie" (11,649), and "Chicken" (11,050).
* **Size:** **Large (L)** size pizzas contribute the highest revenue, indicating a preference for larger sizes or group orders.

### 4. Top & Bottom Performers
* **Best-Sellers:** The analysis identified the top 5 best-selling pizzas by quantity, providing clear insights into customer preferences.
* **Least-Sellers:** The bottom 5 least-selling pizzas were also identified, highlighting products that may need menu optimization.



---

## 🚀 Business Recommendations
Based on the analysis, management can leverage these insights to:

1.  **Optimize Staffing & Operations:** Focus marketing efforts and increase staffing during peak sales periods (weekends and evenings) to maximize revenue and ensure operational efficiency.
2.  **Menu Optimization:** Analyze the performance of the least-selling pizzas. Management should consider modifying the recipes, running targeted promotions, or removing them from the menu to reduce waste and simplify operations.
3.  **Inventory Management:** Ensure a stable supply of the most-used ingredients (Garlic, Tomatoes, Red Onions) to avoid stockouts, especially during peak seasons.

---

## ⚙️ How to Use This Project
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/Pizza-Sales-Analysis.git](https://github.com/your-username/Pizza-Sales-Analysis.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd Pizza-Sales-Analysis
    ```
3.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook Pizza_Sales_Analysis.ipynb
    ```

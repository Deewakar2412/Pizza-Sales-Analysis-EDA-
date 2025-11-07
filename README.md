<div align="center">
  <h1 align="center">🍕 Pizza Sales Analysis 🍕</h1>
  <p align="center">
    An in-depth exploratory data analysis of transactional sales data to drive strategic decisions for marketing, operations, and inventory.
  </p>
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas"/>
  <img src="https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib"/>
  <img src="https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=seaborn&logoColor=white" alt="Seaborn"/>
  <img src="https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=black" alt="Google Colab"/>
</p>

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

- **Source:** `Data/pizza_sales (3).csv`
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

```
pizza-sales-analysis/
│
├── README.md
│
├── Data/                   
│   ├── pizza_sales (3).csv
│   ├── pizza_sales_excel_file (2).xlsx
│
├── Main Business Requirements Doc.pdf    
│   └── Pizza_Sales_EDA.ipynb
│
├── Pizza_Sales_EDA.ipy

```
---
<h2><a class="anchor" id="data-preparation"></a>Data Preparation</h2>

- **Date/Time Conversion:** Converted `order_date` to datetime objects (format `%d-%m-%Y`) and `order_time` to time objects.
- **Feature Engineering:** Created new columns for analysis: `day_of_week`, `hour_of_day`, and `month`.
- **Text Parsing:** Parsed the `pizza_ingredients` string (e.g., "Ingredient1, Ingredient2") into a list of individual ingredients to enable frequency analysis.

---
<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>

The first step of the analysis was to calculate the high-level Key Performance Indicators (KPIs) for the business.

- **Total Revenue:** $817,860.05
- **Total Pizzas Sold:** 49,574
- **Total Orders:** 21,350
- **Average Order Value (AOV):** $38.31
- **Average Pizzas per Order:** 2.32

---
<h2><a class="anchor" id="research-questions--key-findings"></a>Research Questions & Key Findings</h2>

1.  **When are the busiest times? (Time-Based Trends)**
    * **Hourly Trend:** Sales start slow, pick up at lunch (12 PM - 1 PM), and **peak during the evening rush (5 PM - 7 PM)**.
    * **Daily Trend:** The busiest days are **Friday and Saturday**, with Friday being the highest revenue-generating day.
    * **Monthly Trend:** Sales are consistent, with a notable **peak in July** and a dip in October.

2.  **What are our most/least popular products? (Product & Category Insights)**
    * **By Category:** The **"Classic"** category is the clear winner, driving the most orders (14,888 pizzas) and revenue.
    * **By Size:** The **"Large"** size is the most popular, accounting for over 40% of pizzas sold.
    * **Top 5 Best-Sellers:** 1. The Classic Deluxe Pizza, 2. The Barbecue Chicken Pizza, 3. The Hawaiian Pizza.
    * **Bottom 5 Worst-Sellers:** 1. The Brie Carre Pizza, 2. The Mediterranean Pizza, 3. The Calabrese Pizza.

3.  **How can we optimize inventory? (Ingredient Analysis)**
    * **Top Ingredients:** The most frequently used ingredients are **Garlic, Tomatoes, and Red Onions**. This insight is crucial for supply chain management.

---
<h2><a class="anchor" id="key-visualizations"></a>Key Visualizations</h2>

The full notebook contains all visualizations. Below are some of the key charts that drove the final recommendations.

**Total Revenue by Day of the Week**
*(This chart clearly shows Friday and Saturday as the peak sales days.)*
`![Sales by Day of Week](images/daily_sales_chart.png)`

**Total Revenue by Hour of the Day**
*(This chart highlights the critical 12-1 PM lunch spike and the 5-7 PM evening rush.)*
`![Sales by Hour](images/hourly_sales_chart.png)`

**Top 5 Best-Selling Pizzas by Quantity**
*(This chart identifies the "hero" products for marketing.)*
`![Top 5 Pizzas](images/top_5_pizzas_chart.png)`

---
<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

This project was developed using **Google Colab**.

1.  **Open in Google Colab:**
    * Download the `Pizza_Sales_EDA.ipynb` file from this repository.
    * Go to [https://colab.research.google.com/](https://colab.research.google.com/) and upload the notebook.
    * *(Alternatively, if your repository is public, you can open it directly by replacing `github.com` with `colab.research.google.com/github/` in your repository's URL.)*

2.  **Upload the Data:**
    * In the Colab environment, find the **"Files"** tab on the left-hand sidebar.
    * Click **"Upload to session storage"** and select the `pizza_sales.csv` file from your computer.
    * **Important:** Ensure the file path in the notebook (e.g., `pd.read_csv('/content/pizza_sales.csv')`) matches the uploaded file's location.

3.  **Run the Analysis:**
    * Run the cells in the notebook sequentially to see the complete analysis.
    * All required libraries (Pandas, Matplotlib, Seaborn) are pre-installed in Google Colab.

---
<h2><a class="anchor" id="final-recommendations"></a>Final Recommendations</h2>

Based on the analysis, the following strategic recommendations were provided to management:

1.  **Optimize Staffing:** Increase staff levels during peak hours (**5 PM - 7 PM**) and on peak days (**Fridays and Saturdays**) to meet customer demand, reduce wait times, and maximize revenue.
2.  **Menu & Marketing Strategy:**
    * Heavily promote the **Top 5 Best-Selling Pizzas** (e.g., "Classic Deluxe") as "Customer Favorites."
    * Analyze the **Bottom 5 Worst-Selling Pizzas**. Consider removing "The Brie Carre Pizza" from the menu to reduce ingredient waste and simplify kitchen operations.
3.  **Inventory Management:**
    * Ensure a consistent stock of ingredients for the **"Classic"** category (the most popular).
    * Maintain a high stock of the **Top 3 ingredients** (Garlic, Tomatoes, Red Onions) to avoid critical stockouts during peak times.

---
## 🚀 How to Use This Project

Follow the steps below to explore and run this end-to-end data analysis project:

### 📂 1. Clone the Repository
```bash
git clone [https://github.com/Deewakar2412/customer-shopping-behavior-analysis.git]
cd customer-shopping-behavior-analysis
---

## 👤 Author

**Deewakar Kumar**
* 📧 Email: `deewakar2412@gmail.com`
* 📍 Bokaro, Jharkhand, India
* [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/deewakarkumar2412/) 
* [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Deewakar2412)

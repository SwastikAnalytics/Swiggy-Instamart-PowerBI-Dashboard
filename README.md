# 🛒 Swiggy Instamart Sales Analysis Dashboard | Power BI

An interactive **Business Intelligence Dashboard** built using **Power BI** to analyze Swiggy Instamart sales performance, customer orders, product categories, city-wise performance, and customer ratings. The dashboard transforms raw sales data into meaningful business insights, enabling data-driven decision-making.

---

# 📑 Table of Contents

* [📌 Project Overview](#-project-overview)
* [🎯 Business Problem](#-business-problem)
* [🎯 Project Objectives](#-project-objectives)
* [📂 Dataset Overview](#-dataset-overview)
* [🛠️ Tools & Technologies](#️-tools--technologies)
* [📊 Dashboard KPIs](#-dashboard-kpis)
* [📈 Dashboard Visualizations](#-dashboard-visualizations)
* [🧹 Data Cleaning & Preparation](#-data-cleaning--preparation)
* [📊 DAX Measures](#-dax-measures)
* [🔍 Key Business Insights](#-key-business-insights)
* [💡 Business Recommendations](#-business-recommendations)
* [📷 Dashboard Screenshot](#-dashboard-screenshot)
* [📁 Project Structure](#-project-structure)
* [🚀 Future Improvements](#-future-improvements)
* [📌 Conclusion](#-conclusion)
* [👨‍💻 Author](#-author)

---

# 📌 Project Overview

Retail grocery businesses generate thousands of transactions every day. Analyzing this data manually is time-consuming and inefficient.

This Power BI dashboard provides a centralized view of business performance by tracking sales, orders, customer ratings, shop performance, and product category trends.

It enables management to monitor KPIs and make informed business decisions.

---

# 🎯 Business Problem

The business lacked a centralized reporting system to monitor sales performance.

Management wanted answers to questions such as:

* Which city tier generates the highest sales?
* Which product categories perform the best?
* How are orders changing over time?
* Which shop types contribute the most revenue?
* How satisfied are customers?

The objective was to transform raw transactional data into actionable business insights.

---

# 🎯 Project Objectives

* Analyze overall sales performance.
* Monitor customer order trends.
* Compare sales across city tiers.
* Identify top-performing product categories.
* Evaluate customer ratings.
* Build an interactive dashboard for management.

---

# 📂 Dataset Overview

The dataset contains information related to:

* Iteam code
* Shop code
* Categories
* Shop Types
* Shop Sizes
* Sales
* City Tiers
* Shop Opening Year
* Customer Ratings

---

# 🛠️ Tools & Technologies

| Tool             | Purpose                        |
| ---------------- | ------------------------------ |
| Power BI Desktop | Dashboard Development          |
| Power Query      | Data Cleaning & Transformation |
| DAX              | Business Calculations          |
| Excel            | Data Source                    |


---

# 📊 Dashboard KPIs

* 💰 Total Sales(The owerall revenue generated from all items sold.)
* 📦 Total Orders-Number of items(The total count of different items sold.)
* 💵 Average Sales(The average revenue per sale.)
* ⭐ Average Customer Rating(The average customer rating for items sold.)

---

# 📈 Dashboard Visualizations

### KPI Cards

Used to display key business metrics.

---

### Line Chart

Shows yearly order trends.

---

### Bar Chart

Compares sales across product categories.

---

### Donut Chart

Displays city-wise order contribution and shop-size distribution.

---

### Matrix Table

Provides detailed business metrics including:

 Metric = {
 
    ("Total_Sales", NAMEOF('Grocery Shop'[Total_Sales]), 0),
    
    ("Total_Order", NAMEOF('Grocery Shop'[Total_Order]), 1),
    
    ("Avg_Sales", NAMEOF('Grocery Shop'[Avg_Sales]), 2),
    
    ("Avg_Rating", NAMEOF('Grocery Shop'[Avg_Rating]), 3)
    
}

* Total Sales               
* Average Sales
* Total Orders
* Average Ratings
  
---

### Slicers

Interactive filtering by:

* Shop Opening Year
* Shop Size
* City Tier

---

# 🧹 Data Cleaning & Preparation

The dataset was cleaned using Power Query.

Performed tasks:

* Removed replace value
* Corrected data types
* Validated data quality
* Standardized formatting

---

# 📊 DAX Measures

```DAX
Total Sales =
SUM('Grocery shop'[Sales])
```

```DAX
Total Orders =
COUNTROWS('Grocery shop')
```

```DAX
Average Sales =
AVERAGE('Grocery shop'[Sales])
```

```DAX
Average Rating =
AVERAGE('Grocery shop'[Rating])
```

---

# 🔍 Key Business Insights

* Tier 3 cities generated the highest sales.
* Fruits & Vegetables emerged as the top-selling category.
* Supermarket Type 1 contributed the highest revenue.
* Customer ratings remained relatively consistent across shop sizes.
* Order volume showed positive growth over time.

---

# 💡 Business Recommendations

* Expand operations in high-performing Tier 3 cities.
* Increase inventory for high-demand categories.
* Improve customer satisfaction through better delivery service.
* Launch targeted marketing campaigns for low-performing categories.
* Monitor KPI performance regularly using Power BI dashboards.

---

# 📷 Dashboard Screenshot



<img src="image/Dashboard.png" alt="Project Architecture" width="1000">



# 📁 Project Structure

```

Swiggy-Instamart-Sales-Analysis/
│
├── Dataset/
│   └── Instamart_Data.xlsx
│
├── Dashboard/
│   └── Swiggy Dashboard.pbix
│
├── Images/
│   └── Dashboard.png
│
├── README.md
│
└── LICENSE
```

---

# 🚀 Future Improvements

* Profit Analysis
* Monthly Sales Trend
* Year-over-Year Growth
* Sales Forecasting
* Dynamic Tooltips
* Drill-through Reports
* Customer Segmentation
* Mobile Layout Optimization

---

# 📌 Conclusion

This project demonstrates how Power BI can transform raw business data into interactive dashboards that support strategic decision-making.

The dashboard enables business users to monitor KPIs, identify trends, compare performance, and make data-driven decisions efficiently.

---

# 👨‍💻 Author

**Swastik Kumar**

**B.E. Computer Engineering**

**Data Analyst | Excel | SQL | Power BI | Python | Google Apps Script**

GitHub: https://github.com/SwastikAnalytics

linkedin: https://www.linkedin.com/in/swastik-kumar-01sep


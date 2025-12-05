# 📊 Superstore Executive Summary: Sales & Profitability Analysis

![Power BI](https://img.shields.io/badge/Power_BI-Desktop-yellow?style=for-the-badge&logo=powerbi)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 🖼️ Dashboard Preview
<img width="1519" height="852" alt="image" src="https://github.com/user-attachments/assets/784b1fb5-610c-44f2-994f-d10532804400" />


## 📝 Project Overview
This project involves a comprehensive analysis of the **Superstore Sales Dataset**, a retail dataset containing data on sales, profits, and shipping across the United States. 

The goal was to build an interactive **Power BI Dashboard** that allows executives to monitor Key Performance Indicators (KPIs), identify profitable regions, and analyze shipping efficiency against targets. The dashboard utilizes a dark-themed UI for high-contrast visibility of critical metrics.

**Dataset Source:** [Kaggle - Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)

---

## 🎯 Key Business Questions Answered
1.  **Profitability:** Which states and customers are driving the highest profits?
2.  **Operational Efficiency:** Are we meeting our shipping time targets across different shipping modes?
3.  **Sales Trends:** How do sales vary by month across different product categories (Furniture, Office Supplies, Technology)?
4.  **Customer Segmentation:** Which customer segments (Consumer, Corporate, Home Office) contribute most to sales volume?

---

## 📊 Dashboard Features & Insights

### 1. KPI Header
* **Total Sales:** 2.30M
* **Total Profit:** 286.40K
* **Profit Margin:** 12.03%
* *Interactive Slicers:* Allows filtering by **Year** and **Region**.

### 2. Operational Analysis
* **Avg Shipping Days by Ship Mode:** A bar chart analyzing the efficiency of shipping classes.
    * *Insight:* "Standard Class" shipping takes the longest (~5 days), while "Same Day" is the fastest. A reference line highlights the acceptable threshold.

### 3. Regional & State Performance
* **Profit Margin of Each State:** A column chart ranking states by profitability.
    * *Insight:* **California** and **New York** are the clear leaders in profit generation, significantly outperforming other states like Washington and Michigan.

### 4. Product & Segment Trends
* **Average of Sales by Category:** A line chart showing monthly trends.
    * *Insight:* **Technology** products show significant volatility with a strong peak in sales towards the end of the year (Oct-Nov), likely due to holiday seasonality.
* **Sales by Segment:** A pie chart breakdown.
    * *Insight:* The **Consumer** segment is the largest contributor to sales, followed by Corporate.

### 5. Customer Insights
* **Top 5 Customer Sales Overview:** An area chart highlighting the top revenue-generating clients (e.g., Adrian Barton, Tamara Chand) to identify key accounts.

---

## 🛠️ Technical Implementation
* **Data Cleaning:** Processed raw CSV data to ensure correct data types for dates and currency.
* **DAX Measures:** Created custom measures for:
    * `Total Sales` = SUM(Orders[Sales])
    * `Total Profit` = SUM(Orders[Profit])
    * `Profit Margin` = DIVIDE([Total Profit], [Total Sales], 0)
    * `Avg Shipping Days` = AVERAGE(Orders[Days to Ship])
* **Data Visualization:** Used standard visuals (Bar, Line, Area, Pie) with a consistent blue-on-black color theme for visual hierarchy.

---

## 🚀 How to Run
1.  Download the `.pbix` file from this repository.
2.  Open the file in **Microsoft Power BI Desktop**.
3.  The data is embedded, but you can update the Data Source settings to point to the local CSV file if needed.

---

## 👤 Author
* **Vamsi siva ganesh seelam**
* [Your LinkedIn Profile Link]https://www.linkedin.com/in/vamsi-/
* (https://vamsisivaganesh.vercel.app/)

*If you found this project useful, please give it a ⭐!*

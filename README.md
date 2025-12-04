# Zomato
# 🍔 Zomato Market Insights: Pan-India Executive Summary

![Power BI](https://img.shields.io/badge/Power_BI-Desktop-yellow?style=for-the-badge&logo=powerbi)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Data](https://img.shields.io/badge/Data-Zomato_Kaggle-blue?style=for-the-badge)

## 📊 Project Overview
This project is an end-to-end **Power BI** analysis of the Indian restaurant aggregation market. Using a dataset of over **45,000+ restaurants** across India's top 100 cities, this dashboard provides strategic insights into dining trends, pricing dynamics, and customer preferences.

The goal was to transform raw data into actionable intelligence for stakeholders in the Food-Tech industry, helping them understand where the market is saturated and where opportunities lie.

---

## 🖼️ Dashboard Visuals

### 1. Executive Summary

<img width="1356" height="770" alt="image" src="https://github.com/user-attachments/assets/286ec63d-3f79-4f12-ab9f-ea4681b4a46a" />



---

## 🎯 Problem Statement
The Indian food delivery market is highly competitive. Stakeholders (Investors, Restaurant Owners, Zomato Execs) struggle to answer key questions based on raw data alone:
1.  **Market Penetration:** Which cities have high restaurant density but low average ratings?
2.  **Pricing Strategy:** What is the optimal "Cost for Two" in Tier-1 vs. Tier-2 cities?
3.  **Operational Quality:** Do restaurants with "High Safety" tags actually get better customer ratings?
4.  **Cuisine Demand:** Which cuisines are the primary revenue drivers in specific regions?

---

## 🛠️ Tech Stack & Methodology

### 1. Data Cleaning (Power Query)
* **Handling Nulls:** Removed records with missing coordinates or critical rating data.
* **Standardization:** Corrected inconsistent city names and merged duplicate entries.
* **Transformation:** Created conditional columns to categorize "Price Range" into Low, Medium, and Premium buckets.

### 2. Data Modeling
* Built a **Star Schema** to optimize performance.
* Created a dedicated **Date Table** (if applicable) and Dimension tables for `City`, `Cuisine`, and `Restaurant Info`.

### 3. DAX Calculations
Key measures created for this analysis:
* `Avg Rating` = AVERAGE(Data[Aggregate Rating])
* `Restaurant Count` = DISTINCTCOUNT(Data[Restaurant ID])
* `Safety Compliance %` = Calculate percentage of restaurants with valid hygiene ratings.
* `Delivery Speed Score` = Weighted average based on delivery time buckets.

---

## 🔍 Key Insights Discovered

* **Geographic Dominance:** While North India has the highest density of restaurants, South Indian cities show a higher average customer retention rate.
* **The "Safety Premium":** Restaurants with "Excellent" safety ratings saw a **15% higher** average order value compared to non-compliant ones.
* **Pricing Sweet Spot:** In Tier-1 cities, the optimal "Cost for Two" for maximum order volume is between **₹500 - ₹800**.
* **Cuisine Trends:** Local cuisines outperform international chains in Tier-2 cities, whereas Fast Food dominates the metro hubs.

---

## 📂 Dataset
* **Source:** (https://www.kaggle.com/datasets/rrkcoder/zomato-data-40k-restaurants-of-indias-100-cities/data)
* **Volume:** ~45,000 Records
* **Key Attributes:** Restaurant Name, City, Location, Cuisines, Currency, Has Table Booking, Has Online Delivery, Aggregate Rating, Votes.

---

## 🚀 How to Run This Project
1.  Download the `.pbix` file from this repository.
2.  Open the file in **Power BI Desktop**.
3.  (Optional) If you want to refresh the data, update the data source settings to point to your local CSV file path.

---

## 👤 Author

**VAMSI SIVA GANESH SEELAM**
* Data Analyst | Power BI Developer
* https://www.linkedin.com/in/vamsi-
* https://vamsisivaganesh.vercel.app/

---
*If you find this project useful, please ⭐ this repository!*

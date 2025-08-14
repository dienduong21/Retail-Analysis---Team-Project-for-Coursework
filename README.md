# Retail-Analysis-Team-Project-for-Coursework

## 📌 Project Overview
This is the final project for the Business Analytics course at university. It is an exploratory data analysis of a retail company’s sales, customer, and product dataset provided by our lecturer. The objective was to independently define key business questions and uncover insights to improve business performance. The analysis was presented through an interactive Power BI dashboard.

## 🏆 Team Result
- Evaluated on analytical approach, dashboard quality, and actionability  
- **Final Score:** **9.5/10**

---

## 🎯 Report Objectives
- Understand performance trends across time, geography, customer segments, and product categories.  
- Identify high-performing markets, behaviors, and assortment opportunities.  
- Propose data-driven strategies for pricing, marketing, and operations.

---

## ❓ Key Questions Answered
- How did sales and customer behavior vary by month, region, and segment?  
- Which products/brands/categories drove revenue and margin potential?  
- What time windows and customer demographics offer the highest growth potential?

---

## 🛠 Tools & Techniques Used
- **Excel**: data understanding, cleaning, descriptive statistics  
- **Power BI**: data modeling, visualization, basic forecasting  
- **Transformations**: VLOOKUP/XLOOKUP, custom lookup tables, data type fixes, anomaly detection  
- **DAX**: `Quarter`, `Time_Bin` (4-hour bins), `Weekday`

---

## 👤 My Role
- **Team Lead**: project scoping, task allocation, QA, delivery
- **Data Owner**: full data understanding & cleaning; created lookup tables (**Geography**, **Product**, **Ratings**)
- **Dashboard Developer**: designed & built all report pages (Overview, Geography, Customer, Product, Sales & Forecast)

---

## 🔍 Steps to Conduct
1. **Data Understanding**  
   - Reviewed all fields for meaning, properties, and data types  

2. **Data Cleaning**  
   - Missing values: imputed/derived (e.g., totals from price × quantity) or removed when <1% or non-recoverable  
   - Duplicates: removed using composite keys (e.g., `TransactionID + CustomerID + Product`)  
   - Value fixes: standardized brands, product types (e.g., AC categories), city names (e.g., Düsseldorf/Münster)  
   - **Created lookup tables** and joined back to the fact table:
     - `Geography (Country, State, City)`
     - `Product (Brand, Category, Type)`
     - `Ratings (scale normalization)`

3. **Descriptive Statistics**  
   - Distribution of purchases, amount per transaction, total spend per customer, ratings, and age  
   - Identified skewness and concentration of high-value customers

4. **Business Insights & Solutions**  

   **1 – Seasonal Sales Peaks & Volatility**  
   - Sales peaked in **October** and **January**, likely tied to seasonal events/promotions, but dipped sharply in **February**.  
   - **Solution:** Implement targeted off-peak campaigns (e.g., loyalty discounts, limited-time bundles) to smooth revenue and maintain customer engagement year-round.  

   **2 – Geographic Opportunities**  
   - **USA** accounts for **31.41%** of total sales, with **Chicago** and **Portsmouth** exceeding $6M each.  
   - Germany and Canada have fewer customers but higher **average revenue per customer**.  
   - **Solution:** Maintain high-volume strategy in USA, while testing premium-positioning campaigns in Germany & Canada to leverage higher per-customer value.  

   **3 – High-Value Customer Segments**  
   - Medium-income customers contribute both **high revenue** and **high ratings**, especially medium-income **males** with strong preference for **spring water**.  
   - **Solution:** Develop loyalty programs and targeted upsell campaigns for this segment; bundle spring water with complementary high-margin products.  

   **4 – Product Portfolio Dynamics**  
   - Top categories: **Books, Grocery, Electronics**.  
   - Price increases have a **positive correlation with units sold** for certain SKUs (e.g., Spring Water, Adventure).  
   - **Solution:** Use dynamic pricing and product bundling to maximize profit; prioritize inventory and marketing for top-moving categories.  

   **5 – Fulfillment Bottlenecks**  
   - **16%** of orders remain pending, risking customer satisfaction.  
   - **Solution:** Implement real-time tracking & fulfillment KPIs; automate alerts for delays; negotiate SLAs with logistics partners.  

   **6 – Time-Based Revenue Opportunities**  
   - Peak transaction times: **Wed 00:00–04:00** and **Thu 16:00–20:00**.  
   - **Solution:** Launch flash sales or targeted ads during these windows; align campaigns with time zone differences to capture overseas demand.  

   **7 – Payment Preferences**  
   - Credit cards are the dominant payment method, especially for male customers.  
   - **Solution:** Partner with banks for cashback/loyalty promotions; ensure seamless credit card processing to improve checkout conversion.

---

## 📊 Dashboard Preview
<img width="1242" height="745" alt="Screenshot 2025-08-13 182527" src="https://github.com/user-attachments/assets/d3798eb9-7fbb-4990-b91f-7ec03938f390" />

- **Overview** — topline sales, transactions, ratings over time
<img width="1244" height="744" alt="Screenshot 2025-08-13 182547" src="https://github.com/user-attachments/assets/76bb768f-0d4a-4773-9e16-495870609740" />

- **Geography Analysis** — country/state/city performance & opportunities
<img width="1244" height="746" alt="Screenshot 2025-08-13 182614" src="https://github.com/user-attachments/assets/0d69d387-8c94-4e8c-a688-586ab668a170" />

- **Customer Analysis** — demographics, income segments, behaviors, payment mix
<img width="1245" height="741" alt="Screenshot 2025-08-13 182629" src="https://github.com/user-attachments/assets/16c25c9b-8ef3-41ac-9ab9-501be482cec5" />

- **Product Analysis** — categories/brands drivers, price–volume dynamics
<img width="1243" height="744" alt="Screenshot 2025-08-13 182652" src="https://github.com/user-attachments/assets/55a0a692-8251-4904-ad2a-56aca80d189e" />

- **Sales Trend & Forecast** — seasonality and 2024 projections for planning
<img width="1243" height="742" alt="Screenshot 2025-08-13 182708" src="https://github.com/user-attachments/assets/70a2308b-6c7c-4177-b12c-e9a5ea396464" />

---



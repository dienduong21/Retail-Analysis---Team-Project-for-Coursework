# Retail-Analysis-Team-Project-for-BA-Coursework

## 1. Project Overview
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

## 2. Tools & Techniques Used
- **Excel**: data understanding, cleaning, descriptive statistics  
- **Power BI**: data modeling, visualization, basic forecasting  
- **Transformations**: VLOOKUP/XLOOKUP, custom lookup tables, data type fixes, anomaly detection  
- **DAX**: `Quarter`, `Time_Bin` (4-hour bins), `Weekday`

---

## 3. My Role
- **Team Lead**: project scoping, task allocation, QA, delivery
- **Data Owner**: full data understanding & cleaning; created lookup tables (**Geography**, **Product**, **Ratings**)
- **Dashboard Developer**: designed & built all report pages (Overview, Geography, Customer, Product, Sales & Forecast)

---
## 4. Dashboard Preview
<img width="1242" height="745" alt="Screenshot 2025-08-13 182527" src="https://github.com/user-attachments/assets/d3798eb9-7fbb-4990-b91f-7ec03938f390" />

- **Overview**: topline sales, transactions, ratings over time
<img width="1244" height="744" alt="Screenshot 2025-08-13 182547" src="https://github.com/user-attachments/assets/76bb768f-0d4a-4773-9e16-495870609740" />

- **Geography Analysis**: country/state/city performance & opportunities
<img width="1244" height="746" alt="Screenshot 2025-08-13 182614" src="https://github.com/user-attachments/assets/0d69d387-8c94-4e8c-a688-586ab668a170" />

- **Customer Analysis**: demographics, income segments, behaviors, payment mix
<img width="1245" height="741" alt="Screenshot 2025-08-13 182629" src="https://github.com/user-attachments/assets/16c25c9b-8ef3-41ac-9ab9-501be482cec5" />

- **Product Analysis**: categories/brands drivers, price–volume dynamics
<img width="1243" height="744" alt="Screenshot 2025-08-13 182652" src="https://github.com/user-attachments/assets/55a0a692-8251-4904-ad2a-56aca80d189e" />

- **Sales Trend & Forecast**: seasonality and 2024 projections for planning
<img width="1243" height="742" alt="Screenshot 2025-08-13 182708" src="https://github.com/user-attachments/assets/70a2308b-6c7c-4177-b12c-e9a5ea396464" />

---

## 5. Steps to Conduct
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

## 🔍 Key Insights 

**1. Seasonal Sales Volatility**:
Sales peaked in October ($12.9M) and January ($12.7M), driven by seasonal demand, but dropped to $12.0M in February - the sharpest monthly decline in the observed period.

**2. Geographic Concentration and Untapped Markets**:
The USA generates 31.41% of total revenue ($27.42M), with Chicago and Portsmouth each exceeding $6M. Germany and Canada, while smaller in customer volume, demonstrate higher revenue per customer, pointing to latent premium demand.

**3. High-Value Customer Profile**:
Medium-income customers are the most valuable segment, contributing both the highest revenue ($37.80M) and relatively strong satisfaction ratings. Within this group, male customers show a concentrated preference for spring water and grocery products.

**4. Fulfillment Gap**:
16.17% of all orders ($14.11M) remain in pending status. Given that delivered orders account for 43.68% of total sales, unresolved fulfillment is a material risk to customer retention and revenue realization.

**5. Price-Demand Dynamics in Key Products**:
Certain products, notably Spring Water and Adventure, exhibit a positive correlation between price increases and units sold, suggesting inelastic or prestige-driven demand that has not yet been fully monetized.

**6. Transaction Time Concentration**:
The highest revenue windows occur on Wednesday 00:00–04:00 and Thursday 16:00–20:00, reflecting time zone-driven demand from international customer bases.

---

### Strategic Recommendations

> Applying the Pareto principle, the following three areas: fulfillment performance, customer segment activation, and geographic expansion. They represent the highest-impact levers, collectively addressing the drivers of the majority of revenue risk and growth opportunity.

---

**Priority 1: Resolve Fulfillment Bottlenecks** *(Highest Urgency)*

With $14.11M sitting in pending status, this is the most immediate threat to revenue and customer satisfaction. Poor fulfillment directly erodes repeat purchase rates and average ratings.

- **Short term (2024, Q2–Q3):** Establish real-time order tracking with automated escalation alerts for orders exceeding standard processing windows. Define and enforce service level agreements with logistics partners.
- ***Expected impact:** converting even 30% of pending orders to delivered status would recover approximately $4.2M in at-risk revenue and measurably improve the average rating above its current 3.15 baseline.*
- **Long term (2025 onward):** Integrate a fulfillment performance dashboard with monthly operational reviews. Explore regional warehouse partnerships in high-volume markets such as USA and UK to reduce processing lag structurally.
- ***Expected impact:** a sustained pending rate below 5% would protect an estimated $10M+ in annual revenue and strengthen customer retention, reducing churn risk in the top-performing cities.*

---

**Priority 2: Activate and Retain the Medium-Income Customer Segment**

This segment generates $37.80M (43.3% of total revenue) and is the most satisfied customer group. Deepening loyalty here has compounding returns through higher lifetime value and reduced acquisition cost.

- **Short term (2024, Q2–Q4):** Launch a tiered loyalty program targeting medium-income customers, with rewards anchored to their top-performing products including spring water and grocery. Introduce product bundles pairing spring water with complementary higher-margin items.
- ***Expected impact:** a 10% increase in purchase frequency within this segment could yield an additional $3.8M in revenue, based on its current contribution baseline.*
- **Long term (2025 onward):** Develop personalized re-engagement campaigns using purchase history segmentation. Expand bundle offerings across grocery and electronics informed by basket analysis.
- ***Expected impact:** improved retention within this segment is estimated to reduce customer acquisition costs over time, as retaining an existing customer is typically 5 to 7 times less costly than acquiring a new one.*

---

**Priority 3: Diversify into High-Potential Geographic Markets**

Germany and Canada represent underserved markets with above-average revenue per customer. Continued over-reliance on the USA limits the structural growth ceiling of the business.

- **Short term (2024, Q3–Q4):** Run controlled premium-positioning pilots in Germany and Canada, testing localized campaigns and higher-margin product sets such as electronics and books against a defined conversion target.
- ***Expected impact:** capturing a 15% increase in average order value in these two markets, consistent with their observed per-customer premium, could add an estimated $2M to $4M in incremental revenue within 12 months.*
- **Long term (2025 onward):** If pilots demonstrate a positive return, scale dedicated regional marketing budgets for Germany and Canada. Simultaneously deepen investment in Chicago and Portsmouth through city-level retention campaigns to protect the existing $12M+ combined base.
- ***Expected impact:** a balanced geographic portfolio reduces revenue concentration risk, where currently over 31% of total sales depend on a single country.*

---

## 6. Lessons Learned & Takeaways

- **Data quality is the foundation of credible analysis.** Systematic cleaning, lookup table 
  design, and field-by-field validation were the most time-consuming steps, but they directly 
  determined the accuracy of every insight and visualization that followed.

- **Defining business questions before building anything keeps the work focused.** Every 
  chart, metric, and recommendation in this project traces back to a question agreed upon 
  at the start,  without that discipline, it is easy to produce visually impressive dashboards 
  that do not actually support decision-making.

- **Quantifying impact transforms observations into actionable insights.** Attaching 
  reasonable revenue estimates to recommendations, even with stated assumptions, made the 
  analysis significantly more persuasive and demonstrated the real business value of the 
  analytical work.



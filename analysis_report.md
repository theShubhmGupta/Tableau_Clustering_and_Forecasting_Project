# 📊 Tableau_Clustering_&_Forecasting_Project — Analysis Report

## 1. Project Overview

This analysis is based on the **Sample Superstore Dataset** — a widely used retail dataset containing transactional data for a US-based superstore, covering orders, customers, products, regions, sales, discounts, and profits.

The dashboard was built in **Tableau** to uncover category-level sales performance, customer behavior, regional trends, and future sales projections — using both standard visualizations and advanced analytics like **K-Means Clustering** and **Sales Forecasting**.

---

## 2. Dashboard Charts & Analysis

---

### 📌 Chart 1: Comparison of Region & Segment By Sales

**Business Question:** Which regions and customer segments are driving the most sales?

#### 🔍 What it Shows
- A comparative breakdown of sales across the four regions (East, West, Central, South) and three customer segments (Consumer, Corporate, Home Office)
- Regions are sorted in descending order by total sales
- Color-coding distinguishes segments within each region for easy comparison

#### 💡 Insight
- The **West and East regions** consistently generate the highest sales across all segments
- The **Consumer segment** dominates sales in every region — it is the largest revenue-driving segment for the superstore
- The **Central and South regions** lag significantly behind, indicating either lower market penetration or weaker demand in those areas
- The **Home Office segment** contributes the least across all regions, reflecting its smaller customer base

#### ✅ Recommendation
- Focus **targeted marketing campaigns** in the Central and South regions to close the sales gap with West and East
- Since Consumer is the strongest segment everywhere, **loyalty programs and repeat-purchase incentives** would yield the highest ROI
- Investigate why Home Office sales are low — it may represent an **underserved but growing segment** in the post-remote-work era

---

### 📌 Chart 2: Customer Segmentation (K-Means Clustering)

**Business Question:** Can customers be grouped into distinct behavioral clusters based on their purchasing patterns?

#### 🔍 What it Shows
- A **K-Means clustering model** applied to customer data, grouping customers into **3 distinct clusters** based on sales and purchasing behavior
- Each cluster represents a unique customer profile — high-value, mid-tier, or low-engagement customers
- Outliers are identified separately as "Cluster Outliers" — customers who don't fit neatly into any group

#### 💡 Insight
- **Cluster 1 (High-Value):** A smaller group of customers generating disproportionately high sales — these are the superstore's most important customers
- **Cluster 2 (Mid-Tier):** The largest cluster — regular buyers with moderate spend who represent the core of the customer base
- **Cluster 3 (Low-Engagement):** Customers with infrequent or low-value purchases — high potential for re-engagement
- **Outliers** represent unique purchasing behaviors that don't fit standard patterns — these could be bulk buyers or one-time large-order customers

#### ✅ Recommendation
- For **Cluster 1 (High-Value):** Introduce a VIP or premium membership program — protecting this group from churn is critical since they contribute outsized revenue
- For **Cluster 2 (Mid-Tier):** Use **upselling and cross-selling strategies** to move them toward high-value behavior — small increases in spend per customer have large cumulative impact
- For **Cluster 3 (Low-Engagement):** Run **win-back campaigns** with discounts or personalized offers to reactivate dormant customers

---

### 📌 Chart 3: Sales & Profit for Each Year and Sub-Category

**Business Question:** Which sub-categories are profitable and which are loss-making across years?

#### 🔍 What it Shows
- A year-over-year breakdown of both **Sales and Profit** for each sub-category (e.g., Phones, Chairs, Binders, Tables, etc.)
- Dual-metric view reveals sub-categories where high sales do NOT translate to high profit
- Trends over time show whether sub-category performance is improving or declining

#### 💡 Insight
- **Phones and Chairs** consistently show high sales but varying profit margins — volume leaders that need margin protection
- **Tables** is a notorious loss-maker — high sales volume but negative or near-zero profit due to heavy discounting
- **Copiers and Accessories** tend to show strong profit relative to their sales — high-margin sub-categories
- **Binders** show high sales but thin or negative profits — another sub-category likely suffering from excessive discounting

#### ✅ Recommendation
- **Immediately review the discounting policy for Tables and Binders** — these sub-categories are generating revenue but destroying profit; cap discounts to restore margin
- **Double down on Copiers and Accessories** — these are the most profitable sub-categories and deserve more shelf space, marketing budget, and inventory investment
- Use year-over-year trends to identify sub-categories with **declining profit trajectories** and intervene before they become loss-making

---

### 📌 Chart 4: Sales Forecast by Category for Each Year

**Business Question:** What are the projected sales for each product category in the coming years?

#### 🔍 What it Shows
- A **time-series forecast** of sales broken down by the three main categories: **Furniture, Office Supplies, and Technology**
- Uses Tableau's built-in forecasting model to project future sales based on historical trends
- A **Forecast Indicator** distinguishes actual historical data from projected future values

#### 💡 Insight
- **Technology** shows the strongest upward sales trajectory and is forecast to continue growing — it is the highest-revenue category
- **Office Supplies** demonstrates steady, consistent growth — a reliable but slower-growing category
- **Furniture** shows the flattest growth curve — limited upside potential compared to the other two categories
- All three categories show an **upward forecast trend**, suggesting overall business health — but growth rates differ significantly by category

#### ✅ Recommendation
- **Increase inventory and marketing investment in Technology** ahead of the forecast period — supply chain readiness is critical to capture projected demand
- For **Office Supplies**, focus on **subscription or bulk-order models** to lock in the steady demand and reduce acquisition costs
- For **Furniture**, explore whether **product line refreshes or new sub-categories** could unlock faster growth — the current trajectory is too flat to rely on

---

### 📌 Chart 5: Sales by Segment & Sub-Category

**Business Question:** Which sub-categories perform best within each customer segment?

#### 🔍 What it Shows
- A detailed matrix of sales broken down simultaneously by **Segment (Consumer, Corporate, Home Office)** and **Sub-Category**
- Reveals which products resonate most with each type of buyer
- Helps identify segment-specific product strengths and gaps

#### 💡 Insight
- **Phones** are the top-selling sub-category across all three segments — universally strong demand regardless of buyer type
- **Chairs and Storage** perform strongly in the **Corporate segment** — reflecting office setup purchases
- **Consumer segment** leads in volume across most sub-categories — the broadest and most active buyer group
- **Home Office segment** shows relatively stronger interest in **Bookcases and Supplies** compared to other segments — reflecting home workspace setup needs

#### ✅ Recommendation
- Create **segment-specific product bundles** — e.g., a "Corporate Office Setup" bundle (Chairs + Storage + Phones) and a "Home Office Starter Pack" (Bookcases + Supplies + Phones)
- Use segment-sub-category insights to **personalize email and digital marketing** — showing Corporate buyers office furniture and Consumer buyers tech accessories
- Invest in growing **Home Office sub-category sales** — with remote work becoming permanent for many, this segment's purchasing patterns are likely to grow

---

## 3. Advanced Analytics Used

| Feature | Chart | Description |
|---|---|---|
| 🤖 **K-Means Clustering** | Customer Segmentation | Groups customers into 3 behavioral clusters automatically |
| 📈 **Sales Forecasting** | Sales Forecast by Category | Projects future sales using Tableau's built-in time-series model |

---

## 4. Tools & Dataset

| Item | Details |
|---|---|
| **Tool** | Tableau Desktop / Tableau Public |
| **Dataset** | Sample Superstore (`Sample - Superstore.xls`) |
| **Key Fields** | Order ID, Order Date, Ship Mode, Customer Name, Segment, Region, Category, Sub-Category, Sales, Quantity, Discount, Profit |
| **Categories** | Furniture, Office Supplies, Technology |
| **Segments** | Consumer, Corporate, Home Office |
| **Regions** | East, West, Central, South |

---

*Analysis by Shubham | Category Insights Dashboard Project*
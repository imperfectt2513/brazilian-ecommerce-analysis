# Brazilian eCommerce Analysis 🛒📊

End-to-end data analysis project on 100K+ real Brazilian eCommerce orders (2016–2018).

---

## 🎯 Project Objective

Analyze customer behavior, revenue trends, freight burden, and geographic patterns across 100K+ orders to generate actionable business insights for an eCommerce platform.

---

## 🛠️ Tools Used

- **SQL Server (SSMS)** — Data extraction, transformation, window functions, CTEs, correlated subqueries
- **Excel** — Interactive KPI dashboard, pivot tables, pivot charts, slicers
- **Power BI** — Extended visual dashboard (see related repo below)

---

## 📁 Repository Structure

```
├── ecommerce_analysis.sql        # 9 advanced SQL queries
├── ecommerce_dashboard.xlsx      # Interactive Excel KPI dashboard
├── 01-revenue-by-category.csv
├── 02-monthly-order-volume.csv
├── 03-top10-cities-revenue.csv
├── 04-freight-vs-price.csv
├── 05-revenue-share-pct.csv
├── 06-customer-rank-running-total.csv
├── 07-above-avg-categories.csv
├── 08-top5-cities-revenue-share.csv
├── Query 9 — Above State Average Spenders.csv
```

---

## 📊 Key Business Insights

### 1. Revenue by Category
Bed, bath & table leads all categories with ₹17.1L in revenue, followed by health & beauty (₹16.6L) and computers & accessories (₹15.9L). The top 6 categories collectively contribute over 50% of total platform revenue. Low-performing categories like security & services (₹324) and fashion children's clothes (₹785) occupy platform space without meaningful contribution and should be reviewed for continued listing.

### 2. Monthly Order Volume Trend
Order volume grew from just 4 orders in September 2016 to a peak of 7,544 in November 2017 — representing **1,800x growth in 14 months**. The November 2017 spike is attributable to Black Friday. Volume stabilized between 6,000–7,200 orders/month in early 2018, indicating a maturing platform.

### 3. Geographic Revenue — Top 10 Cities
São Paulo dominates with ₹28.7L — nearly 1.8x Rio de Janeiro (₹15.7L) and 5.7x Belo Horizonte (₹5.1L). The bottom five cities in the top 10 collectively contribute less than São Paulo alone. **Geographic diversification remains the most critical growth lever.**

### 4. Freight Burden Analysis
Home comfort 2 carries a 53.97% freight-to-price ratio — customers pay more than half the product price in shipping. **29 out of 74 categories exceed the 20% freight burden threshold**, making this a systemic logistics problem, not an isolated one. Even top revenue categories are affected: furniture decor sits at 23.67% and electronics at 29% — high concern given price sensitivity.

### 5. Revenue Share Distribution
No single category exceeds 8.37% revenue share, confirming a broadly distributed portfolio. While resilient, this means no category is large enough to anchor a focused growth strategy. The long tail — 40+ categories below 1% share — represents significant platform complexity with marginal revenue return.

> **Data Quality Note:** Two anomalous entries — 'NULL' (₹1.6L) and 'UNKNOWN' (₹2.6L) categories — account for ₹4.2L combined, equivalent to the 8th largest category. Recommendation: trace these records to source orders and assign correct categories before final reporting.

### 6. Customer Spending Distribution (80/20 Analysis)
Customer spending is heavily skewed — a small group of top-ranked customers contributes a disproportionately large share of running total revenue, reaching 50% of total revenue before going through even a fraction of the customer base. **Classic 80/20 behavior.** The top-tier customers (Rank 1–100) should be treated as a VIP segment — loyalty programs, priority support, and early access to deals. Losing even a handful has outsized revenue impact.

### 7. Above-Average Order Value Categories
29 categories perform above the overall average order value of ~180 BRL. High-ticket categories — computers (1,374 BRL), fixed telephony (784 BRL), small appliances (674 BRL) — are the biggest revenue drivers per order. **Focus upsell and cross-sell strategies here** — customers already spending big on computers or appliances have high conversion potential for bundled accessories or warranties.

### 8. Top 5 Cities Revenue Concentration
São Paulo alone contributes ~15% of total store revenue — more than 1 in 7 revenue BRL comes from a single city. There is a sharp drop to Rio de Janeiro at ~7%. São Paulo must be treated as a priority market for logistics and marketing investment. **Rio de Janeiro represents the biggest growth opportunity** given its size and current 7% share.

### 9. Above State Average Spenders
Across all Brazilian states, a consistent segment of customers spends 4x–10x higher than their own state's average. Critically, **this pattern is nationwide** — high-value customers exist in every region, not just São Paulo or Rio. These regional outliers should be tagged as VIP customers and targeted with personalized loyalty programs, regional offers, and faster delivery to increase purchase frequency and lifetime value.

---

## 📈 Dashboard Preview

> Excel KPI dashboard with 4 pivot charts and slicers for category, city, and state-level filtering.
> *(Add screenshot here)*

---

## 🔗 Related Project

- [Brazilian eCommerce — Power BI Dashboard](https://github.com/imperfectt2513/brazilian-ecommerce-powerbi)

---

## 📦 Dataset

- **Source:** Brazilian eCommerce Public Dataset — Olist (via Kaggle)
- **Records:** 100K+ orders
- **Period:** September 2016 – August 2018

---

## 👤 Author

**Dnyaneshwar Tate** | B.Tech Computer Science | 2026  
[LinkedIn](https://linkedin.com/in/dnyaneshwartate) · [GitHub](https://github.com/imperfectt2513)

# customer-behaviour-analysis-sql-powerbi
> A comprehensive data-driven study on beauty & skincare customer behavior — uncovering spending patterns, customer segments, product preferences, and return reasons using **MS SQL Server** and **Power BI**.

![Dashboard Preview](dashboard_screenshot.png)

---

## 📌 Project Overview

This project analyzes real transactional data from a beauty & skincare brand to answer key business questions about **who buys**, **what they buy**, **how they buy**, and **why they return**. The goal is to guide strategic decisions through data.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| MS SQL Server | Data extraction, cleaning & querying |
| Power BI | Interactive dashboard & visualizations |

---

## 📊 Dataset Summary

| Detail | Value |
|--------|-------|
| Total Tables | 6 |
| Total Columns | 39 |
| Total Rows | 4,390 |
| Domain | Beauty & Skincare |

**Tables:** `Customers` · `Orders` · `Order_Items` · `Products` · `Returns` · `Reviews`

---

## 📂 Project Structure

```
customer-shopping-behavior/
│
├── data/
│   ├── Customers.csv
│   ├── Orders.csv
│   ├── Order_Items.csv
│   ├── Products.csv
│   └── Returns.csv
│
├── sql/
│   └── analysis_queries.sql       # All 10 business queries
│
├── powerbi/
│   └── Dashboard.pbix             # Interactive Power BI dashboard
│
├── reports/
│   ├── Analysis_Report.pdf
│   └── Presentation.pdf
│
└── README.md
```

---

## 🔍 SQL Analysis — Business Questions Answered

| # | Question |
|---|----------|
| 1 | Most discount used by age group |
| 2 | Age group with most purchases |
| 3 | Total orders by gender |
| 4 | Top 10 cities by purchases |
| 5 | Top sales channels |
| 6 | Top 5 products by rating |
| 7 | Repeated buyers (more than 5 orders) |
| 8 | Top reasons for product returns |
| 9 | Top customer acquisition channels |
| 10 | High-spending discounted users |

---

## 📈 Power BI Dashboard

The interactive dashboard includes filters by **Gender** and **Product Category**, with the following visuals:

- **KPI Cards** — 500 customers · 2,042 orders · ₹1.12M total revenue
- **Total Orders by Age Group** — Donut chart
- **% of Customers by Acquisition Channel** — Donut chart
- **Most Orders by City** — Bar chart
- **No. of Returns by Return Reason** — Bar chart
- **Discount vs Final Amount by Product** — Stacked bar chart

---

## 💡 Key Insights

### 👥 Customer Segments
- **25–34 age group dominates** with 632 orders (50.56%) and the highest discount usage at ₹62,428
- **18–24** is the second most active group with 313 orders (25.04%)
- Gender split is nearly equal — Male: 441 · Female: 433 · Other: 376

### 🌆 Top Cities
Nagpur (92) → Indore (89) → Lucknow (89) → Surat (87) → Kochi (68)

### 🛒 Sales Channels
Website leads with **698 orders**, followed by Mobile App (444) and Marketplace (108) — together covering **91% of all orders**

### ⭐ Top Rated Products (avg 4.0)
Aqualogica Lightweight Sunscreen · Body Lotion with Niacinamide · Bond Repair Shampoo · Glycolic Acid Face Cleanser · Hyaluronic Acid 2% Serum

### 🔄 Return Reasons
Skin irritation (28) → Late delivery (16) → Damaged packaging (13) → Wrong item (12) → Changed mind (10)

### 📣 Customer Acquisition
Google Search (148) and Instagram (145) together bring in nearly **60% of all new customers**

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/customer-shopping-behavior.git
   ```

2. **Import the CSV files** into MS SQL Server

3. **Run SQL queries** from `sql/analysis_queries.sql`

4. **Open** `powerbi/Dashboard.pbix` in Power BI Desktop and connect to your data source

---

## 📁 Dataset Schema

| Table | Key Columns |
|-------|-------------|
| Customers | customer_id, name, city, state, gender, age_group, signup_date, acquisition_channel |
| Orders | order_id, order_date, order_status, payment_method, sales_channel, gross_amount, discount_amount, final_amount |
| Order_Items | order_item_id, product_id, quantity, unit_price, discount_pct, item_total |
| Products | product_name, category, concern, skin_type, key_ingredient, size, mrp, cost_price |
| Returns | return_id, return_date, return_reason, refund_status |
| Reviews | review_id, rating, review_date |

---

## 📧 Contact

**Your Name**
- 📧 Email: your.email@gmail.com
- 💼 LinkedIn: [linkedin.com/in/your-profile](https://linkedin.com/in/your-profile)
- 🐙 GitHub: [@your-username](https://github.com/your-username)

---

⭐ *If you found this project helpful, please give it a star!*

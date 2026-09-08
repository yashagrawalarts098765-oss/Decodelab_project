# 📊 E-Commerce Data Analysis

*Analyzing 1,200 e-commerce orders (Jan 2023–Jun 2025) to uncover sales, customer, and fulfillment trends — and turning them into business recommendations.*

![Dashboard Preview](project/dashboard-screenshot.png)

---

## 📌 Overview

This project analyzes an e-commerce transaction dataset to answer real business questions — which products drive revenue, how payment and coupon usage behave, and where the business is losing orders — using a full workflow: **data cleaning → exploratory analysis → SQL querying → Power BI dashboard → business recommendations.**

**Dataset:** 1,200 orders across 7 product categories, spanning January 2023 to June 2025. Fields include order ID, date, customer ID, product, quantity, unit price, payment method, order status, coupon code, referral source, and total price.

---

## 🎯 Business Questions

- Which products generate the most revenue and volume?
- How much revenue is lost to cancelled and returned orders?
- Do coupons actually drive higher order values, or just discount sales that would've happened anyway?
- Which payment methods and referral sources contribute the most revenue?
- How does revenue trend month over month?

---

## 💡 Key Insights

- **Total revenue: ₹12,64,761.96** across 1,200 orders, with an **average order value of ₹1,053.97**.
- **Only 19.25% of orders (231) are marked "Delivered."** A combined **41.4% of orders (497) are Cancelled or Returned** — this is the single biggest issue in the dataset and consistent across every product category (39–44% each), meaning it's a systemic fulfillment problem, not a product-specific one.
- Revenue is fairly evenly spread across the 7 product categories, with **Chairs (₹1,95,620) and Printers (₹1,95,613)** narrowly leading, and **Phones (₹1,51,722)** the lowest.
- **Credit Card is the top payment method by revenue (₹2,63,848)**, followed closely by Online and Cash — no single method dominates, so there's no urgent gateway/checkout gap.
- **Coupons show minimal impact on order value** — average order value stays nearly flat whether a customer used FREESHIP (₹1,070), WINTER15 (₹1,036), SAVE10 (₹1,066), or no coupon at all (₹1,043). This suggests coupons may be discounting revenue without actually driving bigger baskets.
- **Instagram is the top-performing referral source by revenue (₹2,75,285)**, ahead of Email, Google, Facebook, and Referral (₹2,26,816, the lowest).
- Monthly revenue is volatile with no strong seasonal pattern — it swings between roughly ₹28,000 and ₹68,000 per month, peaking in June 2024.
- **Customer base is almost entirely one-time buyers** — 1,189 of 1,200 orders are from unique customers, with only 11 customers placing a second order and none placing a third. There isn't a meaningful repeat-customer segment to build loyalty analysis on with this dataset.

---

## ✅ Business Recommendations

1. **Investigate the fulfillment pipeline urgently** — a 41.4% cancel/return rate is far above healthy e-commerce benchmarks (typically 5–15%). Since it's consistent across every product, the root cause is likely operational (payment failures, delivery logistics, inventory mismatches) rather than product quality — worth a root-cause audit before scaling marketing spend.
2. **Re-evaluate coupon strategy** — since coupon usage isn't lifting average order value, consider reserving discounts for cart-abandonment recovery or first-time buyers rather than blanket usage, to protect margin.
3. **Double down on Instagram as an acquisition channel** given its revenue lead, while testing what's underperforming about Referral traffic.
4. **Build a repeat-purchase incentive** (e.g., post-purchase discount code, loyalty program) — with 99% of customers only ordering once, there's a large untapped opportunity in retention rather than pure acquisition.

---

## 🛠️ Tech Stack

| Layer | Tools |
|---|---|
| Data Cleaning & EDA | Python, Pandas, NumPy, Matplotlib, Seaborn |
| Querying & Analysis | SQL |
| Dashboard | Power BI (DAX, Power Query) |
| Environment | Jupyter Notebook |

---

## 📂 Project Structure

```
E-Commerce-Data-Analysis/
│
├── Data/
│   └── raw_ecommerce.csv
│
├── project/
│   ├── Data Cleaning.ipynb
│   ├── EDA.ipynb
│   ├── cleaned_eco.csv
│   ├── data analyis.sql
│   ├── Dashboard.pbix
│   └── dashboard-screenshot.png
│
└── README.md
```

---

## 🗄️ SQL Analysis

Business questions answered directly in SQL (`project/data analyis.sql`):

- Total revenue and average order value
- Revenue and units sold by product
- Top spending customers
- Revenue and usage by payment method
- Order status breakdown
- Coupon usage and its effect on average order value
- Revenue by referral source
- Monthly sales trend

---

## 📊 Power BI Dashboard

Interactive dashboard (`project/Dashboard.pbix`) with:

- KPI cards: total revenue, orders, AOV, cancellation/return rate
- Revenue trend over time (with MoM DAX measures)
- Product-wise and payment-method breakdown
- Order status funnel view

**Screenshot:**
![Dashboard](project/dashboard-screenshot.png)

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/yashagrawalarts098765-oss/E-Commerce-Data-Analysis.git
cd E-Commerce-Data-Analysis

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the notebooks in order
jupyter notebook "project/Data Cleaning.ipynb"
jupyter notebook "project/EDA.ipynb"

# 4. Open the dashboard
# Open project/Dashboard.pbix in Power BI Desktop
```

---

## 📈 Key Learnings

- End-to-end analytics workflow: raw data → cleaned dataset → SQL insights → BI dashboard
- Writing SQL to answer specific business questions, not just exploratory queries
- Building DAX measures for time-intelligence (MoM growth)
- Translating data findings into actionable business recommendations, including identifying operational red flags (fulfillment rate) that go beyond simple sales reporting

---

## 👨‍💻 Author

**Yash Agrawal**
Aspiring Data Analyst | Python · SQL · Power BI · Excel

[LinkedIn](#https://www.linkedin.com/in/yash-agrawal-71b6a8302/) · [Portfolio](#https://github.com/yashagrawalarts098765-oss/E-Commerce-Data-Analysis/tree/main) · [Email](#yashagrawalarts98765@gmail.com)

---

⭐ If you found this useful, consider starring the repo!
⭐ If you found this useful, consider starring the repo!

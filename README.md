# Business Sales Performance Analytics
### Future Interns — Data Science & Analytics | Task 1 | `FUTURE_DS_01`

---

## Objective
Analyze an online retail dataset to uncover revenue trends, identify top-selling products, evaluate regional performance, and surface actionable business recommendations.

---

## Dataset
- **Source:** [Online Retail Dataset — Kaggle](https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset)
- **Size:** 541,910 rows × 8 columns
- **Period:** December 2010 – December 2011
- **Columns:** InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

---

## Tools Used
| Tool | Purpose |
|------|---------|
| Python (Pandas) | Data loading, cleaning, transformation |
| Matplotlib & Seaborn | Data visualizations |
| Jupyter Notebook | Interactive analysis environment |
| Google Looker Studio | Interactive dashboard |

---

## Data Cleaning Steps
- Removed rows with missing `CustomerID`
- Removed cancelled orders (InvoiceNo starting with `'C'`)
- Filtered out rows with `Quantity ≤ 0` or `UnitPrice ≤ 0`
- Converted `InvoiceDate` to datetime format
- Created new column: `Revenue = Quantity × UnitPrice`

---

## Analysis Performed

| # | Analysis | Chart |
|---|----------|-------|
| 1 | Monthly Revenue Trend | Line chart with area fill |
| 2 | Top 10 Products by Revenue | Horizontal bar chart |
| 3 | Revenue by Country | Bar + Pie chart |
| 4 | Top 10 High-Value Customers | Bar chart |
| 5 | Top 10 Products by Quantity Sold | Horizontal bar chart |
| 6 | Revenue by Day of Week | Bar chart |
| 7 | Repeat vs One-Time Customers | Pie chart |

---

## Key Insights

1. **Revenue Peaks** — Significant spike in Q4, driven by holiday season demand
2. **UK Dominance** — United Kingdom accounts for the majority of total revenue
3. **Top Product** — A small set of products contributes disproportionately to revenue (Pareto effect)
4. **VIP Customers** — Top 10 customers contribute a significant share of total revenue
5. **Thursday is Peak Day** — Highest revenue generated mid-week
6. **Repeat Buyers** — Majority of customers are repeat purchasers, indicating strong loyalty

---

## Recommendations

- Launch **pre-holiday campaigns** in September–October to ride the Q4 revenue wave
- Build a **VIP loyalty program** for top 10% of customers by spend
- Ensure **top products are always in stock** — stockouts directly impact revenue
- Run **Thursday promotions** to capitalize on peak buying behavior
- Target **one-time buyers** with post-purchase email sequences to convert them to repeat customers
- **Expand internationally** — Netherlands, Germany, and France show strong potential

---

## Repository Structure

```
FUTURE_DS_01/
├── FUTURE_DS_01_Sales_Analytics.ipynb
├── online_retail.csv
├── online_retail_cleaned.csv
├── chart_01_monthly_revenue.png
├── chart_02_top_products.png
├── chart_03_country_revenue.png
├── chart_04_top_customers.png
├── chart_05_top_qty_products.png
├── chart_06_day_of_week.png
├── chart_07_repeat_customers.png
├── summary_monthly_revenue.csv
├── summary_top_products.csv
├── summary_country_revenue.csv
├── summary_top_customers.csv
└── README.md
```
## Live Dashboard
**[View Interactive Dashboard]([https://lookerstudio.google.com/s/kQSem6iHWcM](https://lookerstudio.google.com/reporting/55b3cdf0-3d3e-423f-8185-17507543864d))
```
---

*Completed as part of the **Future Interns — Data Science & Analytics** Internship Program*  
*Track Code: DS | Task: 01*


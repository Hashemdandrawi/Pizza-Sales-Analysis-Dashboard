# 🍕 PizzaPulse – Pizza Sales Analysis Dashboard (Excel)

> **Note:** The business problem in this project is a **hypothetical scenario** created to practice and showcase beginner-level data analysis skills. It is not a real company case.

## 1. Business Problem (Assumed)

A pizza restaurant noticed that its sales are dropping. The owner wants to know **what sells and what doesn't**, so he can increase sales and reduce ingredient waste.

**Goal:** Increase sales by a fixed percentage (e.g. **10%**) next quarter by identifying the best and weakest items and the strongest and weakest times, then recommending data-driven decisions.

## 2. Business Questions

1. What are the total sales, number of orders, and average order value?
2. Which pizzas, categories, and sizes sell the most and the least?
3. Which months and days of the week are the strongest and the weakest?
4. Which KPIs should the owner track? (Total sales, total orders, total customers, total quantity, best-selling item)

## 3. Tools Used

| Tool | Purpose |
|---|---|
| PivotTables / PivotCharts | Summarizing and analyzing the data |
| Slicers & Timeline | Interactive filtering |
| Excel formatting | Final dashboard design |
## 4. Pivot Tables Summary

| # | Pivot Table | Rows | Values |
|---|---|---|---|
| 1 | KPI cards | – | Sum of sales, Count of Customer Name, Count of order_id, Sum of quantity |
| 2 | Sales per category | pizza_category | Sum of sales |
| 3 | Monthly sales volume | Month | Sum of sales |
| 4 | Sales by size | pizza_size | Sum of sales |
| 5 | Weekly order distribution | Weekday | Count of order_id (sorted high → low) |
| 6 | Top 5 best-selling pizzas | pizza name | Sum of sales (Top 10 filter → Top 5) |
| 7 | Bottom 5 best-selling pizzas | pizza name | Sum of sales (Top 10 filter → Bottom 5) |

Full step-by-step instructions are in [`pivot_table_steps.txt`](pivot_table_steps.txt).

## 5. Dashboard

The dashboard combines the pivot charts and KPI cards in one sheet, with **slicers** for `pizza_category`, `pizza_size`, and a **timeline** for `order_date`, so the owner can filter everything with one click.

![Dashboard](images/dashboard.png)
![Pivot Tables](images/pivot_tables.png)

### Dashboard components

- **KPI cards:** Total Sales, Total Customers, Total Orders, Total Quantity
- **Doughnut chart:** Total sales per category
- **Line chart:** Monthly sales volume
- **Pie chart:** Sales distribution by pizza size
- **Column chart:** Weekly order distribution
- **Bar charts:** Top 5 and Bottom 5 best-selling pizzas
- **Filters:** Category, Size, Order date timeline

## 6. Key Insights

| Metric | Result |
|---|---|
| Total sales | **$8,436.05** |
| Total orders | **499** |
| Total quantity | **511** |
| Average order value | **≈ $16.91** (8,436.05 ÷ 499) |
| Best category | **Veggie (28%)**, then Classic (27%), Supreme (24%), Chicken (21%) |
| Best size | **Large (L) – 48%** of sales; XL is only 3% |
| Best-selling pizza | **The Classic Deluxe Pizza** (459) |
| Weakest pizza | **The Brie Carre Pizza** (47) |
| Strongest months | **June (859)**, **August (858)**, **May (832)** |
| Weakest months | **March (520)**, **February (528)** |
| Busiest day | **Friday (91 orders)** |
| Slowest day | **Wednesday (48 orders)** |

## 7. Recommendations (Data-Driven)

1. **Promote the weak days:** Offer Wednesday/Monday deals (combo or discount) since Friday has almost double the orders of Wednesday.
2. **Boost low-season months:** Run campaigns in February–March, when sales are lowest.
3. **Review the bottom 5 pizzas:** Consider repositioning, bundling, or removing items like Brie Carre and Spinach Supreme to reduce waste in ingredients.
4. **Push the winners:** Feature Classic Deluxe, Four Cheese, and Thai Chicken in ads and combos.
5. **Upsell sizes:** Large is already the leader; test an offer to move Small/Medium customers up to Large.

## 8. Limitations & Next Steps

- This is a practice project based on an assumed scenario.
- Peak **hours** were not analyzed in the dashboard; adding an order-time analysis would complete the "peak hours" question.
- Next steps: add a profit analysis, compare quarter over quarter, and rebuild the dashboard in Power BI.

## 9. Repository Files

```
PizzaPulse/
├── PizzaPulse_Dashboard.xlsx
├── README.md
├── pivot_table_steps.txt
└── images/
    ├── dashboard.png
    └── pivot_tables.png
```

## 10. Author

**Hashem Dandrawi** – Aspiring Data Analyst

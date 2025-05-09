# Sales Analytics Dashboard Documentation
**Note:** Please refer to the attached PDF document before exploring the dashboard — it outlines key business questions and insights derived from the analysis.

## Project Overview

The Sales Analytics Dashboard is an interactive Power BI report that provides executive-level insights into Adventure Works' sales performance. By combining sales transactions, budget figures, and dimensional attributes (products, customers, calendar), stakeholders can explore revenue trends, product performance, and customer segmentation to inform strategic decisions.

**Technologies & Tools**

* **Power BI**: Data modeling, DAX measures, interactive dashboards
* **Excel & CSV**: Source files for sales, budget, product, customer, and calendar data

**Data Sources**

* `FACT_InternetSales.csv`: Internet sales transactions
* `SalesBudget.xlsx`: Monthly sales budget figures
* `DIM_Products.csv`, `DIM_Customers.csv`, `DIM_Calendar.csv`: Dimension tables

## Business Questions & Insights

Below are the key business questions addressed by the dashboard, with references to the corresponding report pages.

### 1. Revenue Performance (Sales Overview page)

* **What is the total revenue and how does it compare to the budget?**
  Displayed via KPI cards showing actual vs. budget and month‑over‑month variance.
* **Which months over‑ or under‑perform against budget?**
  Line chart of monthly actual vs. budget trends highlights peak performance and shortfalls.

### 2. Product Analysis (Product Details page)

* **Which product categories, lines, and individual products generate the highest sales?**

  * Donut and treemap charts for category and line breakdowns.
  * Bar chart of top 10 products by sales.
* **How does product performance evolve over time?**
  Time‑series line chart of sales vs. budget by month.
* **What is the contribution at each level of the product hierarchy?**
  Decomposition tree from Category → Subcategory → Product.

### 3. Customer Segmentation (Customer Details page)

* **Which geographic markets drive the most revenue?**
  Bar chart and treemap of sales by customer country.
* **Who are the top customers by sales?**
  Top 10 customers list with total sales figures.
* **How do customer demographics impact sales?**
  Pie chart segmentation by gender.
* **When did customers make their first purchase?**
  Table showing earliest purchase date per customer.

## Dashboard Features

* **Dynamic Slicers**: Filter by Country, City, Product Name, Product Line, Product Category across all pages.
* **Interactive Visuals**: Hover tooltips, drill‑through details, and highlight states.
* **Custom Visuals**: Decomposition tree, gradient bars, KPI cards.

## File Structure

```
├─ DIM_Calendar.csv
├─ DIM_Customers.csv
├─ DIM_Products.csv
├─ FACT_InternetSales.csv
├─ SalesBudget.xlsx
├─ Sales_Analytics_Dashboard.pbix
└─ DOCUMENTATION.md
```

## How to Run

1. Open `Sales_Analytics_Dashboard.pbix` in Power BI Desktop.
2. Ensure CSV and Excel files are in the same folder or update data source paths.
3. Refresh data to load the latest values and interact with the report.

---

*Prepared by \[Your Name], May 2025*

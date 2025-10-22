

# Excel Project on Financial Data

## Project Overview

This Excel project focuses on **financial data analysis and interactive dashboards** to provide insights into sales, profit, and product performance across different countries, segments, and time periods.
The goal is to simplify decision-making by summarizing large datasets into actionable visual reports.

---

## Dataset Description

The dataset includes the following key columns:

* **Calc Profit, Calc Sales, Calc Gross Match, Calc Gross Sales, COGS, Discount Band, Manufacturing Price, Sales Price, Units Sold, Consistency between month, number, and name, Country, Year, Quarter, Month, Day, Product, Segment, Month Name, Month Number, Gross Difference, Months, Profit Difference, Product & Year Concatenation**

---

## 🧮 Data Preparation

Several calculated columns were added for data consistency and deeper analysis:

* **Profit Check:** Verified as `Profit = Sales - COGS`
* **Sales Calculation:** `Sales = Gross Sales - Discount`
* **Profit Difference:** `Profit Difference = Profit - Calc Profit`
* **Concatenated Column:** `Product-Year = Product + " " + Year` — for easier cross-reference in pivot tables.

---

## Pivot Tables Created

1. **Sales by Country and Year** – Breakdown of total sales per country across years.
2. **Profit by Segment and Product** – Profit performance segmented by business segment and product type.
3. **Monthly Sales Trend** – Tracks sales evolution over time (Month Number and Month Name).
4. **Top 5 Products by Sales** – Highlights the highest-performing products in terms of total sales.

---

## Dashboards and Key Insights

### 1. Line Chart – Monthly Sales Trend

**Insights:**

* Sales fluctuate throughout the year.
* Q1 (Jan–Mar) shows steady but lower sales.
* Mid-year (Jun–Aug) dips slightly.
* November and December peak — strong holiday demand.
* Suggests promoting during mid-year and maximizing Q4 campaigns.

---

### 2. Clustered Column Chart – Sales by Country and Year

**Insights:**

* Year-on-Year Growth from 2013 to 2014 across most countries.
* **Top Market:** United States leads, followed by Germany and France.
* Indicates successful international expansion.

---

### 3. Pie Chart – Profit by Segment and Product

**Insights:**

* Largest slices = most profitable segments/products.
* Smaller slices indicate areas to improve or reconsider continuing.

---

### 4. Bar Chart – Top 5 Products by Sales

**Insights:**

* **Paseo** is the top-selling product (~4,000,000).
* **VTT** and **Velo** follow as moderate performers.
* **Amarilla** and **Montana** show lower performance — potential areas for marketing or product improvement.

---

## Formulas Summary

| Metric             | Value       |
| ------------------ | ----------- |
| **Total Sales**    | 118726125.8 |
| **Average Profit** | 27460.8     |
| **Max Sales**      | 1159200     |
| **Min Sales**      | 1655.08     |

---

## VLOOKUP Implementation

A **VLOOKUP** formula was used to fetch the **Sale Price** based on the *Product-Year* lookup value.
This demonstrated how to efficiently reference specific product-year combinations from a sales dataset.

| Lookup Value     | Sale Price |
| ---------------- | ---------- |
| Paseo - 2013     | 15         |
| Paseo - 2014     | 350        |
| Carretera - 2014 | 7          |
| VTT - 2014       | 300        |

**Formula Used:**

```excel
=VLOOKUP(A2, LookupTable!A:B, 2, FALSE)
```

**Purpose:**
To automatically retrieve sale prices corresponding to specific product-year entries, ensuring data accuracy and eliminating manual lookup errors.

---

## How to Use

1. Download the Excel file.
2. Navigate to the **Dashboard** tab.
3. Use the interactive slicers to filter data.
4. Explore pivot tables directly for deeper insights.
5. Review the **VLOOKUP example** in the “Formulas” sheet for reference.


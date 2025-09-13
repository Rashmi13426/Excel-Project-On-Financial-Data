# Excel-Project-On-Financial-Data

## Project Overview

This Excel project focuses on financial data analysis and interactive dashboards to provide insights into sales, profit, and product performance across different countries, segments, and time periods. The goal is to simplify decision-making by summarizing large datasets into actionable visual reports.

---

## Dataset Description

The dataset includes the following key columns:

* **Calc Profit, Calc Sales, Calc Gross Match, Calc Gross Sales, COGS, Discount Band, Manufacturing Price, Sales Price, Units Sold, Consistency between month, number, and name, Country, Year, Quarter, Month, Day, Product, Segment, Month Name, Month Number, Gross Difference, Months, Profit Difference, Product & Year Concatenation**

---

## Data Preparation

Several calculated columns were added for data consistency and deeper analysis:

- **Profit Check:** Verified as `Profit = Sales - COGS`
- **Sales Calculation:** `Sales = Gross Sales - Discount`
- **Profit Difference:** `Profit Difference = Profit - Calc Profit`
- **Concatenated Column:** `Product-Year = Product + " " + Year` — for easier cross-reference in pivot tables.

---

## Pivot Tables Created

1. **Sales by Country and Year**
   Provides a breakdown of total sales per country across different years.

2. **Profit by Segment and Product**
   Displays profit performance segmented by business segment and product type.

3. **Monthly Sales Trend**
   Tracks the sales evolution over time (by Month Number and Month Name).

4. **Top 5 Products by Sales**
   Highlights the highest-performing products in terms of total sales.

---

## Dashboards and Key Takeaways

A professional dashboard was designed to provide an intuitive, visual summary of key insights and these dashboards were created from the pivot tables.

* Created a line chart for monthly sales trend
  KEY INSIGHTS:
  Sales show a fluctuating pattern throughout the year.
  The first quarter (Jan–Mar) had relatively steady but lower sales.
  A dip is noticeable mid-year (Jun–Aug), indicating weaker performance in summer months.
  Sales peak in November and December, showing strong year-end/holiday demand.
  This seasonal trend suggests opportunities to boost promotions during mid-year and maximize revenue with campaigns during Q4.
  
* Created a Clustered Column Chart for sales by county and year.
  KEY INSIGHTS:
  Year-on-Year Growth: Sales increased from 2013 to 2014 across most countries, showing business expansion.
  Top Market: The United States contributed the highest sales overall, followed by Germany and France.
  
* Created a Pie Chart for profit by segment and product
  KEY INSIGHTS:
  The chart suggests a potential opportunity to focus on the most profitable segments and products (largest slices) to maximize strategy efficiency.
  Conversely, the smaller slices might be reviewed to see if they are worth continuing or could be improved.

  * Created a Bar Chart for top 5 products by sales
    KEY INSIGHTS:
    Paso is the top-selling product, far ahead of the others with sales close to 4,000,000.
    VTT and Velo follow as moderate performers, while Amarilla and Montana have significantly lower sales.
    Focus should be on boosting top products and evaluating underperformers for improvement.

---

## 🎯 How to Use

1. Download the Excel file.
2. Navigate through the Dashboard tab.
3. Use the interactive slicers to filter the data.
4. Explore pivot tables directly for detailed analysis.



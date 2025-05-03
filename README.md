# 🛍️ Discount Promotion Profitability Analysis

This was my first end-to-end project which explored the real profit impact of discount-based promotions using a simulated retail dataset(from InstaCart Data) enriched through SQL, Excel, and Tableau.

I ask found this dataset: https://www.kaggle.com/datasets/psparks/instacart-market-basket-analysis?select=departments.csv

I then asked chatGPT to provide me a question around this data...something real-worldy...

I got something like the one below...

## 🎯 Business Question
Do discounted promotions truly drive profitability across departments and products—or are they hurting margins?

## 💡 Summary
Using simulated promotional data, we analyzed retail performance under four promotion types. Discount promotions showed the lowest profit per item and lowest margin, despite high volume.

## 🔍 Key Metrics
- Profit per Product
- Margin %
- Total Items Sold

## Tools used
- SQL (MySQL)
- Excel
- Tableau
- Git

## 🧪 Approach
1. **SQL**: I first Built a custom enriched table from raw Instacart-style order data using MySQL. Joined multiple tables to prepare a clean base dataset.
2. **Excel**: Simulated key missing data:
  - Randomized **base prices** by department.
  - Assigned **random promotion types** (BOGO, Discount, Loyalty, the rest were left at None).
  - Applied conditional **discount percentages**.
  - Calculated unit cost, revenue, profit, and margin.
3. **SQL AGAIN** Wrote SQL logic to calculate:
  - Top/bottom performing products by profit and margin.
  - Promo type profitability summaries.
  - Department-level performance metrics.
4. **Tableau Visualization**: Built 3 dashboards + an executive summary:
  - **Promotional Effectiveness** (Pie + KPI table)
  - **Top Performing Products** (Filtered by margin and volume)
  - **Underperforming Products & Departments**
  - **Landing Page** with dashboard navigation
5. **Real-World Recovery**: Rebuilt the entire workbook after an accidental file loss(don't ask please) ... recreated all dashboards and structure from scratch. I think the practice helped...
---

##  Project Highlights!

- **SQL Data Modeling**: I first Built a custom enriched table from raw Instacart-style order data using MySQL. Joined multiple tables to prepare a clean base dataset.
- **Excel Enrichment**: Simulated key missing data:
  - Randomized **base prices** by department.
  - Assigned **random promotion types** (BOGO, Discount, Loyalty, the rest were left at None).
  - Applied conditional **discount percentages**.
  - Calculated unit cost, revenue, profit, and margin.
- **Reintegration in SQL**: Imported the enriched data back into MySQL to query for clean, pre-aggregated views due to calculated field limitations(I am still learning!) in Tableau.
- **Custom Queries**: Wrote SQL logic to calculate:
  - Top/bottom performing products by profit and margin.
  - Promo type profitability summaries.
  - Department-level performance metrics.
- **Tableau Visualization**: Built 3 dashboards + an executive summary:
  1. **Promotional Effectiveness** (Pie + KPI table)
  2. **Top Performing Products** (Filtered by margin and volume)
  3. **Underperforming Products & Departments**
  4. **Landing Page** with dashboard navigation
- **Real-World Recovery**: Rebuilt the entire workbook after an accidental file loss — recreated all dashboards and structure from scratch. I think the practice helped...

---

## 📊 Key Findings

- **Discounted items sold well but had the lowest average margin and profit per product.**
- **Discount promotions**, while common(30% of data), led to significantly lower profit margins (~12%) and average profits per product.
- High-volume products like **sushi items** and **Smart Ones Egg Breakfast Wrap** consistently underperformed and even lost money.
- **Personal Care , Snacks and some others** has massive margin gains and were the top departments in regards to profit.
- **Meat Department items** showed to be the most profitable under discounts. Shows emphasis on possiblyt focusing efforts on these products
- Not all positive margins equal strong returns — some departments(Dry goods, breakfast and some others) had thin profits per item despite non-negative margins. There was a need to sell a bunch to break even.

---

## 🔗 Check it out!

- [View on Tableau Public »](https://public.tableau.com/app/profile/tristan.t4195/viz/PromoBook/BottomPerformers?publish=yes)
- Or download the full `.twbx` from this repo to open in Tableau Desktop.

---

## 📁 Folder Structure 




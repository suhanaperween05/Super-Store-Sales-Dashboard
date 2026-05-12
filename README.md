<h1>Super Store Sales Dashboard</h1>
<br>
<p>The Super Store Sales Dashboard is an interactive Power BI report designed to analyze sales and profit performance for a retail superstore business. The dashboard provides a clear view of key business metrics such as total sales, total profit, profit margin, quantity sold, average delivery days, loss amount, and loss-making orders.</p>
<p>This project is divided into two main dashboard pages: Sales Analysis and Profit Analysis. The Sales Dashboard helps track sales performance by customer segment, product category, sub-category, shipping mode, payment method, and state. It also includes year-over-year monthly sales and profit trends to compare business performance across different time periods.</p>
<p>The Profit Analysis Dashboard focuses on profitability by category, sub-category, customer segment, and state. It highlights profitable areas as well as loss-making orders, helping identify where the business is performing well and where improvement is needed.</p>
<p>The project was developed using Power BI Desktop, with data cleaning and transformation performed in Power Query and business calculations created using DAX measures. This dashboard demonstrates skills in data analysis, data visualization, interactive reporting, KPI tracking, and business intelligence dashboard design.</p>

<h2>Project Insight</h2>
-The Central region recorded total sales of 341.01K, profit of 27.45K, and a profit margin of 8.05%.<br>
-The Consumer segment generated the highest sales compared to Corporate and Home Office segments.<br>
-Standard Class was the most used shipping mode and contributed the highest sales.<br>
-Office Supplies had the highest sales among product categories.<br>
-COD was the most preferred payment method, followed by Online and Cards.<br>
-The Profit Analysis Dashboard shows total profit of 175.26K with an overall profit margin of 11.19%.<br>
-Technology generated the highest profit among all categories.<br>
-Some orders generated losses, with a total loss amount of -91.71K, showing areas where pricing, discount, or product strategy may need improvement.<br>
-State-wise visuals help identify regions with strong and weak sales or profit performance.<br>
-Year-over-year monthly trends help compare sales and profit performance between 2019 and 2020.<br>



## Dashboard Preview

[Sales Dashboard](Sales_Dashboard.png)

[Profile Dashboard](Profile_Dashboard.png)


## Key KPIs

- Total Sales
- Total Profit
- Profit Margin
- Quantity Sold
- Average Delivery Days
- Sales by Segment
- Sales by Category and Sub-Category
- Sales by Ship Mode
- Sales by Payment Method
- Sales and Profit by State
- Year-over-year monthly sales and profit

## Tools Used

- Power BI Desktop
- Power Query
- DAX
- Excel / CSV


## Data Cleaning and Transformation

The dataset was cleaned and transformed in Power Query before building the dashboard. Main cleaning steps included:

- Removed duplicate records
- Checked and handled missing values
- Corrected data types for date, sales, profit, quantity, and delivery fields
- Created calculated delivery days from order date and ship date
- Standardized category, segment, region, ship mode, and payment method fields
- Created date-based columns such as year, month, and month name
- Prepared the data model for dashboard analysis


## DAX Measures

Example measures used in the dashboard:

```DAX
Total Sales = SUM(Orders[Sales])

Total Profit = SUM(Orders[Profit])

Profit Margin = DIVIDE([Total Profit], [Total Sales])

Total Quantity = SUM(Orders[Quantity])

Average Delivery Days = AVERAGE(Orders[Delivery Days])
```

More measures are documented in [DAX Measures](dax_measures.md)




<h6>
## Credits

This project was created for learning and portfolio purposes using a Super Store sample dataset by given link. The dashboard was recreated and customized as part of my Power BI practice.

Raw dataset reference: [https://www.youtube.com/watch?v=fZn83JRt4Nk](https://drive.google.com/drive/folders/1HDkNHNslI3rgCv9LZzGtxag8JvYzss-b)</h6>

# Data Cleaning Steps

Use this file to explain what you cleaned in Power Query.

## Cleaning Performed

1. Imported the Super Store sales dataset into Power BI.
2. Checked column headers and renamed fields where needed.
3. Removed duplicate rows.
4. Removed blank rows and unnecessary columns.
5. Changed data types:
   - Order Date: Date
   - Ship Date: Date
   - Sales: Decimal Number
   - Profit: Decimal Number
   - Quantity: Whole Number
   - Discount: Decimal Number / Percentage
6. Trimmed and cleaned text columns such as Segment, Category, Sub-Category, Region, State, Ship Mode, and Payment Method.
7. Created a Delivery Days column:

```powerquery
Duration.Days([Ship Date] - [Order Date])
```

8. Created Year, Month Number, and Month Name columns from Order Date.
9. Checked for negative profit values and kept them because they represent loss-making orders.
10. Loaded the cleaned data into Power BI for modeling and visualization.

## Data Quality Checks

- Checked missing values in important columns.
- Verified date columns imported correctly.
- Verified sales, profit, and quantity columns are numeric.
- Checked duplicate order records.
- Checked whether delivery days are valid and non-negative.

## Notes

Negative profit values are not errors. They are useful for identifying loss-making categories, products, states, or ship modes.

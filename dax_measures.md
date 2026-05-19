# DAX Measures

Add or update these measures according to your table and column names.

```DAX
Total Sales = SUM(SuperStore_Sales_Dataset[Sales]) 
```

```DAX
Total_Profit = SUM(SuperStore_Sales_Dataset[Profit])
```

```DAX
ProfitMargin = DIVIDE(SUM(SuperStore_Sales_Dataset[Profit]), SUM(SuperStore_Sales_Dataset[Sales]), 0)  
```

```DAX
Total Quantity = SUM(SuperStore_Sales_Dataset[Quantity])
```

```DAX
AvgDelivery = DATEDIFF('SuperStore_Sales_Dataset'[Order Date],'SuperStore_Sales_Dataset'[Ship Date],DAY) 
```

```DAX
Total Orders = DISTINCTCOUNT(SuperStore_Sales_Dataset[Order ID])
```

```DAX
Average Order Value = DIVIDE([Total Sales], [Total Orders])
```
```DAX
Average_Profit_per_order = DIVIDE(SuperStore_Sales_Dataset[Total_Profit], DISTINCTCOUNT(SuperStore_Sales_Dataset[Order ID]))
```
```DAX
Loss_making_orders =
CALCULATE(
    COUNTROWS(SuperStore_Sales_Dataset),
    SuperStore_Sales_Dataset[Profit] <0
    )
```
```DAX
New_ProfitMargin = DIVIDE(SuperStore_Sales_Dataset[Total_Profit],SuperStore_Sales_Dataset[Total Sales], 0)
```
```DAX
Loss Amount = CALCULATE(SUM(SuperStore_Sales_Dataset[Profit]), SuperStore_Sales_Dataset[Profit] <0)
```

```DAX
YoY Sales Growth =
DIVIDE(
    [Total Sales] - [Sales Previous Year],
    [Sales Previous Year]
)
```

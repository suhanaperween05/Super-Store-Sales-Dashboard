# DAX Measures

Add or update these measures according to your table and column names.

```DAX
Total Sales = SUM(Orders[Sales])
```

```DAX
Total Profit = SUM(Orders[Profit])
```

```DAX
Profit Margin = DIVIDE([Total Profit], [Total Sales])
```

```DAX
Total Quantity = SUM(Orders[Quantity])
```

```DAX
Average Delivery Days = AVERAGE(Orders[Delivery Days])
```

```DAX
Total Orders = DISTINCTCOUNT(Orders[Order ID])
```

```DAX
Average Order Value = DIVIDE([Total Sales], [Total Orders])
```

```DAX
Loss Orders = 
CALCULATE(
    COUNTROWS(Orders),
    Orders[Profit] < 0
)
```

```DAX
Sales Previous Year =
CALCULATE(
    [Total Sales],
    SAMEPERIODLASTYEAR('Date'[Date])
)
```

```DAX
YoY Sales Growth =
DIVIDE(
    [Total Sales] - [Sales Previous Year],
    [Sales Previous Year]
)
```

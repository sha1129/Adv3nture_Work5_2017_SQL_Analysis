# Queries working with date field

### Order Date Vs Ship Date Q1, 2013
```SQL
SELECT Distinct DATEDIFF(day,OrderDate,ShipDate) AS NumberOfDaysToShip
FROM FactInternetSales
WHERE YEAR(OrderDate) = 2013 and DATEPART(q,OrderDate) = 1
```
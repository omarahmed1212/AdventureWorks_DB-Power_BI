# AdventureWorks_DB-Power_BI
dashboard for AdventureWorks database with Power BI Desktop
Conductivity Mode => DirectQuery

Tables:
Sales.SalesOrderHeader
Sales.SalesOrderDetail
Sales.vSalesPerson (view)
Sales.SalesTerritory
Purchasing.ShipMethod
Production.Product
Production.ProductSubcategory
Production.ProductCategory

Status (Add based on ufnGetSalesOrderStatusText function)
Dates (DAX)

-Rename Tables, columns
-Remove unused columns 

-one table (Merge M Language)
Production.Product
Production.ProductSubcategory
Production.ProductCategory

Contains: PorductID, Product, SubCategory, Category

Solve TotalDue, Tax and Fright by Power Query OR DAX

Modelig:

- Star Schema 
- Product Hierarchy


- line chart vs. counts (USERELATIONSHIP)
orderdate
shipdate
duedate

Model => Star Schema

Measures
- # Orders Measure 
- Total SubTotal Measure 
- Total Tax Measure 
- Total Freight Measure 
- Total Due Measure 
- # Qty

create DAX Measures table that contains all measures

Visuals: (Use Measures)

- Drill Down
- Drill Through 
- Tooltip page

- # Orders Card
- Total SubTotal Card
- Total Tax Card
- Total Freight Card
- Total Due Card

# Orders by OrderDate vs. ShipDate vs. DueDate
# Orders by Status
# Orders by Shipmethod
# Orders by Category, SubCategory, Product
# Orders by FlagOnlineOffline
# Orders vs. TotalDue by Territory
Top 10 Sales Perosns (# Orders or Total Amount) (Filter filter pane)

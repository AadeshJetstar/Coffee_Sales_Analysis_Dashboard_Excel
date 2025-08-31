<img width="1366" height="768" alt="Coffee Sales Dashboard" src="https://github.com/user-attachments/assets/8ef1f559-f0d8-4eb5-88d2-1f915e9b4e74" />

# Coffee_Sales_Analysis_Dashboard_Excel
An interactive Excel dashboard to analyze a coffee shop’s sales across products, categories, time of day, sizes, and locations. Built with PivotTables, slicers, and Power Pivot data model.
✨ Key KPIs (snapshot)
- Total Quantity: 4,933
- Total Transactions: 3,390
- Total Revenue: 15,789


📊 Main Visuals
- Top 10 Products by Quantity
- Distribution by Product Category (Coffee, Tea, Bakery, etc.)
- Hourly Sales by Quantity (peaks in morning)
- Distribution by Product Type (brew methods/styles)
- Size‑wise Sales (Regular, Large, Small, Not Defined)
- Location by Sales (e.g., Astoria, Lower Manhattan, Hell’s Kitchen)


🛠️ Build Steps
1. Load data into Excel tables (Insert ▶ Table). Name them as in the schema above.
2. Add to Data Model (Power Pivot ▶ Add to Data Model) and create relationships.
3. Create measures (DAX):
- `Total Quantity := SUM(FactSales[Quantity])`
- `Total Transactions := DISTINCTCOUNT(FactSales[TransactionID])`
- `Total Revenue := SUMX(FactSales, FactSales[Quantity] * FactSales[Price])`
4. Insert PivotTables linked to the Data Model and build the visuals.
5. Add Slicers for `DimDate[DayName]` and `DimDate[MonthName]`; connect to all PivotTables.
6. Design the dashboard: consistent fonts, spacing, label hierarchy, and soft neutral background.

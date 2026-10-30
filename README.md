# Assignment-4--DAX-and-data-visualisation
Assignment 4- DAX and data visualisation
 Calculated Column for 'Category Type Order Details (2)'[Category]& " "&'Order Details (2)'[Sub-Category]
 Revenue per Order in Order Details Table 'Order Details (2)'[Amount]*'Order Details (2)'[Quantity]
 Calculated Column to Categorize Sales 'Above Average' or 'Below  Average' based on the Amount value.IF('Order Details (2)'[Amount]>AVERAGE('Order Details (2)'[Amount]),"above average","below average")
 Order Count = COUNT('List of Orders (2)'[Order ID])
 Average Profit in Delhi=CALCULATE(AVERAGE('Order Details (2)'[Profit]),'List of Orders (2)'[City]="delhi")
 Year-to-Date (YTD) Sales MAX('List of Orders (2)'[Order Date]),MIN('List of Orders (2)'[Order Date])
 calender = CALENDAR(MIN('List of Orders (2)'[Order Date]),MAX('List of Orders (2)'[Order Date]))
 YTD = TOTALYTD([total sales],calender[Date].[Date])
 Sales Target Achievement by Category, column chart, x axis category, y axis sum of target
 Max Profit Margin by Sub-Category: donut chart, legnd subcategory,values- sum of profit
 Comparison of Profit and Quantity by Sub-Category values subcategory,x axis- sum of profit, y axis - sum of quantity
 Comparison of Total Sales Amount and Target, cards - value sum of amount ,sum of target
 Sales Performance Matrix value sum of target,trend axis category
 Sales Performance Matrix , map - city
 Sales Distribution by Sub-Category tree map category - sub category, values - order count
 Sales Distribution by Sub-Category funnel chart ategory - state, values - order count

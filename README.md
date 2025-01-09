# Power BI Dashboard: Sales and Performance Analysis

## Project Overview  
This Power BI dashboard provides a comprehensive analysis of sales performance, focusing on key metrics such as sales revenue, gross profit, quantity sold, and gross profit percentage (GP%). The report enables stakeholders to identify trends, outliers, and actionable insights, supporting data-driven decision-making.

## Dataset Description  
The dataset used for this analysis consists of three main tables:

1. **Fact Table**: Contains transactional data, including sales, cost of goods sold (COGS), quantity, prices, and timestamps.  
   - **Key columns**: `Product_id`, `Sales_USD`, `Quantity`, `Price_USD`, `COGS_USD`, `Date_Time`, `Account_id`.

2. **Account Table**: Provides details about accounts, geographical information, and related master IDs.  
   - **Key columns**: `Account_id`, `Account`, `Country_code`, `Country2`, `Latitude2`, `Longitude`, `Postal_code`, `Street_name`.

3. **Product Table**: Includes product hierarchy, types, sizes, and group identifiers.  
   - **Key columns**: `Product_Family`, `Product_Group`, `Product_Name`, `Product_Type`, `Product_Size`.

Additionally, a **Date Table** was created to enhance time-based analysis, facilitating drilldowns by year, month, and day.

## Key Insights Visualized  
1. **Overall Performance**  
   - Displayed total sales (YTD), gross profit (GP%), and the difference between this year and the previous year (PYTD).  
   - KPI cards offer a high-level overview of progress against targets.

2. **Bottom 10 Analysis**  
   - A tree map highlights underperforming countries by comparing year-to-date (YTD) performance with the previous year.

3. **Quantity Changes Over Time**  
   - A waterfall chart illustrates monthly variations in quantity sold, segmented by country and product type. This visualization identifies patterns of increase and decrease in sales.

4. **Value and GP% by Account**  
   - A scatter plot correlates sales value (YTD) with gross profit percentages (GP%) across accounts, helping identify high-value customers or accounts needing attention.

5. **Monthly Sales Breakdown**  
   - A clustered column chart shows sales trends by product type (indoor, outdoor, landscape) for each month. A line chart overlays year-to-date vs. previous year comparisons.

## Measures and Calculations  
Custom measures were created to calculate:  
- **YTD Sales**, **PYTD Sales**, and **YTD vs. PYTD** differences.  
- **Gross Profit (GP%)** as `(Sales_USD - COGS_USD) / Sales_USD`.  
- Dynamic slicers and filters were implemented for user interactivity.

## Value Delivered  
This dashboard provides actionable insights by identifying underperforming regions and products, evaluating customer profitability, and tracking sales trends over time. The interactive visuals enable stakeholders to drill down into data for detailed analysis.

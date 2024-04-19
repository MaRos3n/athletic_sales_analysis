# Module 5 challenge: Athletic Sales Analysis 

Instructions taken from the UNC bootcampspot website.

## Background

This project aims to analyze sales data to gain insights into athletic wear sales trends across different cities in the U.S. over two years. The analysis will focus on determining which regions, retailers, and days had the highest sales, as well as identifying the top-selling retailers for women's athletic footwear.

## Combine and Clean the Data

1. Import the CSV files athletic_sales_2020.csv and athletic_sales_2021.csv.
2. Check the column names and data types for consistency.
3. Combine the two DataFrames using an inner join and reset the index.
4. Check for null values and column data types.
5. Convert the "invoice_date" column to a datetime data type.

## Determine which Region Sold the Most Products
1. Create a multi-index DataFrame using either the groupby or pivot_table function with the columns "region", "state", and "city".
2. Rename the aggregated column to reflect the total number of products sold.
3. Sort the results in descending order to show the top five regions with the greatest number of products sold.

## Determine which Region had the Most Sales
1. Use either the groupby or pivot_table function to create a multi-index DataFrame with the columns "region", "state", and "city".
2. Rename the aggregated column to reflect the total sales.
3. Sort the results in descending order to show the top five regions with the highest sales.

## Determine which Retailer had the Most Sales
1. Use either the groupby or pivot_table function to create a multi-index DataFrame with the columns "retailer", "region", "state", and "city".
2. Rename the aggregated column to reflect the total sales.
3. Sort the results in descending order to show the top five retailers along with their region, state, and city that generated the most sales.

## Determine which Retailer Sold the Most Women's Athletic Footwear
1. Filter the combined DataFrame to create a DataFrame with only women's athletic footwear sales data.
2. Use either the groupby or pivot_table function to create a multi-index DataFrame with the columns "retailer", "region", "state", and "city".
3. Rename the aggregated column to reflect the total units sold.
4. Sort the results in descending order to show the top five retailers along with their region, state, and city that sold the most women's athletic footwear.

## Determine the Day with the Most Women's Athletic Footwear Sales
1. Create a pivot table with the "invoice_date" column as the index and the "total_sales" column as the values.
2. Apply the resample function to the pivot table to get the total sales for each day.
3. Sort the results in descending order to show the top 10 days with the most women's athletic footwear sales.

## Determine the Week with the Most Women's Athletic Footwear Sales
1. Apply the resample function to the pivot table created in the previous step to get the total sales for each week.
2. Sort the results in descending order to show the top 10 weeks with the most women's athletic footwear sales.

## References:
- "Pandas DataFrame Documentation." Pandas, PyData, https://pandas.pydata.org/docs/reference/frame.html.
- ChatGPT, OpenAI, https://openai.com/chatgpt.
- Norman, Ryan. UNC AI Bootcamp, Instructor.
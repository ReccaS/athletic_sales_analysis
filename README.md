# Title
Athletic Sales Analysis
# Description
You'll analyze sales data to gain insights into which cities in the U.S. have sold the most athletic wear over two years. 
Next, you'll determine which retailers had the greatest total sales for athletic wear, and which retailers sold the most women's athletic footwear. 
Finally, you'll determine which day and week had the highest sales for women's athletic footwear.
# Installation
**Before You Begin**
Before starting the assignment, be sure to complete the following steps:
  * Create a new repository for this project called athletic_sales_analysis. Do not add this homework assignment to an existing repository
  * Clone the new repository to your computer.
  * Push these changes to GitHub or GitLab.

Download the following file from my repository: starter_code
# Instruction
The starter code provided includes all the steps necessary to complete this challenge.

**Combine and Clean the Data**
 1. Import the two CSV files, athletic_sales_2020.csv and athletic_sales_2021.csv, and read them into DataFrames.
 2. Check that the columns in the two DataFrames have similar names and data types.
 3. Combine the two DataFrames by the rows using an inner join, and reset the index.
 4. After combining the DataFrames, do the following:
     * Check if there are any null values.
     * Check each column’s data type.
     * Convert the "invoice_date" column to a datetime data type.
     * Confirm that the data type has been changed.

**Determine which Region Sold the Most Products**
 1. Use either the groupby or pivot_table function to create a multi-index DataFrame with the "region", "state", and "city" columns.
 2. Rename the aggregated column to reflect the aggregation of the data in the column.
 3. Sort the results in descending order to show the top five regions, including the state and city that have the greatest number of products sold.
 4. Your final table should look like the following image:
    ![image](https://github.com/ReccaS/athletic_sales_analysis/assets/168928543/76821397-ddea-4cb2-87e7-d8546e92791f)

**Determine which Region had the Most Sales**
 1. Use either the groupby or pivot_table function to create a multi-index DataFrame with the "region", "state", and "city" columns.
 2. Rename the aggregated column to reflect the aggregation of the data in the column.
 3. Sort the results in descending order to show the top five regions, including the state and city that generated the most sales. Your final table should look like the following image:
    ![image](https://github.com/ReccaS/athletic_sales_analysis/assets/168928543/80e19da2-9a29-4eb9-a238-11be96167152)

**Determine which Retailer had the Most Sales**
 1. Use either the groupby or pivot_table function to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns.
 2. Rename the aggregated column to reflect the aggregation of the data in the column.
 3. Sort the results in descending order to show the top five retailers along with their region, state, and city that generated the most sales. Your final table should look like the following image:
    ![image](https://github.com/ReccaS/athletic_sales_analysis/assets/168928543/82000b19-46d5-4577-ac08-bc31b29a1c72)

**Determine which Retailer Sold the Most Women's Athletic Footwear**
 1. Filter the combined DataFrame to create a DataFrame with only women's athletic footwear sales data.
 2. Use either the groupby or pivot_table function to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns.
 3. Rename the aggregated column to reflect the aggregation of the data in the column.
 4. Sort the results in descending order to show the top five retailers along with their region, state, and city that sold the most women's athletic footwear. Your final table should look like the following image:
    ![image](https://github.com/ReccaS/athletic_sales_analysis/assets/168928543/f84ec714-e11d-4211-bbaa-187cb4137e2b)

**Determine the Day with the Most Women's Athletic Footwear Sales**
 1. Create a pivot table with the "invoice_date" column as the index and the "total_sales" column as the values parameter.
 2. Rename the aggregated column to reflect the aggregation of the data in the column.
 3. Apply the resample function to the pivot table, place the data into daily bins, and get the total sales for each day.
 4. Sort the resampled DataFrame in descending order to show the top 10 days that generated the most women's athletic footwear sales. Your final table should look like the following image:
    ![image](https://github.com/ReccaS/athletic_sales_analysis/assets/168928543/a45c9a7f-b3c6-4dad-841a-9e6d3dbde6c7)

**Determine the Week with the Most Women's Athletic Footwear Sales**
 1. Apply resample to the pivot table above, place the data into weekly bins, and get the total sales for each week.
 2. Sort the resampled DataFrame in descending order to show the top 10 weeks that generated the most women's athletic footwear sales.
 3.  Your final table should look like the following image:
    ![image](https://github.com/ReccaS/athletic_sales_analysis/assets/168928543/bc6f02b2-03ac-4846-9892-817ce0969c83)
     
# References
Sales Product Data. Available: https://www.kaggle.com/datasets/knightbearr/sales-product-dataLinks to an external site.
The sales product data above was modified by edX Boot Camps LLC, and is intended for educational purposes only.



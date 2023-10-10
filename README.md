# Home_Sales

In this challenge, I used my knowledge of SparkSQL to determine key metrics about home sales data, such as:
  -  What is the average price for a four-bedroom house sold for each year?
  -  What is the average price of a home for each year it was built that has three bedrooms and three bathrooms?
  -  What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater         than or equal to 2,000 square feet?
  -  What is the "view" rating for homes costing more than or equal to $350,000? (Determine the run time for this query).
  -  Please note: all of the above calculations were rounded off to two decimal places.

I created and cached the temporary table 'home_sales' and using the cached data, ran the query that filters out the view ratings with an average price of greater than or equal to $350,000. I determined the runtime and compared it to the uncached runtime and proceeded with the following steps:
  -  Partition by the "date_built" field on the formatted parquet home sales data.
  -  Create a temporary table for the parquet data.
  -  Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the      runtime and compare it to uncached runtime.
  -  Uncache the home_sales temporary table.
  -  Verify that the home_sales temporary table is uncached using PySpark.


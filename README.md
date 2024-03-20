# Home_Sales

## Overview
### In this module I will use SparkSQL to determine key metrics about home sales data.   I will use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached. 

## Instructions
### I will import home_sales_revised.csv data into a Spark DataFrame called home_sales.  Using SparkSQL I will answer the following questions:

1. What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
![image](https://github.com/eferna1/Home_Sales/assets/145945547/79ab8ca5-939f-4f99-ae3f-e970d79c8213)

2. What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
   
![image](https://github.com/eferna1/Home_Sales/assets/145945547/0d318638-5155-4920-a6a2-730115b15aa2)

3. What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
![image](https://github.com/eferna1/Home_Sales/assets/145945547/cbec9b97-ed5f-42f5-aa76-276741d88efb)

4. What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
![image](https://github.com/eferna1/Home_Sales/assets/145945547/a09b725d-753f-4f59-8658-95012a162dd3)

### After answering the above questions: 
-> Cache the temporary table.

-> Check if your temporary table is cached.

![image](https://github.com/eferna1/Home_Sales/assets/145945547/1ca10d43-8d75-4adb-88c4-47dfd3046151)

-> Using the cached data, will rull the last query that calculates the average price of a home per "view" rating having an average home price greate than or equal to $350,000.  Determine the runtime and compare it to uncached runtime. 

![image](https://github.com/eferna1/Home_Sales/assets/145945547/15b8c828-16dd-4c2e-a57d-4d31a76550ad)

-> Partition by the "data_built" field on the fomratted parquet home sales data. 

-> Create a temporary table for the parquet data. 
![image](https://github.com/eferna1/Home_Sales/assets/145945547/cca4cd40-c494-400b-81cb-25d4b0dd87f6)

-> Run the last query that calculates the average price of a home per "view" rating having an average home price greate than or equal to $350,000.   Determine the runtime and compare it to uncached runtime. 
![image](https://github.com/eferna1/Home_Sales/assets/145945547/39c006ea-d8cb-4a8b-8e48-b370a38699db)

-> Uncache the home_sales temporary table. 

-> Verify that the home_sales temporary table is uncached using PySpark. 

![image](https://github.com/eferna1/Home_Sales/assets/145945547/9e422e5e-01e3-44d4-b1a0-f2ce90f17e6e)



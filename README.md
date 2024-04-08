# Home_Sales
Module 22 Challenge

**Goal:** Use SparkSQL to identify key metrics about home sales data. Spark used to create temporary views, patition the data, cache/uncache a temporary table, and verify uncached. These steps explore methods of data saving that allows for shorter processing times.

**Requested measures:**
- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

```
+----+---------+
|year|avg_price|
+----+---------+
|2022|296363.88|
|2021|301819.44|
|2020|298353.78|
|2019| 300263.7|
+----+---------+
```

- What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

```
+----+---------+
|year|avg_price|
+----+---------+
|2022|292725.69|
|2021|294211.46|
|2020|294204.16|
|2019|287287.82|
+----+---------+
```

- What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.


- What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
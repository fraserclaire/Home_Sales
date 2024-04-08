# Home Sales - Module 22 Challenge

**Goal:** Use SparkSQL to identify key metrics about home sales data. Spark used to create temporary views, patition the data, cache/uncache a temporary table, and verify uncached. These steps explore methods of data saving that allows for shorter processing times.

### Time differences
- Original: 1.11 seconds
- From cache: 0.678 seconds
- From parquet: 0.485 seconds
Saving ~40% time by using cache, ~60% using parquet.

### Requested measures:
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
```
+----+---------+
|year|avg_price|
+----+---------+
|2022|290242.99|
|2021|296330.96|
|2020|292289.09|
|2019|289859.14|
+----+---------+
```

- What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
```
+----------+
| avg_price|
+----------+
|1061201.42|
|1053739.33|
|1129040.15|
|1017815.92|
| 1054325.6|
| 1033536.2|
|1026006.06|
| 970402.55|
|1137372.73|
|1062654.16|
| 401393.34|
|1107839.15|
|1031719.35|
| 1072285.2|
|1070444.25|
|1056336.74|
|1117233.13|
|1033965.93|
| 1063498.0|
|1053472.79|
+----------+
```

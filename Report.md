# Lab 3: Spark and Parquet Optimization Report

Name:
 
NetID: 

## Part 1: Spark

#### Question 1: 
How would you express the following computation using SQL instead of the object interface: `sailors.filter(sailors.rating > 6).select(sailors.sid, sailors.sname, sailors.age)`?

Code:
```SQL

<your_query_here>

```


Output:
```

<copy_resulting_table_from_stdout_here>

```


#### Question 2: 
How would you express the following using the object interface instead of SQL: `spark.sql('SELECT sid, COUNT(bid) from reserves WHERE bid != 101 GROUP BY sid')`?

Code:
```python

<your_Spark_Transformations_here>

```


Output:
```

<copy_resulting_table_from_stdout_here>

```

#### Question 3: 
Using SQL and (multiple) inner joins, in a single query, how many distinct boats did each sailor reserve? 
The resulting DataFrame should include the sailor's id, name, and the count of distinct boats. 
(Hint: you may need to use `first(...)` aggregation function on some columns.) 
Provide both your query and the resulting DataFrame in your response to this question.

Code:
```SQL

<your_SQL_query_here>

```


Output:
```

<copy_resulting_table_from_stdout_here>

```

#### Question 4: 
Repeating the analysis from Q6.2 in Lab2, implement a query using Spark transformations
which finds for each artist term, compute the minimum year of release,
average track duration, and the total number of artists for that term (by ID).
What are the results for the ten terms with the longest average track durations?  
Include both your query code and resulting DataFrame in your response.

Code:
```python

<your_Spark_Transformations_here>

```


Output:
```

<copy_resulting_table_from_stdout_here>

```
#### Question 5: 
Create a query using Spark transformations that finds the number of distinct tracks associated
(through artistID) to each term.  Modify this query to return only the top 10 most popular terms, and again for the bottom 10.
Include each query and the tables for the top 10 most popular terms and the 10 least popular terms in your response. 

##### 10 Most Popular Terms
Code:
```

<your_Spark_Transformations_here>

```
Output:
```

<copy_resulting_table_from_stdout_here>

```

##### 10 Least Popular Terms
Code:
```

<your_Spark_Transformations_or_SQL_query_here>

```

Output:
```

<copy_resulting_table_from_stdout_here>

```

## Part 2: Parquet Optimization:

What to include in your report:
  - Tables of all numerical results (min, max, median) for each query/size/storage combination for part 2.3, 2.4 and 2.5.
  - How do the results in parts 2.3, 2.4, and 2.5 compare?
  - What did you try in part 2.5 to improve performance for each query?
  - What worked, and what didn't work?

Basic Markdown Guide: https://www.markdownguide.org/basic-syntax/

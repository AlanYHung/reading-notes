# Code 301
## Reading 08
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)


### Complete SQLBolt
[Article Source](http://sqlbolt.com/)
* SQL stands for Structured Query Language
* SQL allows users to query databases and pull back data in the way they need/want to use it
* SQL Lesson 1: SELECT queries 101
  * Select Statements allow you to choose what data you want pull from the database
* SQL Lesson 2: Queries with constraints (Pt. 1)
  * Where Clause allows you to filter data via conditional statements
    1. AND
    1. OR
    1. BETWEEN...AND...
    1. NOT BETWEEN...AND...
    1. IN(...)
    1. NOT IN (...)
* SQL Lesson 3: Queries with constraints (Pt. 2)
  * The conditional statements use the following operators
    1. =
    1. != or <>
    1. LIKE
    1. NOT LIKE
    1. %
    1. -
* SQL Lesson 4: Filtering and sorting Query results
  * DISTINCT lets you get all unique values from a set of data
  * ORDER BY lets you sort the data by a specific set of data in asc or desc sort
  * LIMIT will allow you to tell how many rows to retrieve
  * OFFSET will allow you to tell the query which row to start pulling the data from
* SQL Review: Simple SELECT Queries
* SQL Lesson 6: Multi-table queries with JOINs
  * Joins allow you to merge the merge relational data from multiple sources by using a key value
  * INNER JOIN combines the data from both tables but does not return non-matching rows from either table
* SQL Lesson 7: OUTER JOINs
  * LEFT JOIN joins the data from the 2nd table to the first table
  * RIGHT JOIN joins the data from the 1st table to the 2nd table
  * FULL JOIN joins both data sets fully whether data matches or not
* SQL Lesson 8: A short note on NULLs
  * NULL is are undefined values in a table
  * Can be handled through joining or in a where clause with IS NULL and IS NOT NULL
* SQL Lesson 9: Queries with expressions
  * AS can give a descriptive alias to an table element
* SQL Lesson 10: Queries with aggregates (Pt. 1)
  * Aggregate functions can summarize a set of rows
  * Aggregate Functions:
    1. COUNT()
    1. MIN()
    1. MAX()
    1. AVG()
    1. SUM()
  * Aggregate Functions can be grouped using GROUP BY
* SQL Lesson 11: Queries with aggregates (Pt. 2)
  * You can use HAVING to filter the grouped data
* SQL Lesson 12: Order of execution of a Query
  * Order of Operations:
    1. FROM / JOIN
    1. WHERE
    1. GROUP BY
    1. HAVING
    1. SELECT
    1. DISTINCT
    1. ORDER BY
    1. LIMIT / OFFSET
* SQL Lesson 13: Inserting rows
  * INSERT INTO to add data to table
* SQL Lesson 14: Updating rows
  * UPDATE allows you to update specific data in a dataset
* SQL Lesson 15: Deleting rows
  * DELETE lets you delete data from a server
* SQL Lesson 16: Creating tables
  * CREATE TABLE lets you create a new table
  * IF NOT EXISTS handles and skips creating tables in case of errors
  * Data Types:
    1. INTEGER
    1. BOOLEAN
    1. FLOAT
    1. DOUBLE
    1. REAL
    1. CHARACTER
    1. VARCHAR
    1. TEXT
    1. DATE
    1. DATETIME
    1. BLOB
  * Table Constraints
    1. PRIMARY KEY
    1. AUTOINCREMENT
    1. UNIQUE
    1. NOT NULL
    1. CHECK
    1. FOREIGN KEY
* SQL Lesson 17: Altering tables
  * FIRST and AFTER specify where to insert rows
  * DROP lets you remove full columns
  * RENAME TO lets you rename the table
* SQL Lesson 18: Dropping tables
  * DROP TABLE lets you delete tables
  * IF EXISTS can be used to check if a table exists



### Practice SQL on W3Schools
[Article Source](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all)
* Things you can practice:
  * Select
  * From
  * Join
  * Union
  * Order By
  * Where
  * Group By


### Additional SQL Resources
* [A Primer on SQL - Click the blue Download button](https://openlibra.com/en/book/a-primer-on-sql-3rd-edition)
* [SQL Cheat Sheet](http://www.cheat-sheets.org/sites/sql.su/)


[<-- Back](../README.md)

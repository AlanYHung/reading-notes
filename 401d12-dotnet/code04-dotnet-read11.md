# Code 401
## Reading 11
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)

<br>
<br>
<br>

### Summary
* C# allows you to create complex data models where you can manipulate the data type, declare variables as columns, make them required, and make them keys.
* This enables you to create database like data models with relationships via code, and be queried.
* A Database Schema is a default skeleton structure that can be used to standardize and conform new database instantiations based on your programs needs.
* There are multiple types of keys a database can have.  Among them are Primary, Foreign, and Composite Keys.
  * Primary Keys are the key values assigned to each row of data in a database table by default as a way to identify/access each row of data.
  * Foreign Keys are key values taken from a table by another table in order to create a relationship between the 2 tables.  This enables you to query data from 2 different tables with 1 query.
  * Composite keys are keys derived from 2 or more different column values in order to help create a unique key for that table to relate to another database to help enable/simplify querying the 2 tables.
* When relating databases together, they can be said to have a specified type of relationship.
  * 1:1 relationship means that both sides have only 1 value that equals each other, so if you filter by that specific value/key on each table they will each return only 1 result.
  * Many:Many relationship is when both tables have multiple values that equal a specific value/key.  This means that if you try filtering on that value/key on each table, they will both return multiple results.
  * Many:1 / 1:Many means that 1 table has a single value and another table has multiple values that equal to a value/key.  This means that if you filter each table for that value/key, 1 table will will return a single result and another table will return multiple results. 

<br>
<br>

### Resources
* #### __Tutorial: Create a complex data model - ASP.NET MVC with EF Core__
  * ##### Author:  Microsoft Docs
  * ##### [Article Source](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/complex-data-model?view=aspnetcore-2.0)

* #### __DBMS - Overview__
  * ##### Author:  Tutorials Point: Simply Easy Learning
  * ##### [Article Source](https://www.tutorialspoint.com/dbms/dbms_overview.htm)

<br>
<br>
<br>

[<-- Back](../README.md)

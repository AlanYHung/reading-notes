# Code 301
## Reading 14
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)


### Database Normalization (Explained in Simple English)
#### Author:  Kris Wenzel
[Article Source](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)
> Database normalization is a process used to organize a database into tables and columns.
> ###### (Quoted from Article)


* Every table should be used for one purpose
  * This prevents data duplication
* 3 Reasons to normalize databases:
  1. Minimize duplicate data
  1. Makes table modifications easier and less prone to issues
  1. Simplify Queries


* 3 common forms of database normalization:
  > * 1NF - The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
  > * 2NF - The table is in first normal form and all the columns depend on the table’s primary key.
  > * 3NF - the table is in second normal form and all of its columns are not transitively dependent on the primary key
  > ###### (Quoted from Article)






[<-- Back](../README.md)

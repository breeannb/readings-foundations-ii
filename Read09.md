# Read 09: SQL Relations and Joins

## [Complete SQLBolt (Lessons 5-8](https://sqlbolt.com/)
> * Multi-table queries with JOINs
```
Select query with INNER JOIN on multiple tables
SELECT column, another_table_column, …
FROM mytable
INNER JOIN another_table 
    ON mytable.id = another_table.id
WHERE condition(s)
ORDER BY column, … ASC/DESC
LIMIT num_limit OFFSET num_offset
```
> * You might see queries where the INNER JOIN is written simply as a JOIN. These two are equivalent, but we will continue to refer to these joins as inner-joins because they make the query easier to read once you start using other types of joins, which will be introduced in the following lesson.
> * SQL Lesson 7: Outer Joins
```
Select query with LEFT/RIGHT/FULL JOINs on multiple tables
SELECT column, another_column, …
FROM mytable
INNER/LEFT/RIGHT/FULL JOIN another_table 
    ON mytable.id = another_table.matching_id
WHERE condition(s)
ORDER BY column, … ASC/DESC
LIMIT num_limit OFFSET num_offset;
```
>   * When joining table A to table B, a LEFT JOIN simply includes rows from A regardless of whether a matching row is found in B.
>   * The RIGHT JOIN is the same, but reversed, keeping rows in B regardless of whether a match is found in A.
>   * Finally, a FULL JOIN simply means that rows from both tables are kept, regardless of whether a matching row exists in the other table.
>   * You might see queries with these joins written as LEFT OUTER JOIN, RIGHT OUTER JOIN, or FULL OUTER JOIN, but the OUTER keyword is really kept for SQL-92 compatibility and these queries are simply equivalent to LEFT JOIN, RIGHT JOIN, and FULL JOIN respectively.
> * A short note on NULLs
>   * An alternative to NULL values in your database is to have data-type appropriate default values, like 0 for numerical data, empty strings for text data, etc. But if your database needs to store incomplete data, then NULL values can be appropriate if the default values will skew later analysis (for example, when taking averages of numerical data).
>   * Sometimes, it's also not possible to avoid NULL values, as we saw in the last lesson when outer-joining two tables with asymmetric data. In these cases, you can test a column for NULL values in a WHERE clause by using either the IS NULL or IS NOT NULL constraint.
```
SELECT column, another_column, …
FROM mytable
WHERE column IS/IS NOT NULL
AND/OR another_condition
AND/OR …;
```

## [Database Normalization Explained in Simple English](https://canvas.instructure.com/courses/1968689/assignments/14846186/submissions/25726594)
> * Database normalization is a process used to organize a database into tables and columns. 
> * Resons to normalize a database: 
>   * minimize duplicate data
>   * minimize or avoid data modification issues
>   * simplify queries
> * Data Duplication and Modification Anomalies
>   * Duplicated information presents two problems:
>       * It increases storage and decrease performance.
>       * It becomes more difficult to maintain data changes
* Definition of Database Normalization
>   * There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively. 
>       * First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
>       * Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
>       * Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key
* Data Duplication and Modification Anomalies

## [Visual Representation of SQL Joins](https://www.codeproject.com/Articles/33052/Visual-Representation-of-SQL-Joins)

## [Reference](https://ia801302.us.archive.org/6/items/aprimeronsql/aprimeronsql.pdf)
# Read 08: SQL

## [Introduction to SQL](https://sqlbolt.com/)
> * SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.
> * A relational database represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.
> * Lesson 1: Select Queries
>   * To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries. A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned.
>   * And given a table of data, the most basic query we could write would be one that selects for a couple columns (properties) of the table with all the rows (instances).
```
Select query for a specific columns
SELECT column, another_column, …
FROM mytable;
```
>   * The result of this query will be a two-dimensional set of rows and columns, effectively a copy of the table, but only with the columns that we requested.
>   * If we want to retrieve absolutely all the columns of data from a table, we can then use the asterisk (*) shorthand in place of listing all the column names individually.
```
Select query for all columns
SELECT * 
FROM mytable;
```
>   * This query, in particular, is really useful because it's a simple way to inspect a table by dumping all the data at once.
> * SQL Lesson 2: Queries with constraints (Pt. 1)
>   * n order to filter certain results from being returned, we need to use a WHERE clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not.
```
Select query with constraints
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```
>   * More complex clauses can be constructed by joining numerous AND or OR logical keywords (ie. num_wheels >= 4 AND doors <= 2). And below are some useful operators that you can use for numerical data (ie. integer or floating point):
>   * Please see assetts folder for operator table
> * SQL Lesson 3: Queries with constraints (Pt. 2)
>   * When writing WHERE clauses with columns containing text data, SQL supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching.
```
Select query with constraints
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;

```

> * SQL Lesson 4: Filtering and sorting Query results
>   * Even though the data in a database may be unique, the results of any particular query may not be – take our Movies table for example, many different movies can be released the same year. In such cases, SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.
``` 
Select query with unique results
SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);
```
>   * Since the DISTINCT keyword will blindly remove duplicate rows, we will learn in a future lesson how to discard duplicates based on specific columns using grouping and the GROUP BY clause.
>   * Ordering results
>       * Unlike our neatly ordered table in the last few lessons, most data in real databases are added in no particular column order. As a result, it can be difficult to read through and understand the results of a query as the size of a table increases to thousands or even millions rows.
>       *  To help with this, SQL provides a way to sort your results by a given column in ascending or descending order using the ORDER BY clause.
```
Select query with ordered results
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC;
```
>   * When an ORDER BY clause is specified, each row is sorted alpha-numerically based on the specified column's value. In some databases, you can also specify a collation to better sort data containing international text.
>   * Limiting results to a subset
>       * Another clause which is commonly used with the ORDER BY clause are the LIMIT and OFFSET clauses, which are a useful optimization to indicate to the database the subset of the results you care about.
The LIMIT will reduce the number of rows to return, and the optional OFFSET will specify where to begin counting the number rows from.


> * SQL Lesson 13: Inserting rows
>   * What is a Schema?
>       * In SQL, the database schema is what describes the structure of each table, and the datatypes that each column of the table can contain.
>   * Inserting new data
>       * When inserting data into a database, we need to use an INSERT statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert.
```
Insert statement with values for all columns
INSERT INTO mytable
VALUES (value_or_expr, another_value_or_expr, …),
       (value_or_expr_2, another_value_or_expr_2, …),
       …;
```
```
Insert statement with specific columns
INSERT INTO mytable
(column, another_column, …)
VALUES (value_or_expr, another_value_or_expr, …),
      (value_or_expr_2, another_value_or_expr_2, …),
      …;
```

```
Example Insert statement with expressions
INSERT INTO boxoffice
(movie_id, rating, sales_in_millions)
VALUES (1, 9.9, 283742034 / 1000000);
```

## [Practice SQL on W3 Schools - This resource has sample databases you can use to practice writing SQL queries](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all)


## [A Primer on SQL](https://openlibra.com/en/book/download/a-primer-on-sql-3rd-edition)
> * https://canvas.instructure.com/courses/1968689/assignments/14846187/submissions/25726594

## [SQL Cheat Sheet](http://www.cheat-sheets.org/sites/sql.su/)

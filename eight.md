What is SQL?
SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

Queries with constraints
In order to filter certain results from being returned, we need to use a WHERE clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not.


Relational databases
A relational database represents a collection of related (two-dimensional) tables. with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.

SELECT queries
To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially referred to as queries.

the most basic query we could write would be one that selects for a couple columns (properties) of the table with all the rows (instances).

Select query for a specific columns :

SELECT column, another_column, etc...
FROM mytable;
"two-dimensional set of rows and columns, effectively a copy of the table, but only with the columns that we requested."

Select query for all columns

SELECT *
FROM mytable;
"inspect a table by dumping all the data at once."


OUTER JOINs
If the two tables have asymmetric data, which can easily happen when data is entered in different stages, then we would have to use a LEFT JOIN, RIGHT JOIN or FULL JOIN instead to ensure that the data you need is not left out of the results.

Select query with LEFT/RIGHT/FULL JOINs on multiple tables

SELECT column, another_column, …
FROM mytable
INNER/LEFT/RIGHT/FULL JOIN another_table
ON mytable .id = another_table.matching_id
WHERE condition(s)
ORDER BY column, … ASC/DESC
LIMIT num_limit OFFSET num_offset;
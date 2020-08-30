# SQL

## CHEATSHEET

> SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database

- A relational database represents a collection of related (two-dimensional) tables

- To retrieve data from a SQL database, we need to write `SELECT` statements

> Select query for a specific columns
> `SELECT` column, another_column, …
> `FROM` mytable

If we want to retrieve absolutely all the columns of data from a table, we can then use the asterisk `(*)` shorthand in place of listing all the column names individually

### Queries with constraints

- In order to filter certain results from being returned, we need to use a `WHERE` clause
  - The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not

Select query with constraints
`SELECT` column, another_column, …
`FROM` mytable
`WHERE` condition
    `AND/OR` another_condition
    `AND/OR` …;

- We should note that while most database implementations are quite efficient when using these operators, full-text search is best left to dedicated libraries like **Apache Lucene** or **Sphinx**


# Create Schema

-`CREATE SCHEMA schema_name;`

Or  

-`CREATE SCHEMA [IF NOT EXISTS] schema_name;`


-`CREATE SCHEMA employee;`

# Create Schema with ownership

-` CREATE SCHEMA schemaname [ AUTHORIZATION username ] [ schema_element [ ..... ] ]`


# Create Schema with object

-`schema_name.table_name`

-`public.customer`
or
-`marketing.customer`


# Public Schema

-`CREATE TABLE table_name;`
and
-`CREATE TABLE public.table_name;`

# Rename Schema

-`ALTER SCHEMA old_name RENAME TO new_name;`
-`ALTER SCHEMA staff to employees;`

# Alter Owner of Schema

-` ALTER SCHEMA schema_name
OWNER TO { new_owner | CURRENT_USER | SESSION_USER};`

-`ALTER SCHEMA staff
OWNER TO kate;`

# Drop Schema

-`DROP SCHEMA [ IF EXISTS ] name [, ...] [ CASCADE | RESTRICT ] `

-`DROP SCHEMA IF EXISTS sales;`

# Drop Schema with Object

-`DROP SCHEMA schema_name CASCADE; `

-`DROP SCHEMA sales CASCADE;`

# Create Schema Owned by Someone Else

-`CREATE SCHEMA schema_name AUTHORIZATION user_name; `

# Drop Table

-`DROP TABLE mytable;`

# Revoke Privileges

-`REVOKE CREATE ON SCHEMA public FROM PUBLIC;`

# Create Role

-`CREATE ROLE role_name; `


# Create New Role with Username and Password

-`CREATE ROLE username NOINHERIT LOGIN PASSWORD password;`

# Change Role for the Current Session

-`SET ROLE new_role;`

# Allow role 1 to be role 2

-`GRANT role_2 TO role_1;`

# Create DB

-`CREATE DATABASE [IF NOT EXISTS] db_name; `

# Drop DB

-`DROP DATABASE [IF EXISTS] db_name; `

# Create Table

-`CREATE [TEMP] TABLE [IF NOT EXISTS] table_name(
pk SERIAL PRIMARY KEY,
c1 type(size) NOT NULL,
c2 type(size) NULL,
...
);`


# Alter Column

- `ALTER TABLE table_name ALTER COLUMN column_name new_data_type;`

# Add New Column

-`ALTER TABLE table_name ADD COLUMN new_column_name TYPE; `

# Drop Column

-`ALTER TABLE table_name DROP COLUMN column_name; `

# Rename Column

-`ALTER TABLE table_name RENAME column_name TO new_column_name; `

# Set or Remove Default Column

-`ALTER TABLE table_name ALTER COLUMN [SET DEFAULT value | DROP DEFAULT] `

# Add Primary Key

-`ALTER TABLE table_name ADD PRIMARY KEY (column,...); `

# Remove Primary Key from Table

-`ALTER TABLE table_name
DROP CONSTRAINT primary_key_constraint_name; `

# Rename Table

-`ALTER TABLE table_name RENAME TO new_table_name; `

# Drop Table

-` DROP TABLE [IF EXISTS] table_name CASCADE; `

# Create View

-`CREATE OR REPLACE view_name AS
query; `

# Create Recursion View

-`CREATE RECURSIVE VIEW view_name(column_list) AS
SELECT column_list; `

# Create Materialized View

-`CREATE MATERIALIZED VIEW view_name
AS
query
WITH [NO] DATA; `

# Refresh Materialized View

-`REFRESH MATERIALIZED VIEW CONCURRENTLY view_name;`

# Drop a View

-`DROP VIEW [ IF EXISTS ] view_name; `

# Rename a View

-`ALTER VIEW view_name RENAME TO new_name;`

# Create an Index with Specific Name on a Table

-`CREATE [UNIQUE] INDEX index_name
ON table (column,...) `

# Remove a Specific Index from Table

-`DROP INDEX index_name; `

# Query All Data

-`SELECT * FROM table_name; `

# Query All Data from Specific Column

-`SELECT column_list
FROM table; `

# Query All Data from Specific Row

-`SELECT DISTINCT (column)
FROM table; `

# Query with Filter

-`SELECT *
FROM table
WHERE condition; `

# Assign an Alias to a Column

-`SELECT column_1 AS new_column_1, ...
FROM table;
`
# Query Data using LIKE Operator

-` SELECT * FROM table_name
WHERE column LIKE '%value%'`

# Query Data using BETWEEN Operator

-`SELECT * FROM table_name
WHERE column BETWEEN low AND high; `

# Query Data using IN Operator

-`SELECT * FROM table_name
WHERE column IN (value1, value2,...); `

# Constrain the Returned Rows with the LIMIT Clause:

-`SELECT * FROM table_name
LIMIT limit OFFSET offset
ORDER BY column_name; `

# Query Data from Multiple using the Inner Join, Left Join, Full Outer Join, Cross Join and Natural Join

-`SELECT * 
FROM table1
INNER JOIN table2 ON conditions `

-`SELECT * 
FROM table1
LEFT JOIN table2 ON conditions `

-`SELECT * 
FROM table1
FULL OUTER JOIN table2 ON conditions `

-`SELECT * 
FROM table1
CROSS JOIN table2; `

-`SELECT * 
FROM table1
NATURAL JOIN table2; `

# Return the Number of Rows of a Table

-`SELECT COUNT (*)
FROM table_name; `

# Sort Rows in Ascending or Descending Order

-`SELECT select_list
FROM table
ORDER BY column ASC [DESC], column2 ASC [DESC],...; `

# Group rows using GROUP BY clause

-`SELECT *
FROM table
GROUP BY column_1, column_2, ...; `

# Filter Groups using the HAVING Clause

-`SELECT *
FROM table
GROUP BY column_1
HAVING condition; `


>## Set Operators
# Combine the Result set of Two or More Queries with UNION Operator

-`SELECT * FROM table1
UNION
SELECT * FROM table2; `

# Minus a result set using EXCEPT operator

-`SELECT * FROM table1
EXCEPT
SELECT * FROM table2; `

# Get intersection of the result sets of two queries

-`SELECT * FROM table1
INTERSECT
SELECT * FROM table2; `


>## Modifying Data
# Insert a new row into a table

-`INSERT INTO table(column1,column2,...)
VALUES(value_1,value_2,...); `

# Insert multiple rows into a table

-`INSERT INTO table_name(column1,column2,...)
VALUES(value_1,value_2,...),
(value_1,value_2,...),
(value_1,value_2,...)...`

# Update data for all rows

-`UPDATE table_name
SET column_1 = value_1,
...; `

# Update data for a set of rows specified by a condition in the WHERE clause

-`UPDATE table
SET column_1 = value_1,
...
WHERE condition; `

# Delete all rows of a table

-`DELETE FROM table_name; `

# Delete specific rows based on a condition

-`DELETE FROM table_name
WHERE condition; `


>## Performance
# Show the query plan for a query

-`EXPLAIN query; `

# Show and execute the query plan for a query

-`EXPLAIN ANALYZE query; `

# Collect statistics

-`ANALYZE table_name; `

__ __
-` `


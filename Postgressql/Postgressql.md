__Create Schema__

-`CREATE SCHEMA schema_name;`
Or  
-`CREATE SCHEMA [IF NOT EXISTS] schema_name;`

-`CREATE SCHEMA employee;`

__Create Schema with ownership__
-` CREATE SCHEMA schemaname [ AUTHORIZATION username ] [ schema_element [ ..... ] ]`

__Create Schema with object__
-`schema_name.table_name`

-`public.customer`
or
-`marketing.customer`

__Public Schema__
-`CREATE TABLE table_name;`
and
-`CREATE TABLE public.table_name;`

__Rename Schema__
-`ALTER SCHEMA old_name RENAME TO new_name;`
-`ALTER SCHEMA staff to employees;`

__Alter Owner of Schema__
-` ALTER SCHEMA schema_name
OWNER TO { new_owner | CURRENT_USER | SESSION_USER};`
-`ALTER SCHEMA staff
OWNER TO kate;`

__Drop Schema__
-`DROP SCHEMA [ IF EXISTS ] name [, ...] [ CASCADE | RESTRICT ] `
-`DROP SCHEMA IF EXISTS sales;`

__Drop Schema with Object__
-`DROP SCHEMA schema_name CASCADE; `
-`DROP SCHEMA sales CASCADE;`

__Create Schema Owned by Someone Else__
-`CREATE SCHEMA schema_name AUTHORIZATION user_name; `

__Drop Table__
-`DROP TABLE mytable;`

__Revoke Privileges__
-`REVOKE CREATE ON SCHEMA public FROM PUBLIC;`

__Create Role__
-`CREATE ROLE role_name; `


__Create New Role with Username and Password__
-`CREATE ROLE username NOINHERIT LOGIN PASSWORD password;`

__Change Role for the Current Session__
-`SET ROLE new_role;`

__Allow role 1 to be role 2__
-`GRANT role_2 TO role_1;`

__Create DB__
-`CREATE DATABASE [IF NOT EXISTS] db_name; `

__Drop DB__
-`DROP DATABASE [IF EXISTS] db_name; `

__Create Table__
-`CREATE [TEMP] TABLE [IF NOT EXISTS] table_name(
pk SERIAL PRIMARY KEY,
c1 type(size) NOT NULL,
c2 type(size) NULL,
...
);`

__Add New Column__
-`ALTER TABLE table_name ADD COLUMN new_column_name TYPE; `

__Drop Column__
-`ALTER TABLE table_name DROP COLUMN column_name; `

__Rename Column__
-`ALTER TABLE table_name RENAME column_name TO new_column_name; `

__Set or Remove Default Column__
-`ALTER TABLE table_name ALTER COLUMN [SET DEFAULT value | DROP DEFAULT] `

__Add Primary Key__
-`ALTER TABLE table_name ADD PRIMARY KEY (column,...); `

__Remove Primary Key from Table__
-`ALTER TABLE table_name
DROP CONSTRAINT primary_key_constraint_name; `

__Rename Table__
-`ALTER TABLE table_name RENAME TO new_table_name; `

__Drop Table__
-` DROP TABLE [IF EXISTS] table_name CASCADE; `

__Create View__
-`CREATE OR REPLACE view_name AS
query; `

__Create Recursion View__
-`CREATE RECURSIVE VIEW view_name(column_list) AS
SELECT column_list; `

__Create Materialized View__
-`CREATE MATERIALIZED VIEW view_name
AS
query
WITH [NO] DATA; `

__Refresh Materialized View__
-`REFRESH MATERIALIZED VIEW CONCURRENTLY view_name;`

__Drop a View__
-`DROP VIEW [ IF EXISTS ] view_name; `

__Rename a View__
-`ALTER VIEW view_name RENAME TO new_name;`

__Create an Index with Specific Name on a Table__
-`CREATE [UNIQUE] INDEX index_name
ON table (column,...) `

__Remove a Specific Index from Table__
-`DROP INDEX index_name; `

__Query All Data__
-`SELECT * FROM table_name; `

__Query All Data from Specific Column__
-`SELECT column_list
FROM table; `

__Query All Data from Specific Row__
-`SELECT DISTINCT (column)
FROM table; `

__Query with Filter__
-`SELECT *
FROM table
WHERE condition; `

__Assign an Alias to a Column__
-`SELECT column_1 AS new_column_1, ...
FROM table;
`
__Query Data using LIKE Operator__
-` SELECT * FROM table_name
WHERE column LIKE '%value%'`

__Query Data using BETWEEN Operator__
-`SELECT * FROM table_name
WHERE column BETWEEN low AND high; `

__Query Data using IN Operator__
-`SELECT * FROM table_name
WHERE column IN (value1, value2,...); `

__Constrain the Returned Rows with the LIMIT Clause:__
-`SELECT * FROM table_name
LIMIT limit OFFSET offset
ORDER BY column_name; `

__Query Data from Multiple using the Inner Join, Left Join, Full Outer Join, Cross Join and Natural Join__
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

__Return the Number of Rows of a Table__
-`SELECT COUNT (*)
FROM table_name; `

__Sort Rows in Ascending or Descending Order__
-`SELECT select_list
FROM table
ORDER BY column ASC [DESC], column2 ASC [DESC],...; `

__Group rows using GROUP BY clause__
-`SELECT *
FROM table
GROUP BY column_1, column_2, ...; `

__Filter Groups using the HAVING Clause__
-`SELECT *
FROM table
GROUP BY column_1
HAVING condition; `


>## Set Operators
__Combine the Result set of Two or More Queries with UNION Operator__
-`SELECT * FROM table1
UNION
SELECT * FROM table2; `

__Minus a result set using EXCEPT operator__
-`SELECT * FROM table1
EXCEPT
SELECT * FROM table2; `

__Get intersection of the result sets of two queries__
-`SELECT * FROM table1
INTERSECT
SELECT * FROM table2; `


>## Modifying Data
__Insert a new row into a table__
-`INSERT INTO table(column1,column2,...)
VALUES(value_1,value_2,...); `

__Insert multiple rows into a table__
-`INSERT INTO table_name(column1,column2,...)
VALUES(value_1,value_2,...),
(value_1,value_2,...),
(value_1,value_2,...)...`

__Update data for all rows__
-`UPDATE table_name
SET column_1 = value_1,
...; `

__Update data for a set of rows specified by a condition in the WHERE clause__
-`UPDATE table
SET column_1 = value_1,
...
WHERE condition; `

__Delete all rows of a table__
-`DELETE FROM table_name; `

__Delete specific rows based on a condition__
-`DELETE FROM table_name
WHERE condition; `


>## Performance
__Show the query plan for a query__
-`EXPLAIN query; `

__Show and execute the query plan for a query__
-`EXPLAIN ANALYZE query; `

__Collect statistics__
-`ANALYZE table_name; `

__ __
-` `


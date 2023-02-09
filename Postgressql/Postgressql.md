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

__ __
-` `

__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
__ __
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `
-` `









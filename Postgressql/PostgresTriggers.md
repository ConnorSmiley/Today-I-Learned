# Create Schema with object
<pre>
CREATE FUNCTION trigger_function()
RETURNS TRIGGER
LANGUAGE PLPGSQL
AS $$
BEGIN
-- trigger logic
END;
$$
</pre>


# Basic Structure
<pre>
 - CREATE [ OR REPLACE ] [ CONSTRAINT ] TRIGGER name { BEFORE | AFTER | INSTEAD OF } { event [ OR ... ] }
 ON table_name
 [ FROM referenced_table_name ]
 [ NOT DEFERRABLE | [ DEFERRABLE ] [ INITIALLY IMMEDIATE | INITIALLY DEFERRED ] ]
 [ REFERENCING { { OLD | NEW } TABLE [ AS ] transition_relation_name } [ ... ] ]
 [ FOR [ EACH ] { ROW | STATEMENT } ]
 [ WHEN ( condition ) ]
 EXECUTE { FUNCTION | PROCEDURE } function_name ( arguments )
</pre>


# simple trigger

<pre>
CREATE TRIGGER trigger_name 
   {BEFORE | AFTER |INSTEAD OF} { event_name }
   ON table_name
   [FOR [EACH] { ROW | STATEMENT }]
       EXECUTE PROCEDURE trigger_function
</pre>>

# post gres trigger

<pre>
CREATE OR REPLACE FUNCTION log_last_name_changes()
  RETURNS TRIGGER 
  LANGUAGE PLPGSQL
  AS
$$
BEGIN
	IF NEW.last_name <> OLD.last_name THEN
		 INSERT INTO employee_audits(employee_id,last_name,changed_on)
		 VALUES(OLD.id,OLD.last_name,now());
	END IF;

	RETURN NEW;
END;
$$
</pre>>

# create postgres trigger ???

<pre>
CREATE TRIGGER last_name_changes
  BEFORE UPDATE
  ON employees
  FOR EACH ROW
  EXECUTE PROCEDURE log_last_name_changes();

</pre>>


# drop trigger

<pre>
DROP TRIGGER [ IF EXISTS ] name ON table_name [ CASCADE | RESTRICT ]

</pre>>

# drop trigger sample

<pre>
DROP TRIGGER username_check
ON staff;
</pre>>

# rename a trigger

<pre>
ALTER TRIGGER name ON table_name RENAME TO new_name
</pre>>

# marking a postgres trigger on extension

<pre>
ALTER TRIGGER name ON table_name [ NO ] DEPENDS ON EXTENSION extension_name

</pre>>

# rename a trigger extension

<pre>
ALTER TRIGGER emp_stamp ON emp RENAME TO emp_track_chgs;

</pre>>

# marking a trigger dependent on an extension

<pre>
ALTER TRIGGER emp_stamp ON emp DEPENDS ON EXTENSION emplib;
</pre>>

# disable postgres trigger

<pre>
ALTER TABLE table_name
DISABLE TRIGGER trigger_name | ALL
</pre>>

# disable single postgres trigger

<pre>
ALTER TABLE employees
DISABLE TRIGGER log_last_name_changes;
</pre>>

# Disabling all postgres triggers

<pre>
ALTER TABLE employees
DISABLE TRIGGER ALL;
</pre>>

# enabling postgres triggers

<pre>
ALTER TABLE table_name
ENABLE TRIGGER trigger_name |  ALL;
</pre>>

# Enabling a single postgres trigger

<pre>
ALTER TABLE employees
ENABLE TRIGGER salary_before_update;
</pre>>

# enabling all postgres triggers

<pre>
ALTER TABLE employees
ENABLE TRIGGER ALL;
</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

#

<pre>

</pre>>

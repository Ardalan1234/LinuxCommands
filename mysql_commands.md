# MYSQL

display a list of all databases:
- `SHOW DATABASES;`

create a new database:
- `CREATE DATABASE database_name`

select a specific database:
- `USE database_name;`

display a list of tables within the currently selected database:
- `SHOW TABLES;`

create a new table within the currently selected database:
- `CREATE TABLE table_name (column1 datatype, column2 datatype, ...);`

rename one or more tables within a database:
- `RENAME TABLE current_table_name TO new_table_name;`

delete a table from a database:
- `DROP TABLE table_name;`

modify an existing table's structure:
- `ALTER TABLE table_name ADD COLUMN column_name data_type;`

rename a column in an existing table:
- `ALTER TABLE table_name RENAME COLUMN current_column_name TO new_column_name;`

modify the structure of an existing column in a table:
- `ALTER TABLE table_name MODIFY COLUMN column_name new_data_type;`

insert a new row of data into a table:
- `INSERT INTO table_name (column1, column2, ...) VALUES (value1, value2, ...);`

retrieve data from a table based on specified criteria:
- `SELECT column1, column2, ... FROM table_name WHERE condition;`

modify existing records in a table:
- `UPDATE table_name SET column1 = value1, column2 = value2, ... WHERE condition;`

remove one or more rows from a table:
- `DELETE FROM table_name WHERE condition;`

enforce uniqueness on the values of one or more columns in a table:
- `ALTER TABLE table_name ADD CONSTRAINT constraint_name UNIQUE (column1, column2, ...);`

specify that a column cannot accept null values:
- `ALTER TABLE table_name ALTER COLUMN column_name SET NOT NULL;`

specify a default value for a column when no explicit value is provided during an INSERT operation:
- `ALTER TABLE table_name ALTER COLUMN column_name SET DEFAULT default_value;`

uniquely identify each row in a table. It ensures that the values in the specified column or columns are unique and not null:
- `ALTER TABLE table_name ADD CONSTRAINT constraint_name PRIMARY KEY (column1, column2, ...);`

enforce specfic conditions on the values entered into a column:
- `ALTER TABLE table_name ADD CONSTRAINT constraint_name CHECK (condition);`

A FOREIGN KEY is a constraint in  relational database that establishes a link between two tables based on a specified column or set of columns:

- `ALTER TABLE table_name ADD CONSTRAINT foreign_key_name FOREIGN KEY (column_name) REFERENCES refrenced_table_name(referenced_column_name);`

drop foreign key:
- `ALTER TABLE table_name DROP FOREIGN KEY foreign_key_name;`

combine rows from two or more tables based on a related column between them:
- `SELECT column1, column2, ... FROM table1 INNER JOIN table2 ON table1.column = table2.column;`
- `SELECT column1, column2, ...  FROM table1 INNER JOIN table2 ON table1.column = table2.column;`
- `SELECT column1, column2, ... FROM table1 INNER JOIN table2 ON table1.column = table2.column;`

sort the rows returned by a SELECT statement based on one or more columns:
- `SELECT column1, column2, ... FROM table ORDER BY column1, column2, ... [ASC | DESC];`

restrict the number of rows returned by a query:
- `SELECT column1, column2, ... FROM table LIMIT [number_of_rows] [OFFSET offset_value];`

combine the result sets of two or more SELECT statements into a single result set or if you want to include all rows, including duplicates, use the UNION ALL operator instead of UNION:
- `SELECT column1, column2, ... FROM table1 UNION SELECT column1, column2, ... FROM table2;`

combine rows from the same table based on a related condition or relationship within the table:
- `SELECT a.column, a.column, ..., b.column, b.column. ... FROM table AS a INNER JOIN table AS b ON a.column = b.column;`

a view is a virtual table that is derived from the result of a query:
- `CREATE VIEW view_name AS SELECT column1, column2, ... FROM table WHERE condition;`

an index is a data structure that improves the speed of data retrieval operations on database tables:
- `CREATE INDEX index_name ON table_name (column1, column2, ...);`

group rows in a result set based on one or more columns:
- `SELECT column1, aggregate_function(column2) FROM table GROUP BY column1 HAVING condition;`

the ROLLUP modifier is used in conjunction with the GROUP BY clause to generate subtotals and grand totals in result sets:
- `SELECT column1, column2, ..., aggregate_function(column) FROM table GROUP BY column1, column2, ..., ROLLUP (column);`

on delete:
- `ALTER TABLE Child ADD CONSTRAINT constraint_name FOREIGN KEY (parent_id) REFERENCES Parent (id) ON DELETE CASCADE;`

- `ALTER TABLE Child ADD CONSTRAINT constraint_name FOREIGN KEY (parent_id) REFERENCES Parent (id) ON DELETE SET NULL;`



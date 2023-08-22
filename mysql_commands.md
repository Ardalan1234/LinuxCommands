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



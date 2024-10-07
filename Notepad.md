# MySQL Basic Syntax

## To create a new database(folders):
CREATE DATABASE database_name;

## To use a specific database:
USE database_name;

## To create a new table(files.db) within a database:
CREATE TABLE selectable_characters (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  age INT
);

## To insert data into a table(files.db):
INSERT INTO table_name (name, age)
VALUES ('John', 30);
## To insert multiple rows or data into a table:
VALUES  ('value', 'value', 2, 4),
        ('value', 'value', 6, 12),
        ('value', 'value', 3, 9);
## To retrieve data from a table:
selects all:
SELECT * FROM table_name;  

selects specific:
SELECT name, age FROM table_name;

## To update values in existing records:
UPDATE table_name
SET age = 31
WHERE id = 1;

## To add a new column to a table:
ALTER TABLE table_name
ADD email VARCHAR(50);

## To remove a column from a table:
ALTER TABLE table_name
DROP COLUMN email;

## To delete an entire table:
DROP TABLE table_name;

## To delete a database:
DROP DATABASE database_name;
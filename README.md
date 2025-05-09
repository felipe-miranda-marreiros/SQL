# SQL

> What is SQL?
- SQL is a standard language for storing, manipulating and retrieving data in databases.
> What SQL stands for?
- Structured Query Language
> What's the difference among DDL, DML, DCL and TCL?
- DDL (Data Definition Language): Defines or changes the structure of the database (tables, columns, etc.).

| Command    | Purpose                                      |
| ---------- | -------------------------------------------- |
| `CREATE`   | Creates tables, databases, indexes, etc.     |
| `ALTER`    | Modifies an existing structure               |
| `DROP`     | Deletes tables, databases, etc.              |
| `TRUNCATE` | Removes all records from a table             |
| `RENAME`   | Renames database objects like tables/columns |

- DML (Data Manipulation Language): Deals with the data itself (CRUD operations).

| Command  | Purpose                          |
| -------- | -------------------------------- |
| `INSERT` | Adds new records                 |
| `UPDATE` | Modifies existing records        |
| `DELETE` | Removes records                  |
| `SELECT` | Retrieves data from the database |

- DCL (Data Control Language): Manages permissions and access control.

| Command  | Purpose                       |
| -------- | ----------------------------- |
| `GRANT`  | Gives privileges to users     |
| `REVOKE` | Removes privileges from users |

- TCL (Transaction Control Language): Manages transactions to ensure data integrity.

| Command     | Purpose                                   |
| ----------- | ----------------------------------------- |
| `BEGIN`     | Starts a transaction                      |
| `COMMIT`    | Saves the changes made in the transaction |
| `ROLLBACK`  | Reverts changes if something goes wrong   |
| `SAVEPOINT` | Creates a point to partially roll back to |


- Structured Query Language
> What is the SQL order of execution?

| Order  | Clause | Function
| ------------- | ------------- | ------------- |
| 1  | FROM  | Choose and join tables to get base data.
| 2  | WHERE  | Filters the base data.
| 3  | GROUP BY  | Aggregates the base data.
| 4  | HAVING  | Filters the aggregated data.
| 5  | SELECT  | returns the final data.
| 6  | ORDER BY  | Sorts the final data.
| 7  | LIMIT  | Limits the returned data to a row count.

## DATABASE OPERATIONS

> How do you create a database?
```sql
CREATE DATABASE store;
```
> How do you select a database?
```sql
USE store;
```
> How do you delete a database?
```sql
DROP DATABASE store;
```
> How do you rename a database?
```sql
ALTER DATABASE store MODIFY NAME = stores
```
[It requires more steps to rename a database in MySQL](https://blog.devart.com/how-to-rename-a-mysql-database.html)

## TABLE OPERATIONS
> How do you create a table?
```sql
CREATE TABLE clients (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100) NOT NULL,
  email VARCHAR(100) NOT NULL,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
);
```
> How do you drop a table?
```sql
DROP TABLE clients;
```
> How do you truncate a table?
```sql
TRUNCATE TABLE clients;
```
> Whats the difference between DROP, DELETE and TRUNCATE?
- The DROP command in SQL removes the table from the database, the DELETE command removes one or more records from the table, and the TRUNCATE command removes all the rows from the existing table.
> How do you view details from database or table?
```sql
DESC store;
-- table
DESC clients;
```
## CRUD OPERATIONS

> How to create (INSERT) values?
```sql
INSERT INTO clients (name, email)
VALUES ('Alice', 'alice@example.com');
```
> How to read (SELECT) values?
```sql
SELECT name, emai FROM clients;
-- OR
SELECT * FROM clients;
```
> How to update (UPDATE) values?
```sql
UPDATE clients
SET email = 'alice@gmail.com'
WHERE id = 1;
```
> How to delete (DELETE) values?
```sql
-- Removes records from a table.
DELETE FROM clients
WHERE id = 1;
```

> ### What is SQL?

- SQL is a standard language for storing, manipulating and retrieving data in databases.
  > #### What SQL stands for?
- Structured Query Language
  > #### What's the difference among DDL, DML, DCL and TCL?
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
  > #### What is the SQL order of execution?

| Order | Clause   | Function                                 |
| ----- | -------- | ---------------------------------------- |
| 1     | FROM     | Choose and join tables to get base data. |
| 2     | WHERE    | Filters the base data.                   |
| 3     | GROUP BY | Aggregates the base data.                |
| 4     | HAVING   | Filters the aggregated data.             |
| 5     | SELECT   | returns the final data.                  |
| 6     | ORDER BY | Sorts the final data.                    |
| 7     | LIMIT    | Limits the returned data to a row count. |

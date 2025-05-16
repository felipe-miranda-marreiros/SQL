### TABLE OPERATIONS

> #### How do you create a table?

```sql
CREATE TABLE clients (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100) NOT NULL,
  email VARCHAR(100) NOT NULL,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
);
```

> #### How do you drop a table?

```sql
DROP TABLE clients;
```

> #### How do you truncate a table?

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

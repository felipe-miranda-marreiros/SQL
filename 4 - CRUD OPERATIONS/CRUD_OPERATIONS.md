### CRUD OPERATIONS

> #### How to create (INSERT) values?

```sql
INSERT INTO clients (name, email)
VALUES ('Alice', 'alice@example.com');
```

> #### How to read (SELECT) values?

```sql
SELECT name, emai FROM clients;
-- OR
SELECT * FROM clients;
```

> #### How to update (UPDATE) values?

```sql
UPDATE clients
SET email = 'alice@gmail.com'
WHERE id = 1;
```

> #### How to delete (DELETE) values?

```sql
-- Removes records from a table.
DELETE FROM clients
WHERE id = 1;
```

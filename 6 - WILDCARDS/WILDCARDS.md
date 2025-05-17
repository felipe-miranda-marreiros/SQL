# WILDCARDS

A wildcard character is used to substitute one or more characters in a string.

> ## `%`

The % symbol in SQL is called a wildcard, specifically:

- `%` represents zero or more characters.
- It is used with the `LIKE` operator for pattern matching.

```sql
WHERE name LIKE 'mouse%'   -- matches any string that starts with "mouse"
WHERE name LIKE '%mouse'   -- matches any string that ends with "mouse"
WHERE name LIKE '%mouse%'  -- matches any string that contains "mouse"
```

> ## `_` (underscore)

Matches exactly one character.

```sql
WHERE name LIKE '_ouse'   -- matches "Mouse", "House", etc.
```

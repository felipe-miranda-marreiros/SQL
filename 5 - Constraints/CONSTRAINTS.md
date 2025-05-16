### CONSTRAINTS

SQL constraints are used to specify rules for the data in a table.

| Constraints    | Rules                                                                             |
| -------------- | --------------------------------------------------------------------------------- |
| `NOT_NULL`     | Ensures that a column cannot have a NULL value                                    |
| `UNIQUE`       | Ensures that all values in a column are different                                 |
| `PRIMARY KEY`  | A combination of a `NOT NULL` and `UNIQUE`. Uniquely identifies each row in table |
| `FOREIGN KEY`  | Prevents actions that would destroy links between tables                          |
| `CHECK`        | Ensures that the values in a column satisfies a specific condition                |
| `DEFAULT`      | Sets a default value for a column if no value is specified                        |
| `CREATE INDEX` | Used to create and retrieve data from the database very quickly                   |

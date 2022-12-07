# This time the subject to by studied is SQL and its adapatation to postgresQL

## Symbols to have in mind to query data

- asterisc "\*": means select all
- non-asterisc: instead of using "\*" you can select a specific field by writting its name

## Queries for database

Create database:

```sql
  CREATE DATABASE db_name;
```

Drop database "deletes permanently the db selected":

```sql
  DROP DATABASE db_name;
```

## Queries for table

Create a table:

```sql
  CREATE TABLE table_name (
    prop datatype,
  );
```

Select data from a table:

```sql
  SELECT * FROM table_name;
```

Select data that is not duplicate:

```sql
  SELECT DISTINCT * FROM table_name;
```

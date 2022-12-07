# This time the subject to by studied is SQL and its adapatation to postgresQL

## Symbols to have in mind to query data

- asterisc "\*": means select all
- non-asterisc: instead of using "\*" you can select a specific field by writting its name

Keywords:

- AS: used to rename a field
- AND, OR, NOT: logic operators that can be paired with themself to generate a complex condition
- ORDER BY: query the data in a specific order mainly by choosing a table field
- ASC, DESC: query the data in ascendent or descendent order, based in dates, alphabeticaly, etc
- IS NULL, IS NOT NULL: evaluates if a value is or not null

Funtions:

- MIN(): selects the minimun value of a column
- MAX(): selects the maximun value of a column

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

Select data by accomplished a condition:

```sql
  SELECT * FROM table_name WHERE field_name='';
```

Insert data into specific columns:

```sql
  INSERT INTO table_name (col_name_1, col_name_2) VALUES (value_1, value_2);
```

Update columns in a table, always include a conditional:

```sql
  UPDATE table_name SET col_1=value, col_2=value WHERE field_name='';
```

Delete a value from a column of a table, always include a conditional:

```sql
  DELETE FROM table_name WHERE field_name='';
```

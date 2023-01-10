# This time the subject to be studied is SQL and its adapatation to postgresQL

## Symbols to have in mind to query data

- asterisc "\*": means select all
- non-asterisc: instead of using "\*" you can select a specific field by writting its name

Keywords:

- AS: alias is used to give a column a temporary name
- AND, OR, NOT: logic operators that can be paired with themself to generate a complex condition
- ORDER BY: query the data in a specific order mainly by choosing a table field
- ASC, DESC: query the data in ascendent or descendent order, based in dates, alphabeticaly, etc
- IS NULL, IS NOT NULL: evaluates if a value is or not null
- LIKE: helps to find out data that follows a pattern (E.G a name that starts with letter "x")
- IN: is a shorthand of multiple OR, and it allows you the specifie multiple values in a WHERE clause
- BETWEEN: select a values within a range (values can be numbers, text or dates)

Funtions:

- MIN(column_name): selects the minimun value of a column
- MAX(column_name): selects the maximun value of a column
- COUNT(column_name): counts the amount of rows that meets the requested criteria
- AVG(column_name): returns the average value of a numeric column
- SUM(column_name): returns the total sum of a numeric column

Wildcards:

Depending on the position of a wildcard the data retrieved can vary

- %: this is used in keywods like LIKE
- \_: this is used in keywods like LIKE

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
  SELECT * FROM table_name WHERE column_name='';
```

Insert data into specific columns:

```sql
  INSERT INTO table_name (col_name_1, col_name_2) VALUES (value_1, value_2);
```

Update columns in a table, always include a conditional:

```sql
  UPDATE table_name SET col_1=value, col_2=value WHERE column_name='';
```

Delete a value from a column of a table, always include a conditional:

```sql
  DELETE FROM table_name WHERE column_name='';
```

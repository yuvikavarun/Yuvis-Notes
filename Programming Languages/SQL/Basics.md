## Selecting Data
- ```SELECT```- retrives data we want (followed by the table(s) we want)
-  ```FROM``` - which table we want
- ```;``` - used to end a SQL statement, altho not necessary
- ```,``` - separates column names
- ```*``` - selects all columns of a table
- ```DISTINCT``` - gets only the unique values, leaves behind the duplicates

example code:
```
SELECT *
FROM patients
ORDER BY name;
```

## Ordering Data
- ```ORDER BY``` - orders the data in increasing order

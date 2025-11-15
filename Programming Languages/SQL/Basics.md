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
- ```ORDER BY``` - orders the data in increasing alphabetical/numerical order
- ```ASC``` - added at the end of order by query to order it in ascending order
- ```DESC``` - orders in descending order

## Filtering Data
- ```WHWERE``` - selects only the  items that fulfill a condition, like having the value Biology on the major column.
example:
```
SELECT *
FROM students
WHERE major = 'Biology'
```
- ```=``` - an operator that checks if two things are equal

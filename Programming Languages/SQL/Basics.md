## Selecting Data
- ```SELECT```- retrives data we want (followed by the table(s) we want)
-  ```FROM``` - which table we want
- ```;``` - used to end a SQL statement, altho not necessary
- ```,``` - separates column names
- ```*``` - selects all columns of a table
- ```DISTINCT``` - gets only the unique values, leaves behind the duplicates

## Ordering Data
- ```ORDER BY``` - orders the data in increasing alphabetical/numerical order
- ```ASC``` - added at the end of order by query to order it in ascending order
- ```DESC``` - orders in descending order
example:
```
SELECT *
FROM patients
ORDER BY name;
```

## Filtering Data
- ```WHWERE``` - selects only the  items that fulfill a condition, like having the value Biology on the major column.
example:
```
SELECT *
FROM students
WHERE major = 'Biology'
```

## Operators
- ```=``` - equality operator (to get items that satisfy a condition)
- ```<>``` - inequality operator (to get all items that do not satisfy a condition)
- ```<``` - less than
- ```>``` - greater than
- ```<=``` - less than/ equal to
- ```>=``` - greater than/ equal to
- 
example:
```
SELECT *
FROM students
WHERE marks >= 80;
```

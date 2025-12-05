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
- ```WHERE``` - selects only the  items that fulfill a condition, like having the value Biology on the major column.
- ```AS``` - alias
- ```LIKE``` - pattern matching
example:
```
SELECT *
FROM students
WHERE major = 'Biology'
```

example2:
```
SELECT*
FROM students
WHERE course_id LIKE '___-%
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

## Set Operations
- ```UNION``` - combines results from two queries. Removes duplicates automatically
  - ```UNION ALL``` - keeps duplicates
- ```INTERSECT``` - returns only the rows in both query results
- ```EXCEPT``` - returns only rows from the first query that are not in the second

## Aggregation Functions:
- ```GROUP BY``` - groups
  - ```AVG``` - average
  - ```COUNT``` - counts rows
  - ```SUM``` - adds up value
  - ```MIN``` - finds the smallest value in a group
  - ```MAX``` - finds the highest value in a group
note: we cannot use ```WITH``` while using ```<``` or ```>``` we gotta use ```HAVING```
example:
```
SELECT class_id, AVG(marks) 
FROM students 
GROUP BY class_id 
HAVING AVG(marks) > 75;SELECT*
FROM students
WHILE student_marks > AVG marks;
```

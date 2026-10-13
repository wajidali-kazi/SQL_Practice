# SQL_Practice
Just facing SQL Leet code question and improve my skills and analytics thinking 

# Leed code Question Number 1683.
Write a solution to find the IDs of the invalid tweets. The tweet is invalid if the number of characters used in the content of the tweet is strictly greater than 15.
Return the result table in any order.
# Code
```mysql []
# Write your MySQL query statement below
SELECT tweet_id
from tweets
where LENGTH(content) > 15 ;
```

# Leed code Question Number 1378. Replace Employee ID With The Unique Identifier
Write a solution to show the unique ID of each user, If a user does not have a unique ID replace just show null.
Return the result table in any order.
# Code
```mysql []
# Write your MySQL query statement below
select eu.unique_id, e.name
FROM Employees e
LEFT JOIN EmployeeUNI eu
ON e.id = eu.id;
```

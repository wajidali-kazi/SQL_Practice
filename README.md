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

# Leed code Question Number 1068. Product Sales Analysis I
Write a solution to report the product_name, year, and price for each sale_id in the Sales table.
Return the resulting table in any order.
# Code
```mysql []
# Write your MySQL query statement below
SELECT product_name, year, price 
FROM Sales s
INNER JOIN Product p
ON s.product_id = p.product_id
```

# Leed code Question Number 1581. Customer Who Visited but Did Not Make Any Transactions
Write a solution to find the IDs of the users who visited without making any transactions and the number of times they made these types of visits.
Return the result table sorted in any order.
# Code
```mysql []
# Write your MySQL query statement below
SELECT v.customer_id, COUNT(*) as count_no_trans 
FROM visits v
LEFT JOIN Transactions t
on v.visit_id = t.visit_id
WHERE t.visit_id IS NULL
GROUP BY customer_id ;
```

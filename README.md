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

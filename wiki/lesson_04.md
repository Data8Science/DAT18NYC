## W3 School

We'll be playing with the live database available here:

http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all

## Questions

Let's walk through a few examples:

1) Retrieve all Customers from Madrid

    SELECT * FROM Customers WHERE City='Madrid'

2) What is the most common city for customers?

    SELECT City, COUNT(*) FROM Customers GROUP BY City

3) What category has the most products?

    SELECT CategoryName, COUNT(*) FROM Categories
    JOIN Products on (Categories.CategoryID = Products.CategoryID)
    GROUP BY CategoryName

## Classwork

1. What customers are from the UK
2. What is the name of the customer who has the most orders?
3. What supplier has the highest average product price?
4. What category has the most orders?
5. What employee made the most sales (by number of sales)?
6. What employee made the most sales (by value of sales)?
7. What Employees have BS degrees? (Hint: Look at LIKE operator)
8. What supplier has the highest average product price *assuming they have at least 2 products* (Hint: Look at the HAVING operator)

Submit these SQL queries as a .sql file to schoology, using SQL comments to have the question referring to each:

    -- What customers are from the UK?
    SELECT * FROM Customers WHERE Country = 'UK'

    -- What is the name of the customer who has the most orders?

## APIs

Two APIs worth getting data from:

https://apigee.com/console/instagram

https://apigee.com/console/twitter
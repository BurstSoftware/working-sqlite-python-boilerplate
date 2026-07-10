Create a list of sql quires 

Here is a useful list of common SQL queries you can use as a reference.
If you want queries for a specific database (e.g., MySQL, PostgreSQL) or for a specific project, just let me know!

Basic SQL Queries
Select all records from a table
SELECT * FROM table_name;
Select specific columns
SELECT column1, column2 FROM table_name;
Filter records (WHERE clause)
SELECT * FROM employees
WHERE department = 'Sales';
Sort records (ORDER BY)
SELECT * FROM products
ORDER BY price DESC;
Limit number of records
SELECT * FROM orders
LIMIT 10;
CRUD (Create, Read, Update, Delete)
Insert
INSERT INTO customers (name, email, city)
VALUES ('John Doe', 'john@example.com', 'Boston');
Update
UPDATE customers
SET city = 'New York'
WHERE customer_id = 5;
Delete
DELETE FROM customers
WHERE customer_id = 5;
Joins
Inner Join
SELECT orders.order_id, customers.name
FROM orders
INNER JOIN customers
ON orders.customer_id = customers.customer_id;
Left Join
SELECT c.name, o.order_id
FROM customers c
LEFT JOIN orders o
ON c.customer_id = o.customer_id;
Right Join
SELECT c.name, o.order_id
FROM customers c
RIGHT JOIN orders o
ON c.customer_id = o.customer_id;
Group By & Aggregate Functions
Count
SELECT department, COUNT(*)
FROM employees
GROUP BY department;
Sum
SELECT customer_id, SUM(amount)
FROM payments
GROUP BY customer_id;
Average
SELECT AVG(salary) AS avg_salary
FROM employees;
Subqueries
SELECT name
FROM products
WHERE price > (SELECT AVG(price) FROM products);
Create & Modify Tables
Create table
CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    salary DECIMAL(10,2)
);
Add a column
ALTER TABLE employees
ADD COLUMN hire_date DATE;
Drop a table
DROP TABLE employees;

If you'd like, I can generate:

✔ A set of advanced SQL queries
✔ Queries for a specific dataset
✔ Queries for interview preparation
✔ Queries for MySQL / PostgreSQL / SQL Server / Oracle

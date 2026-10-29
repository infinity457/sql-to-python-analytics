# sql-to-python-analytics
A collection of analytical SQL problems translated into Python/Pandas.

#Purpose of the repository
These are a collection of SQL problems from beginner to advanced for the concepts mentioned. The same problems have been translated into Python.

#SQL concepts covered
GROUP BY
HAVING
JOINS
CTEs
Subqueries
Window functions

#Problem statemnets

#GROUP BY#
Mental model: What does one row of the output represent?

1. Beginner — Department-wise employee count
You are given an employees table. Write a query to find the total number of employees in each department.
Approach: So, What does one row of the output represent here? one row represents each department. Therefore, you count the records of employees for each department.

2. Beginner–Intermediate — Average salary by department
You are given an employees table. Find the average salary for each department and display only departments whose average salary is greater than ₹60,000.
Approach: What does one row of the output represent here? one row represents one department along with average salary for each, with a condition: departments whose average salary is greater than ₹60,000. Therefore, you display the departments which are having the average salary above ₹60,000.

3. Intermediate — Monthly sales aggregation
You are given a sales table. Calculate total sales for each region for each month.
Your output should contain month, region, and total_sales.
Approach: What does one row of the output represent here? one unique combination of month and region with total sales .The output asks for month, region and total sales, so how do you extract each month, by using a function called as String Format Time.

4.Intermediate–Advanced — Customers with multiple orders
You are given an orders table.Find customers who have placed at least two orders and whose total spending exceeds ₹1,000. Return the customer ID, number of orders, and total spending.
Approach: What does one row represent? One row represents one customer/order. So, you select customer_id, count of each orders and total spending, by filtering those totals whose spending exceeds ₹1000.

5. Advanced — Product performance analysis. You are given an order_items table.
For each category, calculate:
- Total quantity sold
- Total revenue (quantity × unit_price)
- Number of distinct orders
Return only categories with total revenue greater than ₹100,000, sorted by revenue from highest to lowest.
Approach: What does one row represent? One row represents one category. Along with this, you have to calculate the sum of quantity sold, revenue for each category, then count of distinct orders.
Filtered with total revenue greater than ₹100,000. Also mind the condition, sort revenue by descending order.

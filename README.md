# SQL-queires


-- Online SQL Editor to Run SQL Online.
-- Use the editor to create new tables, insert data and all other SQL operations.

--SELECT item,AVG(amount)
--FROM Orders
--WHERE amount > 300
--GROUP BY item
--HAVING AVG(amount) >= 300

--SELECT customer_id,
--SUM(CASE WHEN item = 'Keyboard' THEN amount ELSE 0 END) AS Keyboard,
--SUM(CASE WHEN item = 'Mouse' THEN amount ELSE 0 END) AS Mouse,
--SUM(CASE WHEN item = 'Monitor'THEN amount ELSE 0 END) AS Monitor,
--SUM(CASE WHEN item = 'Mousepad' THEN amount ELSE 0 END) AS Mousepad,
--SUM(CASE WHEN item = 'Keyboard' THEN amount ELSE 0 END)
--+ SUM(CASE WHEN item = 'Mouse' THEN amount ELSE 0 END)
--+ SUM(CASE WHEN item = 'Monitor'THEN amount ELSE 0 END)
--+ SUM(CASE WHEN item = 'Mousepad' THEN amount ELSE 0 END) AS Total
--FROM Orders
--GROUP BY customer_id

-- finding duplicates
--SELECT customer_id, COUNT(1) AS frequency
--FROM Orders
--GROUP BY customer_id
--HAVING frequency > 1;


--SELECT * FROM Shippings WHERE customer not in (SELECT customer_id from Orders)

--SELECT s.*, o.customer_id 
--FROM Shippings s 
--LEFT JOIN Orders o ON
--s.customer = o.customer_id
--WHERE o.customer_id IS null

--COUNT(*), COUNT(1), COUNT('a') all gives same values
--except COUNT(col_name) give non-null count
--COUNT(DISTINCT col_name) gives distinct values

--Running sum
--SELECT *, SUM(amount) OVER(ORDER BY order_id) AS running_sum
--FROM Orders;

-- Find Median in SQL
--SELECT AVG(amount) AS Median FROM
--(SELECT *,
--ROW_NUMBER() OVER(ORDER BY amount ASC) AS r_desc,
--ROW_NUMBER() OVER(ORDER BY amount DESC) AS r_asc
--FROM Orders) a
--WHERE ABS(a.r_desc - a.r_asc) <=1;








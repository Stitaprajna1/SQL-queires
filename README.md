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








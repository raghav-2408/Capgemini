# Basic SQL Questions

## 1. **What is SQL?**
SQL (Structured Query Language) is a standardized language used to manage and manipulate databases. It allows you to interact with a database to query, update, insert, and delete data.

## 2. **What are the different types of SQL commands?**
SQL commands are divided into the following categories:

- **DML (Data Manipulation Language)**: Used to manipulate data in the database.
  - `SELECT`: Retrieve data from a database.
  - `INSERT`: Insert new data into a database.
  - `UPDATE`: Modify existing data in the database.
  - `DELETE`: Remove data from a database.

- **DDL (Data Definition Language)**: Used to define and modify database structures.
  - `CREATE`: Create a new table or database.
  - `ALTER`: Modify the structure of a database or table.
  - `DROP`: Delete a table or database.

- **DCL (Data Control Language)**: Used to control access to data.
  - `GRANT`: Give a user permission to perform tasks on the database.
  - `REVOKE`: Remove a user’s permissions.

- **TCL (Transaction Control Language)**: Used to manage database transactions.
  - `COMMIT`: Save changes made during a transaction.
  - `ROLLBACK`: Undo changes made during a transaction.
  - `SAVEPOINT`: Set a point to which you can roll back in a transaction.

---

## 3. **What is the difference between `WHERE` and `HAVING`?**
- **`WHERE`**: Filters records before grouping the data. It is used in `SELECT`, `UPDATE`, and `DELETE` statements.
- **`HAVING`**: Filters records after the grouping is done. It is used with aggregate functions (`COUNT()`, `SUM()`, etc.) in `GROUP BY` clauses.

---

## 4. **What are aggregate functions in SQL?**
Aggregate functions are used to perform calculations on multiple rows of data and return a single value. Common aggregate functions include:
- **`COUNT()`**: Counts the number of rows in a query.
- **`SUM()`**: Calculates the sum of a numeric column.
- **`AVG()`**: Finds the average of a numeric column.
- **`MIN()`**: Finds the minimum value in a column.
- **`MAX()`**: Finds the maximum value in a column.

---

## 5. **What is the difference between `INNER JOIN`, `LEFT JOIN`, and `RIGHT JOIN`?**

- **`INNER JOIN`**: Returns only the rows where there is a match in both tables.
- **`LEFT JOIN`**: Returns all rows from the left table and the matched rows from the right table. If no match is found, `NULL` values are returned for the right table's columns.
- **`RIGHT JOIN`**: Returns all rows from the right table and the matched rows from the left table. If no match is found, `NULL` values are returned for the left table's columns.

---

## 6. **What is a primary key?**
A **primary key** is a column (or a set of columns) that uniquely identifies each row in a table. It cannot contain `NULL` values and must be unique for every record.

---

## 7. **What is a foreign key?**
A **foreign key** is a column (or set of columns) in one table that links to the primary key of another table. It is used to establish a relationship between the two tables.

---

## 8. **What is normalization?**
Normalization is the process of organizing data in a database to avoid redundancy and dependency. It involves dividing large tables into smaller ones and using relationships to ensure data integrity.

---

## 9. **What is the `DISTINCT` keyword in SQL?**
The **`DISTINCT`** keyword is used to return only unique (non-duplicate) values from a column.

---

## 10. **What are indexes in SQL?**
An **index** is a database object that improves the speed of data retrieval operations on a table. It is created on one or more columns of a table to quickly locate data without scanning the entire table.

## 11. **What is the `GROUP BY` clause in SQL?**
The **`GROUP BY`** clause is used to group rows that have the same values in specified columns. It is often used with aggregate functions to summarize data.

## 12. **What is a subquery in SQL?**
A **subquery** is a query embedded within another query. It is used to retrieve intermediate results that are used in the main query.

## 13. **What is the `LIMIT` clause in SQL?**
The **`LIMIT`** clause is used to specify the number of rows returned by the query. It is typically used with `SELECT` statements.

## 14. **What is a view in SQL?**
A **view** is a virtual table based on the result of a `SELECT` query. It does not store data itself but shows data from one or more tables. Views are used to simplify complex queries.

## 15. **What is a transaction in SQL?**
A **transaction** is a sequence of SQL operations that are executed as a single unit. Transactions ensure that either all operations are completed successfully or none of them are, maintaining the integrity of the database.

## 16. **What is the difference between `TRUNCATE` and `DELETE`?**

- **`DELETE`**: Deletes rows one by one and can be rolled back if wrapped in a transaction.
- **`TRUNCATE`**: Deletes all rows from a table and cannot be rolled back. It is faster than `DELETE` because it does not log individual row deletions.

## 17. **What are `NULL` values in SQL?**
A **NULL** value represents missing or unknown data. It is different from an empty string or zero. You can check for `NULL` using `IS NULL` or `IS NOT NULL`.



## 10. Indexes in SQL
CREATE INDEX idx_column_name ON table_name (column_name);

## 11. `GROUP BY` Clause in SQL
SELECT column_name, COUNT(*) 
FROM table_name
GROUP BY column_name;

## 12. Subquery in SQL
SELECT column_name 
FROM table_name 
WHERE column_name IN (SELECT column_name FROM another_table);

## 13. `LIMIT` Clause in SQL
SELECT * FROM table_name LIMIT 5;

## 14. View in SQL
CREATE VIEW view_name AS
SELECT column_name1, column_name2 
FROM table_name 
WHERE condition;

## 15. Transaction in SQL
BEGIN TRANSACTION;
UPDATE table_name SET column_name = value WHERE condition;
COMMIT;

## 16. `TRUNCATE` vs `DELETE` in SQL
DELETE FROM table_name WHERE condition;

TRUNCATE TABLE table_name;

## 17. `NULL` Values in SQL
SELECT * FROM table_name WHERE column_name IS NULL;

SELECT * FROM table_name WHERE column_name IS NOT NULL;

## Applications of MySQL/SQL

1. **Web Development**: MySQL is widely used in backend development for storing and retrieving data in web applications. It's commonly paired with PHP, JavaScript, or Python in full-stack development.
   - Example: Websites like WordPress, Facebook, and Twitter use MySQL for managing user data, posts, and interactions.

2. **E-commerce Platforms**: SQL databases help manage large inventories, customer orders, payments, and shipping details in online stores.
   - Example: Platforms like Amazon, eBay, and Shopify use SQL databases for efficient transaction management.

3. **Banking Systems**: MySQL is used to manage customer accounts, transactions, and financial records securely in banking systems.
   - Example: SQL databases handle data like account balances, transaction history, and customer details.

4. **Customer Relationship Management (CRM)**: SQL databases store customer details, sales, and interactions which can be analyzed to improve customer relationships and services.
   - Example: CRM software like Salesforce uses SQL databases to manage customer data.

5. **Healthcare Management**: SQL is used to store and retrieve patient data, medical records, prescriptions, and appointments.
   - Example: Hospitals and clinics use SQL databases to manage patient information, billing, and treatment history.

---

## Advantages of MySQL/SQL

1. **Data Integrity**: SQL databases provide strong data integrity using constraints (e.g., primary keys, foreign keys, unique constraints) to ensure accuracy and consistency.
   
2. **Scalability**: MySQL can handle large datasets and is suitable for both small and large-scale applications. It can scale vertically and horizontally to meet growing demands.

3. **Security**: MySQL provides user authentication, encryption, and access control to ensure secure data management. 

4. **Ease of Use**: SQL syntax is straightforward and widely understood, making it accessible for developers, database administrators, and analysts.

5. **Relational Structure**: SQL databases store data in a structured format using tables, making it easier to relate different types of data, reducing redundancy.

6. **Transaction Support**: MySQL supports transactions, ensuring data consistency and reliability by enabling commit, rollback, and savepoint operations.

7. **Wide Adoption**: MySQL is open-source and has a large community of developers contributing to its improvement, making it a reliable choice for many applications.

---

## Disadvantages of MySQL/SQL

1. **Complexity with Large Datasets**: As the size of the database grows, managing performance with complex queries, indexing, and optimization becomes challenging.

2. **Limited Flexibility with Schema**: SQL databases rely on a fixed schema, making it difficult to change the structure once the database is designed without causing disruptions.

3. **Not Ideal for Unstructured Data**: SQL databases are not well-suited for storing unstructured data, such as images, videos, and social media content.

4. **Performance Issues in Highly Concurrent Systems**: While MySQL supports concurrency, performance can degrade when handling a very high number of simultaneous queries.

5. **Scaling for High-Volume Traffic**: Although MySQL is scalable, it can require significant effort to maintain performance and data consistency when scaling out horizontally (across multiple servers).

6. **Limited NoSQL Features**: Unlike NoSQL databases, MySQL lacks some features like schema-less designs, which can be an issue for highly dynamic or unstructured data.


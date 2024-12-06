### Database Management System (DBMS)

#### 1. What is DBMS?
A Database Management System (DBMS) is software that allows users to create, manage, and manipulate databases. It acts as an interface between the database and the user, ensuring data is organized, secure, and easily accessible.

#### 2. What are the key features of a DBMS?
- **Data Abstraction**: Simplifies the structure of data for users.
- **Data Security**: Provides mechanisms to protect data from unauthorized access.
- **Data Consistency**: Maintains consistent data during transactions.
- **Concurrency Control**: Allows multiple users to access data simultaneously.
- **Backup and Recovery**: Ensures data is recoverable in case of failure.

#### 3. What are the different types of DBMS?
- **Hierarchical DBMS**: Data is organized in a tree-like structure.
- **Network DBMS**: Data is organized in a graph, allowing many-to-many relationships.
- **Relational DBMS (RDBMS)**: Data is organized in tables with rows and columns (e.g., MySQL, PostgreSQL).
- **Object-Oriented DBMS**: Data is stored in the form of objects.

#### 4. What is a relational database?
A relational database organizes data into tables with rows (records) and columns (attributes). Relationships between data are established using keys.

#### 5. What is SQL?
Structured Query Language (SQL) is a standard language used to communicate with relational databases for tasks like querying, updating, and managing data.

#### 6. What are keys in a database?
- **Primary Key**: A unique identifier for each record in a table.
- **Foreign Key**: A field in one table that references the primary key in another table.
- **Candidate Key**: A field or set of fields that can uniquely identify a record.
- **Composite Key**: A primary key consisting of two or more fields.

#### 7. What is normalization in DBMS?
Normalization is the process of organizing data to reduce redundancy and improve data integrity. It involves dividing large tables into smaller ones and defining relationships between them.

#### 8. What are the types of normalization?
- **1NF (First Normal Form)**: Removes duplicate columns and ensures atomicity.
- **2NF (Second Normal Form)**: Ensures all non-key attributes are fully functional dependent on the primary key.
- **3NF (Third Normal Form)**: Removes transitive dependency.
- **BCNF (Boyce-Codd Normal Form)**: A stricter version of 3NF.

#### 9. What are ACID properties in DBMS?
- **Atomicity**: Ensures transactions are all-or-nothing.
- **Consistency**: Ensures data remains consistent before and after a transaction.
- **Isolation**: Ensures concurrent transactions do not interfere with each other.
- **Durability**: Ensures completed transactions persist even in case of system failure.

#### 10. What is a transaction in DBMS?
A transaction is a sequence of operations performed as a single logical unit of work. It ensures data consistency and integrity.

#### 11. What is the difference between DBMS and RDBMS?
- **DBMS**: Does not necessarily use tables or support relationships (e.g., file systems).
- **RDBMS**: Uses tables with rows and columns, supports relationships, and follows ACID properties.

#### 12. What is indexing in DBMS?
Indexing is a technique to optimize database performance by creating a data structure that allows fast retrieval of records based on certain attributes.

#### 13. What is the difference between clustered and non-clustered indexes?
- **Clustered Index**: Physically sorts data in the table based on key values.
- **Non-Clustered Index**: Maintains a separate structure to point to the data in the table.

#### 14. What are the advantages of DBMS?
- **Data Integrity**: Ensures data accuracy and consistency.
- **Data Security**: Protects data from unauthorized access.
- **Data Sharing**: Allows multiple users to access data concurrently.
- **Backup and Recovery**: Protects data against accidental loss.

#### 15. What are the disadvantages of DBMS?
- **Cost**: High initial setup and maintenance cost.
- **Complexity**: Requires trained personnel to manage.
- **Performance**: May be slower for simple tasks compared to traditional file systems.

#### 16. What is a NoSQL database?
A NoSQL database is a non-relational database designed for unstructured or semi-structured data. It supports horizontal scaling and is commonly used for large-scale, distributed systems.

#### 17. What are the types of NoSQL databases?
- **Document Stores**: Store data as documents (e.g., MongoDB).
- **Key-Value Stores**: Store data as key-value pairs (e.g., Redis).
- **Column Stores**: Store data in columns (e.g., Cassandra).
- **Graph Databases**: Store data as nodes and edges (e.g., Neo4j).

#### 18. What is the difference between SQL and NoSQL?
- **SQL**: Structured, uses tables, schema-based, and best for structured data.
- **NoSQL**: Flexible schema, best for unstructured or semi-structured data, and supports horizontal scaling.

#### 19. What is a view in DBMS?
A view is a virtual table based on the result of an SQL query. It provides a way to simplify complex queries and restrict access to certain data.

#### 20. What is a stored procedure in DBMS?
A stored procedure is a precompiled SQL query that can be executed repeatedly. It helps in reducing redundancy and improving performance.

#### 21. What is a trigger in DBMS?
A trigger is a database object that is automatically executed in response to certain events, such as `INSERT`, `UPDATE`, or `DELETE` operations.

#### 22. What are joins in DBMS?
Joins are used to combine rows from two or more tables based on a related column. Common types include:
- **Inner Join**: Returns records with matching values in both tables.
- **Left Join**: Returns all records from the left table and matching ones from the right.
- **Right Join**: Returns all records from the right table and matching ones from the left.
- **Full Join**: Returns all records when there is a match in either table.

#### 23. What is a data warehouse?
A data warehouse is a centralized repository for storing large volumes of data from multiple sources. It is optimized for querying and analysis.

#### 24. What is data mining in DBMS?
Data mining is the process of discovering patterns and extracting useful information from large datasets using techniques like clustering, classification, and association.

#### 25. What are the different types of database models?
- **Hierarchical Model**: Data is organized in a tree-like structure.
- **Network Model**: Data is organized as a graph with nodes and relationships.
- **Relational Model**: Data is organized in tables with rows and columns.
- **Object-Oriented Model**: Data is stored as objects with attributes and methods.

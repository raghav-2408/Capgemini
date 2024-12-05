## MongoDB Interview Questions for Capgemini

### 1. What is MongoDB?
MongoDB is a NoSQL, document-oriented database that stores data in JSON-like format called BSON (Binary JSON). It is known for its flexibility, scalability, and ease of use, especially in handling large volumes of unstructured or semi-structured data.

### 2. What are the advantages of MongoDB over traditional relational databases?
- **Scalability**: MongoDB supports horizontal scaling through sharding, allowing it to handle large amounts of data across many servers.
- **Flexibility**: MongoDB allows you to store data without defining a strict schema, unlike relational databases that require predefined schemas.
- **High Availability**: MongoDB supports replica sets, providing automatic failover and redundancy for higher availability.
- **Performance**: MongoDB is optimized for read-heavy and write-heavy workloads.

### 3. What are the different types of data models in MongoDB?
- **Document Model**: Stores data as documents (JSON or BSON format). Each document is a set of key-value pairs.
- **Key-Value Model**: MongoDB's document model can also be seen as a key-value pair model, where the key is the unique identifier (e.g., _id).
- **Graph Model**: MongoDB can represent relationships between data through embedded documents or by using MongoDB's graph processing features.

### 4. What is BSON in MongoDB?
BSON (Binary JSON) is a binary representation of JSON-like documents. It extends JSON’s flexibility and supports more data types, such as `Date`, `Binary`, and `ObjectId`. BSON allows MongoDB to efficiently store and process data.

### 5. What is the difference between MongoDB and MySQL?
- **Data Storage**: MongoDB stores data in collections (JSON-like documents), while MySQL uses tables (rows and columns).
- **Schema**: MongoDB is schema-less, allowing flexible data models, while MySQL uses a rigid schema for tables.
- **Scalability**: MongoDB provides horizontal scaling using sharding, while MySQL typically scales vertically.
- **Joins**: MongoDB doesn't support joins in the traditional way but can use `$lookup` for some operations. MySQL supports complex joins between tables.

### 6. What are the main features of MongoDB?
- **Schema-less structure**: Flexible schema allows storing data without predefined structures.
- **High Availability**: Using replica sets to ensure data redundancy and automatic failover.
- **Sharding**: Horizontal scaling by distributing data across multiple servers.
- **Aggregation Framework**: For complex data processing and transformation.
- **Indexing**: MongoDB supports various types of indexes to optimize query performance.
- **Rich Query Language**: MongoDB supports powerful queries, including range queries, sorting, and text search.

### 7. What are collections and documents in MongoDB?
- **Collection**: A collection is a grouping of MongoDB documents, similar to a table in relational databases. Collections don't enforce a schema.
- **Document**: A document is a set of key-value pairs, similar to a row in a relational database but with more flexibility. Documents are stored in BSON format.

### 8. How do you create a database and a collection in MongoDB?
```javascript
use myDatabase; // Creates or switches to a database
db.createCollection("myCollection"); // Creates a collection
```

### 9. What is the difference between `db.createCollection()` and `db.collection()` in MongoDB?
- **`db.createCollection()`**: Explicitly creates a new collection with a defined schema (if required).
- **`db.collection()`**: Refers to a collection that can be used without explicitly creating it first. If the collection doesn’t exist, MongoDB will create it automatically when you insert a document.

### 10. What are indexes in MongoDB?
Indexes in MongoDB improve query performance by providing a more efficient way of finding documents. MongoDB supports various types of indexes like single field, compound, geospatial, text, and hashed indexes.

### 11. How do you create an index in MongoDB?
You can create indexes on fields in a collection to speed up query processing by using the `createIndex()` method.

### 12. What is sharding in MongoDB?
Sharding is the process of distributing data across multiple servers. It helps in horizontal scaling, ensuring that a large dataset can be handled efficiently by splitting the data into smaller chunks (shards).

### 13. What is a replica set in MongoDB?
A replica set is a group of MongoDB instances that maintain the same data set, providing redundancy and high availability. If the primary server fails, one of the secondary servers is automatically promoted to primary.

### 14. What are the different types of joins in MongoDB?
MongoDB doesn’t support traditional joins but provides `$lookup` to perform joins between collections. You can join data from one collection into another using `$lookup`.

### 15. What is an `ObjectId` in MongoDB?
An **ObjectId** is a unique identifier automatically generated by MongoDB for every document. It is a 12-byte identifier that includes timestamp information, ensuring uniqueness.

### 16. How do you perform an aggregation operation in MongoDB?
MongoDB’s aggregation framework allows for advanced data processing, such as filtering, grouping, sorting, and transforming data.

### 17. How does MongoDB handle data consistency?
MongoDB uses eventual consistency in some configurations (e.g., replica sets), meaning data updates might not be immediately visible across all nodes. However, it offers options like `writeConcern` and `readConcern` to control consistency and durability.

### 18. What are the data types supported by MongoDB?
MongoDB supports various data types including:
- **String**: Textual data
- **Integer**: Whole numbers
- **Double**: Decimal numbers
- **Boolean**: True or false values
- **Array**: List of values
- **Date**: Date and time
- **ObjectId**: Unique identifier
- **Null**: Null value
- **Binary Data**: Used to store binary files
- **Object**: Embedded documents

### 19. What is the purpose of `find()` in MongoDB?
The **`find()`** method is used to query and retrieve documents from a MongoDB collection.

### 20. What is the `insertOne()` method in MongoDB?
The **`insertOne()`** method is used to insert a single document into a MongoDB collection.

### 21. What is the `update()` method in MongoDB?
The **`update()`** method is used to modify existing documents in a collection. It can update multiple fields and can either replace or modify parts of the document.

### 22. What is the `deleteOne()` method in MongoDB?
The **`deleteOne()`** method removes a single document from a collection that matches the given filter.

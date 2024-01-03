# SQL vs NoSQL

RDBMS

* Inner Joins: 

1. Full - all records when there is a match in left (table1) or right (table2) table records
2. Inner - records that have matching values in both tables
3. Left - all records from the left table, and the matched records from the right table
4. Right - all records from the right table, and the matched records from the left table


NoSQL - built to scale with high performance but queries are less flexible; structure relies on key/value store; structure can be tables, documents, graphs or json; scales very well


Out of the box, DynamoDB does not support ACID operations. However, developers can use Transactions in DynamoDB to achieve atomicity, consistency, isolation and durability in its GET, PUT, UPDATE or DELETE operations. Therefore DDB is acid compliant.

One of the main differences between SQL and NoSQL is indexing. SQL uses a B-tree index which employs a hierarchical structure to store data. In contrast, NoSQL uses a hash index, which stores data in a key-value store. With a B-tree index, data is stored in an ordered manner, making it easy to retrieve specific values based on their position in the tree. However, this can also make updates and inserts more time-consuming, as the entire tree must be traversed to find the correct location for the new data.
A hash index, however, allows data to be stored in any order. This feature can make inserts and updates faster, as only the relevant key needs to be found. However, it can also make retrieval more difficult, as the data is not sorted in any particular way. As a result, each type of index has its advantages and disadvantages.

Database Indexing Strategies: How NoSQL outperforms traditional indexing


Traditional relational databases use vertical scaling, meaning that when more users are added or data sets grow larger, the database server is upgraded to a more powerful machine (CPU and RAM).
NoSQL databases, on the other hand, use horizontal scaling. When more users are added, or data sets grow larger, additional database servers are added to the system.
In addition, NoSQL databases are generally more scalable than SQL databases since they are designed to run on distributed systems. As a result, they can take advantage of the processing power of multiple machines.
When it comes to performance, SQL databases typically have the edge. This is because they are designed to work with structured data and use declarative query language. This allows developers to write concise and efficient queries.
On the other hand, NoSQL databases are designed to work with large unstructured data sets. As a result, their query languages tend to be less efficient. However, this difference in performance is often offset by the fact that NoSQL databases can scale more easily.



* [NoSQL Design for DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/bp-general-nosql-design.html)

* [DynamoDB Cost Optimization Tips](https://dynobase.dev/dynamodb-cost-optimization/)

* [Normalization](https://www.guru99.com/database-normalization.html)


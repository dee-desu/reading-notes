# Mongo and Mongoose


---

**Fill in the chart below with five differences between SQL and NoSQL databases:**

|SQL|NoSQL|
|---|---|
|primarily called as Relational Databases (RDBMS)|primarily called as non-relational or distributed database|
|table based databases|document based, key-value pairs|
|have predefined schema| have dynamic schema for unstructured data|
|vertically scalable whereas|horizontally scalable|
|uses SQL ( structured query language ) for defining and manipulating the data|ueries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language)|
|examples: MySql, Oracle, Sqlite, Postgres and MS-SQL|MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb|
|For complex queries|not good fit for complex queries|
|not best fit for hierarchical data storage|fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data|
|best fit for heavy duty transactional type applications, as it is more stable and promises the atomicity as well as integrity of the data|you can use NoSQL for transactions purpose, it is still not comparable and sable enough in high load and for complex transactional applications.|
|Excellent support are available for all SQL database from their vendors|have to rely on community support, and only limited outside experts are available for you to setup and deploy your large scale|
|emphasizes on ACID properties ( Atomicity, Consistency, Isolation and Durability)|follows the Brewers CAP theorem ( Consistency, Availability and Partition tolerance )|
|can classify SQL databases as either open-source or close-sourced from commercial vendors|can be classified on the basis of way of storing data as graph databases, key-value store databases, document store databases, column store database and XML databases.|

**What kind of data is a good fit for an SQL database?**

SQL databases are best fit for heavy duty transactional type applications.

**Give a real world example.**

Employees, salary, and HR data in a company.

**What kind of data is a good fit a NoSQL database?**

 fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. 

**Give a real world example.**

Netflix relies on NoSQL database

**Which type of database is best for hierarchical data storage?**

SQL is best for hierarchical storage.

**Which type of database is best for scalability?**

NoSQL does not require to upgrade the hardware.

**What does SQL stand for?**

Structured Query Language.

**What is a relational database?**

a database structured to recognize relations between stored items of information.

**What type of structure does a relational database work with?**

A relational database organizes data into rows and columns, which collectively form a table.

**What is a 'schema'?**

s considered the “blueprint” of a database which describes how the data may relate to other tables or other data models.

**What is a NoSQL database?**

A place that stores data in a form of key-value pair.

**How does it work?**

Store data in documents rather than relational tables.

**What is inside of a Mongo database?**

MongoDB stores data records as documents (specifically BSON documents) which are gathered together in collections.

**Which is more flexible - SQL or MongoDB? and why.**

MongoDB as it ensures high and diverse data availability

**What is the disadvantage of a NoSQL database?**

Don't have the reliability functions which Relational Databases have (basically don't support ACID).

---
---

## Things I want to know more about

- express
- Mongoose
- SQL
- NoSQL

 ---

## References

[1] LUKE P. ISSAC, Jan 14, 2014, _SQL vs NoSQL Database Differences Explained with few Example DB_, thegeekstuff.com, accessed 1 September 2022, <https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool>

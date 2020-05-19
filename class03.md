## data model

 usually we creat in a graphical form. we do a create a diagram which identifies the main concepts in the domain, their features and relationships. The concepts often take the form of named rectangles. In the case of a hospital, they could be named: patient, doctor, ward etc. The relationships between them are illustrated as lines or arrows connecting the rectangles. The rectangles can be annotated in various ways to show additional information. You could for example list all the necessary information for a patient: name, age, gender etc.
 and here is some of penefits

 1. Higher Quality
 2. Reduced cost
 3. Clearer scope
 4. Faster performance
 5. Better documentation
 6. Fewer application errors
 7. Fewer data errors
 8. Managed risk

## CRUD

 CRUD means Create, Read, Update, Delete, and it can mean different things in different systems, but for SQL Server, it is commonly considered to map to the following SQL operations on table records.

 and we use it to make our apllecation more scalable ,controllable,ha a security control and better for Facilitate the trouble-shooting process

## PostgreSQL and mongoDB

 PostgreSQL: PostgreSQL is an object-relational database management system (ORDBMS) with an emphasis on extensibility and standards compliance. PostgreSQL is ACID-compliant, transactional, has updatable and materialized views, triggers, and foreign keys. It also supports functions and stored procedures.

PostgreSQL uses tables, constraints, triggers, roles, stored procedures and views as the core components that you work with. A table consists of rows, and each row contains a same set of columns. PostgreSQL uses primary keys to uniquely identify each row (a.k.a record) in a table, and foreign keys to assure the referential integrity between two related tables.

PostgreSQL also supports many NoSQL features as well.

MongoDB: MongoDB uses JSON-like documents to store schema-free data. In MongoDB, collections of documents do not require a predefined structure and columns can vary for different documents.

MongoDB has many of the features of a relational database, including an expressive query language and strong consistency. However, since it is schema-free MongoDB allows you to create documents without having to create the structure for the document first.

A useful comparison with relational database management systems (RDBMS) in which you have: Table | Column | Value | Records. In comparison, in MongoDB you have: Collection | Key | Value | Document. This means that collections in MongoDB are like tables in RDBMS.

Documents are like records in a RDBMS. Documents can easily be modified by adding or deleting fields without having to restructure the entire document.

## Mongoose

Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node.js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.

## example

for delevery applecation :
coustomer name
location
price
id
owner
status
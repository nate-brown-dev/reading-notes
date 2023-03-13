# Code 301 Reading 11

## nosql vs sql

### Fill in the chart below with five differences between SQL and NoSQL databases

| SQL | NoSQL |
| --- | --- |
| Table based | Document based / key-value pairs / graphs / wide-columns stores|
| Predefined schema | Dynamic schema for unstructured data |
| Vertically scalable | Horizontally scalable |
| Uses SQL (structured query language) | Queries focus on collection of documents / UnQL
| Good fit for complex query environment | Not good fit for complex queries |
| Not best fit for hierarchical data | Better fit for hierarchical / big data |
| Manage load by increasing computing power on single server | Manage by adding servers |

### What kind of data is a good fit for an SQL database?

- Structured data, consistent contents

### Give a real world example for SQL

- Financial data like a transaction register, where each transaction has the same elements

### What kind of data is a good fit a NoSQL database?

- Unstructured, semi-structured, or big data

### Give a real world example for NoSQL

- A music collection consisting of multiple file formats

### Which type of database is best for hierarchical data storage?

- NoSQL

### Which type of database is best for scalability?

- NoSQL probably, if your server is at capacity, just add another server instead of trying to upgrade the one you have

## sql vs nosql (Video)

### What does SQL stand for?

Structured Query Language

### What is a relational database?

- works with tables
- database contents have relationship to one another

### What type of structure does a relational database work with?

- table structure
- strict schema

### What is a ‘schema’?

- 'schema' defines how the database is organized
- in a relational/table database, all records have the same fields
- true even if contents for a single item are null/empty/falsy
- a large relational database connects multiple "related" tables
- related databases can have multiple relation types
- one-to-one
- one-to-many
- many-to-many

### What is a NoSQL database?

- non-relational
- has collections instead of tables
- inside collections are "documents" like rows in table
- multiple documents in collection can have different fields
- instead of forcing null/empty values on items, just define them differently

### How does it work?

- no schema implied

### What is inside of a MongoDB database?

- collections of documents

### Which is more flexible - SQL or MongoDB? and why

- mongoDB is more flexible
- no schema implied
- no relations required

### What is the disadvantage of a NoSQL database?

- records might not have required field because of non table layout
- no relations, have to duplicate data in multiple places
- not as good for regularly updated data
  - data in multiple places and can't be updated relationally
  - possible worse performance when regularly updating

[Go back home](/reading-notes/)

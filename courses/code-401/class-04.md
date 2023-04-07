# Code 401 Reading 4

## nosql vs sql

### What type of database is the best fit for the complex query intensive environment?

SQL

### What type of database is the best fit for hierarchical data storage?

NoSQL

### Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend

SQL is scaled by adding power to a single computer, like getting a larger boat to carry more passengers
NoSQL is scaled by adding more computers, like using a flotilla of small boats to carry lots of passengers

## sql modeling techniques

### Among data tables, what is a one-to-many relationship and how do we “relate” them?

an entry in one table can be connected to more than one entry in another table

one entry in a table: a classroom
multiple related entries in another table: the students in that classroom

### Prior to designing your relational database, it might be useful to ___ a ___ of the database tables and their relationships

CREATE a DIAGRAM

### Explain the difference between a primary and foreign key

primary key: the key for the table
foreign key: key in the table that matches primary key in another table

## sql vs nosql video

### How do we treat keywords and parameters differently in SQL syntax?

here

### Define normalization within the context of schemas and data

in SQL database, all records have to match the defined schema
when records dont match the schema (eg data is missing) they have to be normalized
normalizing applies defaults to the empty fields, or nulls, or something else so that the fields have data

### Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter

- one to one relationship: a record in one table is associated with a single record in another table
  - one record is a student, the other record is the student's schedule
- one to many relationship: a record in one table is associated with many records in another table
  - one record is a student, the other records are all the student's schedules for every period they attended the school
- many to many relationship: many records in one table match many records in another table
  - one table is all students, another table is all classes. each student has multiple classes, and each class has multiple students
  
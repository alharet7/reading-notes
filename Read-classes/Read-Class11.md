# Introduction to Databases and ERDs

## Database Schema

- A database schema is a logical representation of data that shows how the data is organized and the relationships between the tables in a database. A database schema also defines the constraints and rules that apply to the data, such as data types, primary keys, foreign keys, etc. A database schema can be represented visually using diagrams or textually using code or syntax.

### What is a Schema?

- A schema is a skeleton or blueprint of a database that describes its structure and organization. A schema does not contain any actual data, but only the information about how the data is stored and related. A schema can be used to create, modify, or delete tables, fields, views, indexes, and other database objects.

### Why do we use them?

We use database schemas for several reasons:

- They help us design and plan the database before creating it.
- They provide a clear and consistent view of the data and its relationships.
- They enable us to enforce data integrity and consistency rules.
- They facilitate data access and manipulation by using queries and commands.
- They document the database structure and organization for future reference and maintenance.

### What do they look like?

Database schemas can look different depending on the type of database system and the level of abstraction. There are three main types of database schemas:

- Physical schema: This describes how the data is physically stored in the storage devices, such as files, blocks, sectors, etc. This is the lowest level of abstraction and it is usually defined by the database administrator (DBA). The physical schema can vary depending on the hardware and software configuration of the system.
- Logical schema: This describes how the data is logically organized in terms of tables, fields, data types, relationships, constraints, etc. This is the most common level of abstraction and it is usually defined by the database designer or developer. The logical schema can be independent of the physical schema and it can be implemented in different ways.
- View schema: This describes how the data is presented to the end-users or applications. This is the highest level of abstraction and it is usually defined by the database user or analyst. The view schema can be customized to suit different needs and preferences.

---

## Database Keys

- Database keys are attributes or sets of attributes that uniquely identify a row or record in a table and establish relationships between tables. There are different types of keys in database, such as primary, natural, surrogate, composite, alternate, unique, and foreign keys.

### What is a Primary Key?

- A primary key is one or more columns in a table that are used to uniquely identify the row. A primary key cannot have null values and must be unique for each row. A primary key is also used to reference other tables using foreign keys.

- For example, in a table of students, the student ID can be a primary key:

| Student ID | Name  | Email             |
|------------|-------|-------------------|
| 101        | Alice | <alice@example.com> |
| 102        | Bob   | <bob@example.com>   |
| 103        | Carol | <carol@example.com> |

### What is a Foreign Key?

- A foreign key is one or more columns in a table that refer to the primary key of another table. A foreign key can have null values and can have duplicate values. A foreign key is used to create a relationship between two tables and enforce referential integrity.

- For example, in a table of courses, the student ID can be a foreign key that references the student table:

| Course ID | Course Name | Student ID |
|-----------|-------------|------------|
| C101      | Math        | 101        |
| C102      | English     | 102        |
| C103      | Science     | 103        |
| C104      | History     | 101        |

### What is a Composite Key?

- A composite key is a combination of two or more columns that are used to uniquely identify a row in a table. A composite key can be a primary key or a foreign key. A composite key is used when no single column can uniquely identify the row.

- For example, in a table of enrollments, the combination of student ID and course ID can be a composite key:

| Student ID | Course ID | Grade |
|------------|-----------|-------|
| 101        | C101      | A     |
| 101        | C104      | B     |
| 102        | C102      | C     |
| 103        | C103      | D     |

### How are they different? When do you use one over the others?

The main difference between the types of keys is their purpose and function. Here are some general guidelines on when to use one over the others:

- Use a primary key to uniquely identify each row in a table and to reference other tables using foreign keys.
- Use a foreign key to create a relationship between two tables and to ensure that the values in the referencing table exist in the referenced table.
- Use a composite key when no single column can uniquely identify the row and when you need to use more than one column to create a relationship between two tables.

---

## Relationships in a Relational Database

A relational database is a type of database that stores and organizes data in tables, where each table consists of rows and columns. A table represents a collection of related entities, such as customers, products, orders, etc. A row represents a single instance of an entity, such as a specific customer or product. A column represents an attribute or property of an entity, such as a name, price, quantity, etc.

### What is a Relationship?

A relationship is a logical connection or association between two or more tables in a relational database. A relationship allows users to query the database and get results that combine data from different tables into a single table. For example, if you own a record store, the database might have a table for albums, another for song titles, and another for artists. A relationship would allow you to query the database and get a table that shows the album name, song title, and artist name for each song.

### How is a Relationship Established?

A relationship is established between two tables by using a common attribute or column that links them together. This attribute is called a key. A key is a column or a set of columns that uniquely identifies each row in a table. There are different types of keys in a relational database, such as primary keys, foreign keys, candidate keys, etc.

The most common types of keys used to create relationships are primary keys and foreign keys. A primary key is a column or a set of columns that uniquely identifies each row in a table. A primary key cannot have null values or duplicate values. A foreign key is a column or a set of columns that references the primary key of another table. A foreign key can have null values or duplicate values, but it must match an existing value in the referenced table.

### What are the Types of Relationships?

There are three main types of relationships in a relational database: one-to-one, one-to-many, and many-to-many. The type of relationship depends on how many rows in one table can be related to how many rows in another table.

### Why are Relationships Important?

Relationships are important in a relational database because they enable users to:

1- Reduce data redundancy: Relationships help avoid storing the same data in multiple tables, which saves storage space and improves data consistency.

2- Enhance data integrity: Relationships help enforce rules and constraints on the data, such as referential integrity, which ensures that the values in the foreign keys match the values in the primary keys.

3- Facilitate data access: Relationships help perform queries and operations on the data using SQL (Structured Query Language), which allows users to join, filter, sort, group, aggregate, and manipulate data from different tables.
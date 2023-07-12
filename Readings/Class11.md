# Introduction to Databases and ERDs

This topic is important because it provides  into how to design and organize a database effectively, allowing for efficient data storage and retrieval.

## Data Models (Review the DB Schema)

Do some research on what a Database Schema is.

- **What is a Schema?**
schema is the organization or structure of the database.
- **Why do we use them?**
we use it to define the entities and relationships among them, and that makes easier to manage and understand the strucre of data .
- **What do they look like?**
A database schema can be represented in a visual diagram, which shows the database objects and their relationship with each other.

![task6](../assets/schema.png)

---

Different types of Database Keys

- **What is a Primary Key?** is a unique identifier for each record in a table.
- **What is a Foreign Key?**  is a field or combination of fields in a table that refers to the primary key of another table.
- **What is a Composite Key?** is a primary key that consists of multiple columns
- **How are they different? When do you use 1 over the others?**
  - Primary Key: when you need unique identifier for each record in a table.
  - Foreign key:when you want to link table with another table.
  - Composite Key:  when a single column cannot uniquely identify a record.

## DBMS

What are Relationships in a relational database?

- **What is a 1:1 relationship?** each record in one table is linked with exactly one record in another table.

    Example :Each client of a company has a single client ID.

- **What is a Many:Many relationship?** multiple records in one table are linked with multiple records in another table

    Example:Many customers can buy multiple products.

- **How about a 1: Many or a Many:1?** each record in one table is linked with one or more records in another table, but each record in the second table is linked with only one record in the first table.

    Example:One person can have multiple contact numbers.

# Entity Framework and APIs

Entity Framework is a tool to work with databases in the context of APIs. It provides a way to interact with the database.And that is why this topic matters.

## Entity Framework Core

Entity Framework (EF) Core is a lightweight, extensible, open source, and cross-platform version of the popular Entity Framework data access technology.

### The model

EF supports the following model development approaches:

- Generate a model from an existing database.
- Hand-code a model to match the database.
- Once a model is created, use EF Migrations to create a database from the model. Migrations allow evolving the database as the model changes.

### Querying

as we learned before Instances of entity classes are retrieved using LINQ

### Saving data

example:

```charp
db.Blogs.Add(blog);
    db.SaveChanges();
```

### EF O/RM considerations

some of the best practices applicable to any O/RM that help to avoid common pitfalls in production apps:

- Functional and integration testing
-Performance and stress testing with representative loads
- Security review
- Application deployment and migration

## Data Seeding

from the title, it is the process of populating a database with an initial set of data.

ways to achieve this in EF Core:

- Model seed data
- Manual migration customization
- Custom initialization logic

## User Secrets

 It is a secure way of storing private user information such as API keys, client secrets, and connection strings.

## things I want to learn

- best practices of Entity Framework
- discover how to save data changes made to entity instances using the `SaveChanges`

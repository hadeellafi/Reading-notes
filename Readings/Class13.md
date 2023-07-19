# Dependency Injection & Repository Design Pattern

## Overview of dependency injection

it is a powerful technique for managing dependencies and promoting clean and maintainable code by leveraging the principles of loose coupling and separation of concerns.

Dependency injection addresses these problems through:

- The use of an interface or base class to abstract the dependency implementation.
- Registration of the dependency in a service container.
- Injection of the service into the constructor of the class where it's used.

## The Repository pattern

The Repository pattern is a Domain-Driven Design pattern separating persistence concerns from the system's domain model, using persistence abstractions and adapters.

### Define one repository per aggregate

- For each aggregate or aggregate root, you should create one repository class.
- In a microservice based on Domain-Driven Design (DDD) patterns, the only channel you should use to update the database should be the repositories.
- the transactional area (that is, the updates) must always be controlled by the repositories and the aggregate roots.
- When you receive a command in a command handler, you use repositories to get the data you want to update from the database.
- To achieve the goal of the aggregate root to maintain transactional consistency between all the objects within the aggregate, you should never create a repository for each table in the database.

## SOLID Principles

### Why SOLID Matters

The SOLID Principals guide developers in creating well-designed, high-quality, and easy-to-maintain software. These principles promote good practices in software design and development, aiding in Test Driven Development (TDD).

- **Single Responsibility Principle** Is the idea that every method or class in your application should have exactly one reason to change.

- **The Open/Close Principle**
is very closely related to the topics of Encapsulation and Inheritance.OCP states that software, be it a method or a class, should be open for extension, but closed to modification.

- **The Liskov Substitution Principle** states that an object in your application should be able to be replaced with a type derived from it without breaking the application.

- **The Interface Segregation Principle** states that clients should not be forced to rely on interfaces they do not use.you should make fine grained interfaces that are specific to the functions and needs of the client.

- **The Dependency Inversion Principle** is the idea that code should depend on abstractions; not concrete implementations.

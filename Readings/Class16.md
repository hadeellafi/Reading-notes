# Data Transfer Objects

A DTO is an object that defines how the data will be sent over the network.And biggest advantage of using DTOs is decoupling clients from your internal data structures.

## Why use Data Transfer Objects (DTOs)?

our web API exposes the database entities to the client. The client receives data that maps directly to your database tables to accomplish this we use data transfer object (DTO)

### Use DTOs for abstraction

DTOs can be used to split the presentation layer or user interface from the domain objects in the application.
Similar to that, you may change your application's domain layer without modifying its presentation layer.

### Use DTOs for data hiding

by using DTOs you can return only the data requested. For example, the entity employee holds many properties and there is no need the share all of them with each request to avoid this problem, you might design a DTO class named EmployeeDTO that would contain only the properties that are requested.

### DTO serialization challenges

Use lazy loading or asynchronous loading to load entities only when required in order to solve serialization challenges.

## Description

This web application is a REST API microservice responsible for CRUD (Create, Read, Update, Delete) operations on the `Job` entity, including data that is directly related such as a job's `Category` and `Suburb`.
Given the scope of the problem, only Read and Update operations are implemented.

### Getting Started
- From the root of the project, run `docker-compose up`
- Run the commands in init.sql file to initialize the database
- You should now have the Swagger UI running on http://localhost:5000/swagger/index.html

### NOTES
- The application uses CQRS design pattern
- Request handlers are implemented using the [MediatR](https://github.com/jbogard/MediatR) library
- [MediatR](https://github.com/jbogard/MediatR) pipeline behaviours are used perform actions before executing a request handler
- validation logic is implemented using [FluentValidation]
- Entities are mapped to DTOs using [AutoMapper]
- CRUD operations are performed using [EF Core] and [LINQ]


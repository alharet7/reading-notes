# Dependency Injection & Repository Design Pattern

## Dependency injection in ASP.NET Core

Dependency injection is a **technique** for achieving inversion of control between classes and their dependencies. It allows us to decouple our code from specific implementations and make it more testable and maintainable.

ASP.NET Core supports dependency injection by using a built-in service container, which is an implementation of the **IServiceProvider** interface. we can register our services (such as interfaces, classes, or options) with the service container in the **ConfigureServices** method of the Program.cs file. Then, you can request our services via constructor injection or action injection in our controllers or other classes that need them.

---

## The Repository pattern

The Repository pattern is a Domain-Driven Design pattern intended to keep persistence concerns outside of the system's domain model. One or more persistence abstractions - interfaces - are defined in the domain model, and these abstractions have implementations in the form of persistence-specific adapters defined elsewhere in the application.

Repository implementations are classes that encapsulate the logic required to access data sources. They centralize common data access functionality, providing better maintainability and decoupling the infrastructure or technology used to access databases from the domain model.

> A repository performs the tasks of an intermediary between the domain model layers and data mapping, acting in a similar way to a set of domain objects in memory. Client objects declaratively build queries and send them to the repositories for answers. Conceptually, a repository encapsulates a set of objects stored in the database and operations that can be performed on them, providing a way that is closer to the persistence layer. Repositories, also, support the purpose of separating, clearly and in one direction, the dependency between the work domain and the data allocation or mapping.


---

## The repository design pattern

The repository design pattern is a way of abstracting the data access layer from the business logic layer. It provides a collection-like interface for accessing domain objects, while hiding the details of how they are persisted or retrieved. The repository pattern can help with:

1. Decoupling the application from the persistence framework
2. Improving testability by using mock or fake repositories
3. Supporting multiple data sources or data formats
4. Applying common logic or operations to the data access layer.

We can implement the repository pattern in C# using generics, interfaces, and dependency injection. He also shows how to use the repository pattern with Entity Framework Core and Dapper, two popular ORM frameworks for .NET. He concludes by highlighting some benefits and drawbacks of the repository pattern, such as:

1. Benefits: cleaner code, easier maintenance, better performance, more flexibility
2. Drawbacks: extra layer of abstraction, possible duplication of code, potential mismatch with the database model

---

## SOLID principles

SOLID principles are a set of guidelines for writing high-quality, maintainable, and testable code. The SOLID principles are:

- Single Responsibility Principle: A class should have only one reason to change
- Open/Closed Principle: A class should be open for extension but closed for modification
- Liskov Substitution Principle: A subclass should be substitutable for its base class
- Interface Segregation Principle: A client should not depend on methods it does not use
- Dependency Inversion Principle: A class should depend on abstractions, not concretions
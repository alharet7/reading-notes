# Data Transfer Objects

DTOs are objects that define how the data will be sent over the network, and they can be used to change the shape of the data that is exposed to the client. For example, we can use DTOs to remove circular references, hide properties, reduce payload size, flatten object graphs, avoid over-posting, or decouple our service layer from our database layer.

In other words,Data Transfer Objects (DTOs) are objects that carry data between processes in order to reduce the number of methods calls. They are useful when we want to change the shape of the data that we send to the client, for example, to hide some properties, flatten object graphs, or avoid over-posting vulnerabilities.

To create DTOs in EF, we need to define classes that represent the data we want to transfer, and then use LINQ Select statements to convert from our database entities into our DTOs. We can also use AutoMapper to simplify the mapping process.

## Why use Data Transfer Objects (DTOs)?

When designing and developing an application, if you’re using models to pass data between the layers and sending data back to the presentation layer, then you’re exposing the internal data structures of your application. That’s a major design flaw in your application.

By decoupling your layers DTOs make life easier when you’re implementing APIs, MVC applications, and also messaging patterns such as Message Broker. A DTO is a great choice when you would like to pass a lightweight object across the wire — especially when you’re passing your object via a medium that is bandwidth-constrained.

## Immutability of DTOs

A DTO is meant to transport data from one layer of an application to another layer. The consumer of a DTO might be built in .NET/C#/Java or even JavaScript/TypeScript. A DTO is often serialized so that it can be independent of the technology used in the receiver. In most cases, the receiver of the data does not need to modify that data after receipt — ideally it shouldn’t!

This is a classic example of the importance of immutability. And it’s exactly why a DTO should be immutable!

There are several ways in which you can implement immutable DTOs in C#. You could use a ReadOnlyCollection or the thread-safe immutable collection types present in the System.Collections.Immutable namespace. You can take advantage of record types in C# 9 to implement immutable DTOs as well.
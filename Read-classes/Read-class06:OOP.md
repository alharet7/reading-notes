# Object Oriented Principles

## Inheritance

- Inheritance is one of the three primary characteristics of **object-oriented programming**. It enables you to create new classes that reuse, extend, and modify the behavior defined in other classes. The class whose members are inherited is called the base class, and the class that inherits those members is called the derived class.

- A derived ***class*** can have only one direct base **class**. However, inheritance is transitive. If `ClassC` is derived from `ClassB`, and `ClassB` is derived from `ClassA`, `ClassC` inherits the members declared in `ClassB` and `ClassA`.

- Conceptually, a derived class is a specialization of the base class.[READ MORE](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/inheritance)

---

## Abstract

- The `abstract` keyword enables you to create classes and class members that are incomplete and must be implemented in a derived class. The `sealed` keyword enables you to prevent the inheritance of a class or certain class members that were previously marked virtual.

- **Classes** can be declared as abstract by putting the keyword `abstract` before the class definition. An abstract class cannot be instantiated. The purpose of an abstract class is to provide a common definition of a base class that multiple derived classes can share.

- Abstract classes may also define abstract methods. This is accomplished by adding the keyword `abstract` before the return type of the method. Abstract methods have no implementation, so the method definition is followed by a semicolon instead of a normal method block. Derived classes of the abstract class must implement all abstract methods.[READ MORE](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/abstract-and-sealed-classes-and-class-members)

---

## Polymorphism

- Polymorphism means “many forms” and it occurs when we have many classes that are related to each other by inheritance. Inheritance lets us inherit fields and methods from another class. Polymorphism uses those methods to perform different tasks. This allows us to perform a single action in different ways. [READ MORE](https://www.w3schools.com/cs/cs_polymorphism.php)

- Polymorphism is often referred to as the third pillar of object-oriented programming, after encapsulation and inheritance. It has two distinct aspects: At run time, objects of a derived class may be treated as objects of a base class in places such as method parameters and collections or arrays. When this polymorphism occurs, the object’s declared type is no longer identical to its run-time type.[READ MORE](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/object-oriented/polymorphism)

---

## OOP Principles

- **Object-oriented programming** (OOP) is a programming paradigm based on the concept of ***“objects”***, which can contain data and code: data in the form of fields (often known as attributes or properties), and code, in the form of methods (often known as functions or procedures).

There are **four** main principles of OOP: encapsulation, abstraction, inheritance, and polymorphism.

- **Encapsulation** is the practice of keeping fields within a class private, then providing access to them via public methods. It’s a protective barrier that keeps the data and code safe within the class itself. This way, we can re-use objects like code components or variables without allowing open access to the data system-wide.

- **Abstraction** means dealing with the level of complexity by hiding irrelevant details and only showing the necessary information. It helps reduce complexity and isolate the impact of changes.

- **Inheritance** allows us to create new classes that reuse, extend, and modify the behavior defined in other classes. The class whose members are inherited is called the base class, and the class that inherits those members is called the derived class.

- **Polymorphism** means “many forms” and it occurs when we have many classes that are related to each other by inheritance. Inheritance lets us inherit fields and methods from another class. Polymorphism uses those methods to perform different tasks. This allows us to perform a single action in different ways.[READ MORE](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/tutorials/oop)
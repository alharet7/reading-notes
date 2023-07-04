# Class 08 :Collections & Enums

## Collections

- Collections in C# are a way to group objects together. They are flexible and can change in size as needed. Arrays are another way to group objects, but they have a fixed size. Collections can be more flexible and can have keys assigned to objects for easy retrieval. Generic collections are type-safe and only allow one data type to be added.

- The System.Collections.Generic namespace provides generic implementation of standard data structure like linked lists, stacks, queues, and dictionaries. The System.Collections namespace provides general-purpose data structure that works on object references, so it can handle any type of object, but not in a safe-type manner.

## Enumeration

- An enumeration type (or enum type) is a value type defined by a set of named constants of the underlying integral numeric type. To define an enumeration type, use the enum keyword and specify the names of `enum` members:

      enum Season
       {
       Spring,
       Summer,
       Autumn,
       Winter
       }

- In another words An enum (short for “enumeration”) is a special “class” in C# that represents a group of constants (unchangeable/read-only variables). To create an enum, use the `enum` keyword (instead of `class` or `interface`), and specify the names of enum members, separated by a comma. You can access enum items with the dot syntax.

- By default, the associated constant values of enum members are of type `int`; they start with zero and increase by one following the definition text order. You can explicitly specify any other integral numeric type as an underlying type of an enumeration type. You can also explicitly specify the associated constant values.

- Enums are often used to represent a choice from a set of mutually exclusive values or a combination of choices. To represent a combination of choices, define an enumeration type as bit flags.

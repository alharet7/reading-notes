# Readings: LINQ & Delegates

- ***LINQ*** stands for Language-Integrated Query and is a set of technologies based on the integration of query capabilities directly into the C# language. It provides a consistent query experience for objects (LINQ to Objects), relational databases (LINQ to SQL), and XML (LINQ to XML).[READ MORE](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/)

- In a LINQ query, you are always working with objects. You use the same basic coding patterns to query and transform data in XML documents, SQL databases, ADO.NET Datasets, .NET collections, and any other format for which a LINQ provider is available.[READ MORE](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/introduction-to-linq-queries)

- A LINQ query is an expression that retrieves data from a data source. All LINQ query operations consist of three distinct actions: obtaining the data source, creating the query, and executing the query.[READ MORE](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/introduction-to-linq-queries)

For example, here is a simple LINQ query that retrieves all even numbers from an integer array:

    int[] numbers = new int[7] { 0, 1, 2, 3, 4, 5, 6 };
    var numQuery = from num in numbers
                   where (num % 2) == 0
                   select num;
    foreach (int num in numQuery)
    {
        Console.Write("{0,1} ", num);
    }

This example shows how the three parts of a query operation are expressed in source code.

### For practice
[Walkthrough: Writing Queries in C# (LINQ)](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/walkthrough-writing-queries-linq)
# Read-class 03

### 🤔 why this topic matters as it relates to what I'am studying in this module? 

This is important for me as a .NET developer because it gives me the ability to work with files and directories, find files and directories based on certain criteria, and use different types of streams like network, memory, and pipe streams.

---

### File and Stream I/O :

File and stream I/O (input/output) refers to the transfer of data either to or from a storage medium. In .NET, the System.IO namespaces contain types that enable reading and writing, both synchronously and asynchronously, on data streams and files. These namespaces also contain types that perform compression and decompression on files, and types that enable communication through pipes and serial ports.

---

### Write to a file:

We use this classes and methods to write text to a file:

- **StreamWriter** contains methods to write to a file synchronously (`Write` and `WriteLine`) or asynchronously (`WriteAsync` and `WriteLineAsync`).

- **File** provides static methods to write text to a file such as `WriteAllLines` and `WriteAllText`, or to append text to a file such as `AppendAllLines`, `AppendAllText`, and `AppendText`.

- **Path** is for strings that have file or directory path information. It contains the `Combine` method and in .NET Core 2.1 and later, the `Join` and `TryJoin` methods. These methods let you concatenate strings for building a file or directory path.

---

### Read to a file:

The System.IO.BinaryWriter and System.IO.BinaryReader classes are used for writing and reading data other than character strings.
[SEE THIS EXAMPLE](https://learn.microsoft.com/en-us/dotnet/standard/io/how-to-read-and-write-to-a-newly-created-data-file)
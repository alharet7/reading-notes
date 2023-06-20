# Read-class 04 : Classes & Memory Management

### 🤔 why this topic matters as it relates to what I'am studying in this module? 

Understanding static and instance constructors, as well as stack and heap memory, is important in .NET development.

Knowing these concepts helps me structure my code correctly, optimize memory usage, and improve performance. By using value types on the stack when possible and minimizing long-lived objects on the heap, I can make more efficient use of memory resources in my applications. This knowledge is essential for building high-quality software in .NET.

---

### What’s the difference between a static and an instance constructor?

- a ***static constructor*** is a special method that runs only once when a class is first used. It sets up static data or does something that only needs to happen once. An ***instance constructor*** is a method that runs when an object is created. It sets up the object’s data.

---

### How does the use of a static constructor differ from setting properties/values?

- a ***static constructor*** sets up static data or does something that only needs to happen once. It runs only once when a class is first used.and ***setting properties*** allows you to change an object’s values after it has been created. In general, use a constructor when certain values are needed for the object to work and use properties for values that can be changed later.

---

### Knowing what you now know about the stack and the heap, how might you rethink the way you did projects in previous courses, to make more effecient use of memory?

 - I should try to use value types and put them on the stack when I can because it’s faster than using the heap. and I should also pay attention to how long objects last and try to have fewer objects that last a long time on the heap. This can help make memory use more efficient and improve how well garbage collection works.
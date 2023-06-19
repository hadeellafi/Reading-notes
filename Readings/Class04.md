# Class04: Classes & Memory Management

The topic of classes and memory management is important because it directly affects the performance, stability, and efficiency of software applications.

- **What’s the difference between a static and an instance constructor?**

     A static constructor is used to initialize any static data or to perform a particular action that needs to be performed only once. It is called automatically before the first instance is created or any static members are referenced. A static constructor will be called at most once.

    Instance constructor is declared to specify the code that is executed when you create a new instance of a type with the new expression.

- **How does the use of a static constructor differ from setting properties/values?**

    Static constructors are automatically invoked before accessing any static members.On the other hand, setting values allows for dynamic behavior.

---

- **Knowing what you now know about the stack and the heap, how might you rethink the way you did projects in previous courses, to make more effecient use of memory?**

    I would recheck my previous projects to evaluate the efficiency of memory usage. For future projects, I would consider more the data types I choose, aiming to minimize memory allocation and optimize memory usage to achieve better overall efficiency.

---

- **Compare “Garbage Collection” in C# with the lifecycle of normal household items.**

    The garbage collector in C# and the lifecycle of normal household items have some similarities. They both involve managing resources. They aim to prevent keeping things unnecessarily. And both of them focus on using available space or memory efficiently.

---

## Things I want to know more about

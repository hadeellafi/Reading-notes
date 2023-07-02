# Interface

An interface in C# serves as a blueprint of a class, defining a set of related behaviors that classes must implement. It resembles an abstract class, with all methods declared inside the interface being abstract, lacking a method body. Interfaces cannot be instantiated and do not declare instance data like fields. Interface names conventionally begin with the letter "I".

## Default interface members

interfaces can have default members. An interface member may declare a body, and these member bodies in an interface are considered the default implementation.example:

```charp
public interface Idefault
{
    void Method1()
    {
        // Default implementation for Method1
    }
} 
```

## Static abstract and virtual members

Beginning with C# 11, an interface may declare static abstract and static virtual members for all member types except fields. This feature enables generic algorithms to specify number-like behavior.

## Interface inheritance

An interface can inherit from one or more base interfaces. When an interface overrides a method implemented in a base interface, it must use the explicit interface implementation syntax.

## Multiple Interface Implementation

 One of the notable advantages of interfaces is the ability for a class to implement multiple interfaces. This feature enables the class to inherit and provide implementations for the members defined in each interface it implements. This capability enhances code flexibility and promotes the reuse of common functionality.

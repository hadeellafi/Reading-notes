# Collections & Enums

## Collections

Two ways to group objects:

- creating arrays of objects
- creating collections of objects.

Collections provide a more flexible way to work with groups of objects,the group of objects you work can dynamically as the needs of the application change.

### Using a Simple Collection

example of collection initializer is used to add elements to the collection:

```csharp
var salmons = new List<string> { "chinook", "coho", "pink", "sockeye" };
```

you can itreate using:

- foreach
- for loop : The index of the elements starts at 0 and ends at the element count minus 1

### Kinds of Collections

Some of the common collection classes are:

- System.Collections.Generic classes: useful when every item in the collection has the same data type.

- System.Collections.Concurrent classes :used when multiple threads need to access collection items concurrently.

- System.Collections classes:it do not store elements as specifically typed objects, but as objects of type Object.

### Implementing a Collection of Key/Value Pairs

The Dictionary `<TKey,TValue>` generic collection enables  to access  elements by using the key of each element.use a key to retrieve a value is fast because the Dictionary class is implemented as a hash table.

### Using LINQ to Access a Collection

LINQ queries provide filtering, ordering, and grouping capabilities.
example:

```charp
// LINQ Query.
    var subset = from theElement in elements
                 where theElement.AtomicNumber < 22
                 orderby theElement.Name
                 select theElement;
```

## Enums

It is a value type defined by a set of named constants of the underlying integral numeric type. To define it use the `enum` keyword and specify the names of enum members:

```charp
enum Season
{
    Spring,
    Summer,
    Autumn,
    Winter
}
```

### The System.Enum type and enum constraint

The System.Enum type is the abstract base class of all enumeration types.use System.Enum in a base class constraint to specify that a type parameter is an enumeration type.

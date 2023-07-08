# LINQ & Delegates

## Language Integrated Query (LINQ) (C#)

- the name for a set of technologies based on the integration of query capabilities directly into the C# language.
- You write queries against strongly typed collections of objects by using language keywords and familiar operators.
- it provides a consistent query experience for objects (LINQ to Objects), relational databases (LINQ to SQL), and XML (LINQ to XML).
- By using query syntax, you can perform filtering, ordering, and grouping operations on data sources with a minimum of code.

```charp
// LINQ Query.
    var subset = from theElement in elements
                 where theElement.AtomicNumber < 22
                 orderby theElement.Name
                 select theElement;
```

## Introduction to LINQ Queries (C#)

### Three Parts of a Query Operation

All LINQ query operations consist of three distinct actions:

1. Obtain the data source: A queryable type requires no modification or special treatment to serve as a LINQ data source.

```charp
        int[] numbers = new int[7] { 0, 1, 2, 3, 4, 5, 6 };
```

2. Create the query: specifies what information to retrieve from the data source or sources.

```charp
        // numQuery is an IEnumerable<int>
        var numQuery =
            from num in numbers
            where (num % 2) == 0
            select num;
```

3. Execute the query.

```charp
        foreach (int num in numQuery)
        {
            Console.Write("{0,1} ", num);
        }
```

- **Deferred Execution**
In the example we iterate over the query variable in a foreach statement. This concept is referred to as deferred execution

- **Forcing Immediate Execution**
Queries that perform aggregation functions over a range of source elements must first iterate over those elements. Examples of such queries are `Count`, `Max`, `Average`, and `First`.

## Basic LINQ Query Operations (C#)

### Filtering

causes the query to return only those elements for which the expression is true using the `where` clause.

### Ordering

Often it is convenient to sort the returned data.The `orderby` clause will cause the elements in the returned sequence to be sorted according to the default comparer for the type being sorted.

### Grouping

The `group` clause enables you to group your results based on a key that you specify.

### Joining

Join operations create associations between sequences that are not explicitly modeled in the data sources.

### Selecting (Projections)

The `select` clause produces the results of the query and specifies the "shape" or type of each returned element.

## Things I want to know more about

- Advanced LINQ query techniques.
- LINQ performance and best practices.

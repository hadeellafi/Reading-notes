# Graphs

## WHY use Graphs?

Graphs are used because they are a powerful tool for modeling complex relationships between objects or entities.

## WHAT are Graphs?

A graph is a non-linear data structure consisting of `vertices` and edges.

- nodes -> entities
- edges -> relationships between these entities

types of graphs:

- **Undirected Graphs**: These are graphs where each edge is undirected or bi-directional. no direction associated with the edge and it can be traversed in both directions.
- **Directed Graphs (Digraph)**: These are graphs where every edge is directed from one node to another. Each node is directed at another node .
- **Complete Graphs**:where all nodes are connected to all other nodes.
- **Connected Graphs**:where all nodes have at least one edge.
- **Disconnected Graphs**:where some vertices may not have edges.
- **Acyclic Graphs**: These are directed graphs without cycles. A `cycle`is when a node can be traversed through and potentially end up back at itself.
- **Cyclic Graphs**: These are graphs that have cycles.

## HOW are Graphs represented?

- **Adjacency Matrix**: This is a 2-dimensional array that represents the graph. If there are n vertices, then we look at an n x n Boolean matrix.
- **Adjacency List**: An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.

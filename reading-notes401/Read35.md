# Graphs
A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

Here is some common terminology used when working with Graphs:

- **Vertex** - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
- **Edge** - An edge is a connection between two nodes.
- **Neighbor** - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
- **Degree** - The degree of a vertex is the number of edges connected to that vertex.

## Directed vs Undirected

### Undirected Graphs
An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

For example, in the graph below, Node C is connected to Node A, Node E and Node B. There are no “directions” given to point to specific vertices. The connection is bi-directional.

### Directed Graphs (Digraph)
A Directed Graph also called a Digraph is a graph where every edge is directed.

Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

Compare the visual below with the undirected graph above. Can you see the difference? The Digraph has arrows pointing to specific nodes.

## Complete vs Connected vs Disconnected

### Complete Graphs
A complete graph is when all nodes are connected to all other nodes.

### Connected
A connected graph is graph that has all of vertices/nodes have at least one edge.


### Disconnected
A disconnected graph is a graph where some vertices may not have edges.


## Acyclic vs Cyclic

### Acyclic Graph
An acyclic graph is a directed graph without cycles.

A cycle is when a node can be traversed through and potentially end up back at itself.


### Cyclic Graphs
A Cyclic graph is a graph that has cycles.

A cycle is defined as a path of a positive length that starts and ends at the same vertex.


## Graph Representation
We represent graphs through:

1. Adjacency Matrix
1. Adjacency List

## Traversals

### Breadth First
In a breadth first traversal, you are starting at a specific vertex/node. This node must be specified when calling the BreadthFirst() method. The breadth-first traversal of a graph is like that of a tree, with the exception that graphs can have cycles. Traversing a graph that has cycles will result in an infinite loop….this is bad. To prevent such behavior, we need to have some way to keep track of whether a vertex has been “visited” before. Upon each visit, we’ll add the previously-unvisited vertex to a visited set, so we know not to visit it again as traversal continues.


Here is what the algorithm breadth first traversal looks like:

1. Enqueue the declared start node into the Queue.
1. Create a loop that will run while the node still has nodes present.
1. Dequeue the first node from the queue
1. if the Dequeue‘d node has unvisited child nodes, add the unvisited children to 1.visited set and insert them into the queue.

### Depth First
In a depth first traversal, we approach it a bit different than the way we do when working with a depth first traversal of a tree. Similar to how the breadth-first uses a queue, we are going to use a Stack for our depth-first traversal.


## Real World Uses of Graphs
Graphs are extremely popular when it comes to it’s uses. Here are just a few examples of graphs in use:

1. GPS and Mapping
1. Driving Directions
1. Social Networks
1. Airline Traffic
1. Netflix uses graphs for suggestions of products

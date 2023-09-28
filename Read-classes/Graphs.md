# Graphs

A graph data structure is a way of storing and organizing data that shows how different items are related to each other. Graphs can help us to model complex systems, such as social networks, computer networks, maps, and more. Graphs are made up of two main components: vertices and edges.

- Vertices are the points or nodes in the graph that represent the data items. For example, in a social network graph, each vertex could be a person, and each person could have some data associated with them, such as their name, age, location, etc.
- Edges are the lines or links that connect the vertices in the graph. Edges show how the vertices are related to each other. For example, in a social network graph, each edge could be a friendship, and each friendship could have some data associated with it, such as when it was created, how often they interact, etc.

---

There are different types of graphs, depending on how the `vertices` and `edges` are arranged and what kind of data they have. Some common types of graphs are:

- Undirected graph: A graph where the edges do not have any direction. This means that there is no difference between going from vertex A to vertex B or from vertex B to vertex A. For example, a friendship graph is an undirected graph, because friendship is a mutual relationship.
- Directed graph: A graph where the edges have a direction. This means that there is a difference between going from vertex A to vertex B or from vertex B to vertex A. For example, a follower graph is a directed graph, because following is a one-way relationship.
- Weighted graph: A graph where the edges have some numerical value or weight associated with them. This weight can represent the cost, distance, time, or any other measure of the relationship between the vertices. For example, a map graph is a weighted graph, because the edges can represent the distance or time between the locations.
- Cyclic graph: A graph that contains at least one cycle or loop. A cycle is a path that starts and ends at the same vertex. For example, a cycle graph is a cyclic graph that has all the vertices connected in a circular shape.
- Acyclic graph: A graph that does not contain any cycle or loop. For example, a tree is an acyclic graph that has one root vertex and no cycles.
- Bipartite graph: A graph that can be divided into two sets of vertices such that no edge connects two vertices from the same set. For example, a matching graph is a bipartite graph that shows how two sets of items can be paired up.

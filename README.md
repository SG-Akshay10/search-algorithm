# Search Algorithm

Implementation of Breadth First Search and Depth First Search algorithm using C

# Breadth First Search

Breadth-first search is a graph traversal algorithm that starts traversing the graph from the root node and explores all the neighboring nodes. Then, it selects the nearest node and explores all the unexplored nodes. While using BFS for traversal, any node in the graph can be considered as the root node.
It is a recursive algorithm to search all the vertices of a tree or graph data structure. BFS puts every vertex of the graph into two categories - visited and non-visited. It selects a single node in a graph and, after that, visits all the nodes adjacent to the selected node.

### Applications of BFS algorithm

The applications of breadth-first-algorithm are given as follows -

* BFS can be used to find the neighboring locations from a given source location.
* In a peer-to-peer network, BFS algorithm can be used as a traversal method to find all the neighboring nodes. Most torrent clients, such as BitTorrent, uTorrent, etc. employ this process to find "seeds" and "peers" in the network.
* BFS can be used in web crawlers to create web page indexes. It is one of the main algorithms that can be used to index web pages. It starts traversing from the source page and follows the links associated with the page. Here, every web page is considered as a node in the graph.
* BFS is used to determine the shortest path and minimum spanning tree.
* BFS is also used in Cheney's technique to duplicate the garbage collection.
* It can be used in ford-Fulkerson method to compute the maximum flow in a flow network.

### Algorithm
The steps involved in the BFS algorithm to explore a graph are given as follows -

* SET STATUS = 1 (ready state) for each node in G

* Enqueue the starting node A and set its STATUS = 2 (waiting state)

* Repeat Steps 4 and 5 until QUEUE is empty

* Dequeue a node N. Process it and set its STATUS = 3 (processed state).

* Enqueue all the neighbours of N that are in the ready state (whose STATUS = 1) and set their STATUS = 2 (waiting state)

  [END OF LOOP]

* EXIT

# Depth First Search 

It is a recursive algorithm to search all the vertices of a tree data structure or a graph. The depth-first search (DFS) algorithm starts with the initial node of graph G and goes deeper until we find the goal node or the node with no children. The process of implementing the DFS is similar to the BFS algorithm.

The step by step process to implement the DFS traversal is given as follows -

* First, create a stack with the total number of vertices in the graph.
* Now, choose any vertex as the starting point of traversal, and push that vertex into the stack.
* After that, push a non-visited vertex (adjacent to the vertex on the top of the stack) to the top of the stack.
* Now, repeat steps 3 and 4 until no vertices are left to visit from the vertex on the stack's top.
* If no vertex is left, go back and pop a vertex from the stack.
* Repeat steps 2, 3, and 4 until the stack is empty.

### Applications of DFS algorithm
The applications of using the DFS algorithm are given as follows -

* DFS algorithm can be used to implement the topological sorting.
* It can be used to find the paths between two vertices.
* It can also be used to detect cycles in the graph.
* DFS algorithm is also used for one solution puzzles.
* DFS is used to determine if a graph is bipartite or not.

### Algorithm
* SET STATUS = 1 (ready state) for each node in G

* Push the starting node A on the stack and set its STATUS = 2 (waiting state)

* Repeat Steps 4 and 5 until STACK is empty

* Pop the top node N. Process it and set its STATUS = 3 (processed state)

* Push on the stack all the neighbors of N that are in the ready state (whose STATUS = 1) and set their STATUS = 2 (waiting state)

  [END OF LOOP]

* EXIT



- Incidence Matrices
- Graph Isomorphism
- Hamilton Paths and Circuits

## Property of Degrees

If $G = (V, E)$ is an undirected graph with $m$ edges, then:

$$
2m = \sum_{v \in V} \deg v
$$

### Special Graphs

- Complete graphs: $K_{n}$

## Bipartite Graphs

> Partitions into two different sets  
> A bipartite graph is a graph where it is possible to color the vertices red or blue so that no two adjacent vertices are the same color.

![image](https://obsidian-img-studies.tsun1031.xyz/2024/11/25/664befbe798473b2af4a810912e37d5a9b360c4ddebca8ee745c366170c83b39.png)

### Complete Bipartite Graph

### Subgraphs

## Representing Graphs

### Adjacency Matrices

$$
\begin{bmatrix}  
1 & 2 & 3\\  
a & b & c  
\end{bmatrix}
$$

## Euler Paths and Circuits

- **Euler path**: Starts and ends at different vertices
- **Euler circuit**: Starts and ends ==at the same vertex==

## Proof Whether a Valid Graph

### Complete Bipartite

In a complete bipartite graph, the vertices can be divided into two sets, say A and B, such that every vertex in A is connected to every vertex in B, and there are no edges within set A or within set B.

Let's say |A| = _a_ and |B| = _b_. In this case, we must have a + b = n.  Moreover, if a vertex v is in A, its degree will be _b_, and if a vertex v is in B, its degree will be _a_.

### Non Existence

The sum of the degrees of all vertices in a graph is always twice the number of edges (the Handshaking Lemma). Therefore, the sum of the degrees must be an even number.

### In and Out Degrees

They must be equal in sum.

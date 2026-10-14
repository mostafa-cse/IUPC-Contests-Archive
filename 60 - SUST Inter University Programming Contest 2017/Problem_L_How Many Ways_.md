# How Many Ways?

**URL:** https://toph.co/p/how-many-ways  

---

Regular problem solvers starts their journey by solving ad hoc and number theory. After getting the hang of it, they jump into graph and combinatorics type of problems. You are one of guys going through this phase. After learning the basics of graph theory, algorithms (bfs, dfs) and data structures (queue, stack) which are needed for understanding those, you wanted to have a break from graph theory. And thus, you started solving problems from basic combinatorics category.

From your previous math studies, you know all about permutations and combinations. After solving couple of problems from the “Felix Halim” list of combinatorics problems, you found an interesting problem which had ties with graph theory.

You are given a connected undirected graph, which has a starting position (or node) and an ending position (or node). You have to figure out, in how many ways (different paths) can you travel from the starting position to ending position. It is also stated that this graph is actually a tree, and you cannot visit the same node twice in your path from start to end.

Input

Input starts with an integer T (≤ 100), denoting the number of test cases.

Each case starts with a line containing two integers, N (≤ 100) and M (= N-1), denoting the number of nodes and the number of edges in the graph. The next line contains two integers, S and E, (1 ≤ S, E ≤ N), marking the starting and ending node of your path. Each of the next M lines contains two integers, U and V (1 ≤ U, V ≤ 100), denoting an undirected edge between node U and node V.

Output

For each case, print the case number and the total number of ways to go from node S to node E. See the samples for exact formatting.

Example

Notes

A graph is made up of nodes (or vertices, or points) which are connected by edges (or arcs, or lines). An undirected graph means that there is no distinction (or direction) between the two vertices associated with each edge.

Path

In graph theory, a path in a graph is a finite or infinite sequence of edges which connect a sequence of vertices.

Tree

A tree is a data structure made up of nodes or vertices and edges without having any cycle.

More specifically in graph theory, a tree is an undirected graph in which any two vertices are connected by exactly one path.


---

## Samples

### Sample Input 1
```
1
4 3
1 4
1 2
2 3
2 4
```

### Sample Output 1
```
Case 1: 1
```

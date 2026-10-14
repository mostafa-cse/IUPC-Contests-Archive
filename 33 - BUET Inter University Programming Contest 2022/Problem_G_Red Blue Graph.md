# Red Blue Graph

**URL:** https://toph.co/p/red-blue-graph  

---

You are given a connected, undirected, unweighted graph. You need to assign one of the two colors Red or Blue to every edge of the graph in such a way that, for each node

$|degree_R-degree_B| \leq 1$

.

$degree_R$

of a node is the number of adjacent edges to that node which are colored Red.

$degree_B$

of a node is the number of adjacent edges to that node which are colored Blue.

Input

The first line contains one integer

$T$

- the number of test cases. First line of each testcase contains two integers

$N$

,

$M$

- the number of vertices and the number of edges in the graph respectively. Each of the next

$M$

lines contain two integers

$u_i$

and

$v_i$

describing an undirected edge in the graph.

$1 \leq T \leq 100$

$1 \leq N \leq 10^5$

$N-1 \leq M \leq min(3*10^5, (N*(N-1))/2)$

Sum of

$N$

over all testcases doesn’t exceed

$10^6$

and sum of

$M$

over all testcases also doesn’t exceed

$10^6$

.

It is guaranteed that the graph is connected, it has no self-loop and there is at most one edge between every pair of vertices.

Output

If it is not possible to find such a coloring, print

$-1$

. Otherwise print one such coloring of the edges in the order given. If there exists more than one coloring you can print any one. You should print a string containing only

$R$

and

$B$

to denote the coloring.

Example


---

## Samples

### Sample Input 1
```
2
6 5
1 2
1 3
2 4
2 5
5 6
3 3
1 2
2 3
1 3
```

### Sample Output 1
```
BRRRB
-1
```

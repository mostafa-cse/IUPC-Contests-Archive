# MaxFlow (II)

**URL:** https://toph.co/p/maxflow-ii  

---

Given a connected undirected graph with

n

nodes and

m

edges and the capacity of each edge is

1

.

maxFlow(u, v)

defines the maximum flow from node

u

to node

v

. You have to find out how many pair of nodes

(u, v)

are there where

u < v

and

maxFlow(u, v) = 2

.

Input

The first line of the input contains an integer

T

, denoting the number of test cases. For each test case, the first line will have two integers

n

and

m

, denoting the number of nodes and edges of the graph. The following

m

lines will contain two integers

u

and

v

, denoting an undirected edge between

u

and

v

. You can assume that the graph won’t have any self loop.

Output

For each test case, print the case number and the result for that case.

Example


---

## Samples

### Sample Input 1
```
2
3 3
1 2
1 3
3 2
3 2
1 2
2 3
```

### Sample Output 1
```
Case 1: 3
Case 2: 0
```

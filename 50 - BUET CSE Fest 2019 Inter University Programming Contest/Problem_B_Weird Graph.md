# Weird Graph

**URL:** https://toph.co/p/weird-graph  

---

Anik got a directed acyclic graph with some weird properties. For Every node

$v$

of that graph

$in(v)≤1$

and

$out(v)≤1$

where

$in(v)$

means in-degree of vertex

$v$

and

$out(v)$

means out-degree of vertex

$v$

.

Now he is wondering how many different topological sorts of that graph is possible. As he is not smart enough to figure it out, you are asked to help him out.

Input

First line contains two integers

$n$

and

$m$

(

$1 ≤ n ≤ 10^5$

,

$0 ≤ m ≤ 10^5$

): the number of nodes and edges.

Each next m lines contains two integers

$p$

and

$q$

(

$1 ≤  p,q ≤ n$

), meaning there is an edge from

$p$

to

$q$

.

It is guaranteed that the graph is acyclic and

$in(v) ≤ 1$

and

$out(v) ≤1$

.

Output

Print the number of different topological sorts of that graph modulo 1000000007 (

$10^9+7$

).

Examples

Notes

In-degree of a node means number of edges incoming to a node. Out-degree of a node means number of edges outgoing from a node.


---

## Samples

### Sample Input 1
```
4 2
1 2
2 3
```

### Sample Output 1
```
4
```

### Sample Input 2
```
4 3
1 2
2 3
3 4
```

### Sample Output 2
```
1
```

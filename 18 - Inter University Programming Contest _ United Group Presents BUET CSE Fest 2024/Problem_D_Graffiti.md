# Graffiti

**URL:** https://toph.co/p/graffiti  

---

Given a

simple

undirected

connected

graph with

$N$

vertices. Each vertex will have a value

$A_i$

associated with it. You can perform the following operation any number of time

(possibly 0)

:

Choose two vertices such that they are

connected

by an edge. Replace their value with the

XOR

of their

current

value. For example, choosing

$u$

and

$v$

will result in,

$A_u = A_v = A_u \oplus A_v$

You have to

maximize

the

sum

of the value of all the vertices of the

final

graph. Print the

maximum

sum of value.

Input

The first line will contain two space separated integers

$N$

and

$M$

denoting the number of vertices and number of edges respectively.

The second line will have N space separated integers

$A_1$

$A_2$

$\cdots$

$A_N$

representing the initial values of each vertex.

Next M lines each contains two space separated integers

$U_i$

and

$V_i$

indicating that there is an edge between those two vertices.

Constraints:

$1 \le N \le 2 \times 10^5$

$N - 1 \le M \le 3 \times 10^5$

$0 \le A_i \le  10^9$

$1 \le U_i \lt V_i \le N$

The graph contains no self-loop or no multi-edge, which means-

$U_i \ne V_i$

$(U_i, V_i) \ne (U_j, V_j)$

where

$i \ne j$

Output

Print the

maximum

sum of the value of all the vertices of the

final

graph.

Examples


---

## Samples

### Sample Input 1
```
4 3
1 7 2 8
1 2
2 3
3 4
```

### Sample Output 1
```
56
```

### Sample Input 2
```
4 4
1 7 2 8
1 2
1 3
2 3
3 4
```

### Sample Output 2
```
60
```

# Thanos LLC.

**URL:** https://toph.co/p/thanos-llc  

---

On the planet Titan, there are

$N$

residents, numbered from

$1$

to

$N$

, all employed by Thanos. For each

$i$

from

$1$

to

$N$

,

$i^{th}$

person’s salary can be described as

$S_i$

.

On planet Titan, a network of people can be described as an unweighted directed graph containing

$N$

nodes. Each node represents a person and each edge represents a one-way friendship. There can be duplicate edges. In this network, individuals who share mutual friendships are considered part of the same community. These communities form groups where each member can reach every other member through a series of interconnected friendships.

You need to execute

$Q$

queries on this graph, each falling into one of three categories:

$AC$

$X$

$Y$

: Add amount

$X$

to the income of each person within the community to which person

$Y$

belongs.

$AS$

$X$

$Y$

: Add amount

$X$

to the income of person

$Y$

directly.

$Q$

: Determine the maximum individual income across the entire planet and identify the maximum number of people sharing that income within a single community.

Note that the value of the amount

$X$

can be either positive or negative. If an individual's income becomes negative, it indicates they are in debt to Thanos. In case of all negative income in the whole planet, print a single integer 0, otherwise print two integers indicating the maximum individual income across the planet and the maximum number of people who earn that amount within a single community.

Input

The first line of input consists of three integers:

$N$

,

$M$

, and

$Q$

$(2 ≤ N, M, Q ≤ 2 × 10^5)$

, representing the number of nodes, the number of edges, and the number of queries to perform, respectively.

Each of the next

$M$

lines contains two integers,

$U$

and

$V$

$(1 ≤ U, V ≤ N, U ≠ V)$

, indicating a directed edge from node

$U$

to

$V$

.

The next line contains

$N$

space-separated integers, denoted as

$S_i$

$(1 ≤ |S_i| ≤ 10^9)$

for each

$i$

from

$1$

to

$N$

, representing the salary of the

$i^{th}$

person.

The following

$Q$

lines each contain one of three types of queries, presented in the following format:

$AC$

$X$

$Y$

$(1 ≤ Y ≤ N, 1 ≤ |X| ≤ 10^9)$

$AS$

$X$

$Y$

$(1 ≤ Y ≤ N, 1 ≤ |X| ≤ 10^9)$

$Q$

Output

For each of the

$Q$

query types, print two integers

$S$

and

$P$

on a single line separated by a space.

$S$

represents the maximum individual income across the planet, and

$P$

represents the maximum number of people sharing that income within a single community. In case of all negative income in the whole planet, print a single integer 0.

Example


---

## Samples

### Sample Input 1
```
6 6 16
1 2
2 3
2 4
2 5
5 2
3 6
5 2 3 1 6 10
Q
AC 5 2
Q
AS 4 2
Q
AS 1 6
Q
AS 10 1
Q
AS -100 2
AC -100 1
AC -100 4
AC -100 3
AC -100 6
AC -100 5
Q
```

### Sample Output 1
```
10 1
11 1
11 2
11 2
15 1
0
```

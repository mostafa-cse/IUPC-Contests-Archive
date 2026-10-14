# Meena, Raju and Mango Tree

**URL:** https://toph.co/p/meena-raju-and-mango-tree  

---

Clever girl Meena likes to climb trees. One day her brother Raju, after coming back from school, said to Meena with joyful eyes, “I have seen a big tree with many ripe mangoes. Let's go climb that one!”.

We can think of the mango tree as a connected undirected graph with no cycles and having exactly one path from one node to another. Meena asked Raju to describe the tree. Raju could not memorize the exact structure of the tree but remembered how many nodes were at each level considering the tree is rooted. Suddenly, they both got worried as many trees could satisfy that condition and Meena could not climb trees with all diameters.

In tree data structures, the root node is said to be at level 0, the root node's children are at level 1, and the children of that node at level 1 will be at level 2, and so on. And, the diameter of a tree means the number of nodes on the longest path in the tree.

Can you help Meena and Raju determine how many unique diameter lengths are possible for any such tree?

Suppose that, the mango tree has

$n$

levels. For each level

$i\ (0 \leq i < n)$

there exists

$a[i]$

nodes,

$0$

-indexed.

You will be given an array

$b$

of length

$m\ (m < n)$

,

$1$

-indexed.

Now, to construct

$a$

from

$b,$

you need to follow the following instructions:

$a[0] = 1$

$a[i] = b[i]$

for

$1 \leq i \leq m$

$a[i]=a[i-m]$

for

$m < i < n$

Input

The first line will contain

$T\ (1 \leq T \leq 10^5),$

the number of test cases.

For each test cases, the first line will contain two integers

$n,\ m\ (2 \leq n \leq 10^9,\ 1 \leq m < min(n,10^5)),$

the number of levels in the tree and the length of the array

$b.$

In the next line, there will be

$m$

integers denoting the elements of array

$b\ ( 1 \leq b[j] \leq 10^9, for\ all\ 1 \leq j \leq m ).$

It’s guaranteed that,

$\sum m$

over all test cases

$\leq 2 × 10^5.$

Output

For each test case, output a single integer denoting the possible number of unique diameter lengths.

Example


---

## Samples

### Sample Input 1
```
1
3 1
2
```

### Sample Output 1
```
2
```

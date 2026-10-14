# Will Power

**URL:** https://toph.co/p/will-power  

---

Dividing wealth is tricky. When people die, they leave their property to their children, who often end up fighting over it. Sometimes, part of the inheritance even goes to charity, making the whole process more complicated.

We will automate the process of wealth division within a family tree. Initially, there is only one node (Node 1) representing the original ancestor. Consider Node 1 to have

no wealth

. As time progresses, new nodes (children) will be added. Each node is assigned a certain amount of wealth at birth. When a node

$u$

dies, its wealth is distributed evenly among its children. If

$u$

has a child

$v$

who has already passed away, then

$v$

’s share of

$u$

’s wealth is divided equally to

$v$

’s children. This process continues recursively until all shares have been distributed or until a deceased node has no living descendants, in which case the wealth is given to charity.

There will be three types of queries:

Type 1: A Node Dies

This records a node's death and distributes its wealth among its children.

Type 2: A Child is Born

This adds a new node

$x$

to the family tree and assigns them a set amount of wealth

$y$

.

A dead node cannot give birth to another node

.

Type 3: Calculate Wealth

This calculates the current wealth of a

alive

node in the family tree. Since the answer can be fractional, it must be output in the format

$P \times Q^{-1} \mod M$

if the answer is

$\frac{P}{Q}$

where

$M = 10^9 + 7$

.

Input

The input consists of multiple test cases. Each test case starts with an integer

$t$

(the number of test cases). For each test case:

1. The first line contains an integer

$q$

(

$2\leq q\leq 2\times 10^5$

), representing the number of queries.

2. The next

$q$

lines contain the queries in the following format:

Type 1 Query

: An integer

$1$

followed by an integer

$x$

(the number of the deceased node, where

$x\leq q+1$

and

$x$

is alive in the tree ).

Type 2 Query

: An integer

$2$

followed by three integers

$x$

(the node number, where

$x \leq q+1$

and

$x$

was never added to the tree),

$y$

(the wealth of the node, where

$0 \leq y\leq 10^6$

) and parent node

$p$

(

$p$

is alive and present in the tree).

Type 3 Query:

An integer

$3$

followed by an integer

$x$

(the number of the node, where

$x \leq q+1$

and

$x$

is alive).

It is guaranteed that there are no invalid queries. The sum of

$q$

over all test cases doesn’t exceed

$2\times 10^5$

.

Output

For Type 1 Query and Type 2 Query, no output is required. For Type 3 Query, output the current wealth of the specified node in the format

$P \times Q^{-1} \mod M$

where the answer is

$\frac{P}{Q}$

and

$M = 10^9 + 7$

Examples

Notes

This diagram explains the distribution of wealth in the 2nd Sample IO.


---

## Samples

### Sample Input 1
```
1
13
2 2 8 1
2 3 2 2
2 4 5 3
2 8 10 3
2 5 6 2
2 6 5 5
2 7 5 5
1 2
3 5
3 3
1 5
3 6
3 7
```

### Sample Output 1
```
10
6
10
10
```

### Sample Input 2
```
1
9
2 2 8 1
2 3 6 2
2 4 1 3
2 5 1 3
2 6 3 2
1 3
1 2
3 4
3 6
```

### Sample Output 2
```
6
7
```

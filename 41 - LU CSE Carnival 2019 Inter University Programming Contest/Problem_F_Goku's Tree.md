# Goku's Tree

**URL:** https://toph.co/p/goku-s-tree  

---

Recently Goku has discovered a rooted tree graph. Goku’s tree has

N

nodes, among them node 1 is the root and each node has a destruction factor in it.

Goku is very curious about his tree, so he is doing an experiment by removing nodes from the tree. First he selects a node from the tree and removes the subtree rooted in the selected node. He continues this process until there is no remaining node in the tree. When there is no remaining node, he calculates the destruction value of the tree. Destruction value indicates the sum of destruction factor of all selected nodes.

Goku has built a robot that will select the nodes from the tree in a predefined order and will remove the subtree of the selected node. But there are some bugs in Goku’s robot. So instead of selecting the nodes in a predefined order, the robot will select nodes randomly with uniform probability. To measure the randomness of his robot, Goku is interested in knowing the expected destruction value of his tree if the nodes are selected randomly with uniform probability.

In this problem, you will be given a tree with the initial destruction factor of all nodes. There will be

M

update operations. Each operation will contain a node

U

and an integer

X

. An operation

(U, X)

means, you will have to add

X

to the destruction factor of all nodes that are present in the subtree rooted at node

U

. After each update, you will have to output the expected destruction value of the tree. Any update in the tree is permanent.

Input

First line contains an integer

T (1≤T≤500)

, denoting the number of test cases.

The following lines contain the

T

test cases.

Each test case begins with two integer

N (1≤N≤100000)

and

M (1≤M≤100000)

, denoting the number of nodes and number of update operations.

The next line contains

N

integers

Ai (1≤Ai≤10000000)

, denoting the initial destruction factor of node

i (1≤i≤N)

.

Following

N-1

lines contain two integers

u (1≤u≤N)

and

v (1≤v≤N)

, means there is an edge between node

u

and node

v

.

The following

M

lines contain the

M

update operations.

Each operation contains two integers

U (1≤U≤N)

and

X (0≤X≤10000000)

, means you will have to add

X

to the destruction factor of all nodes that are present in the subtree rooted at node

U

.

Note:

Size of the input file won't exceed 20 MB

Output

For each case, first print the case number. Then for each update operation, print an integer in a separate line denoting the expected destruction value of the tree. If the answer is

P/Q

(where

P(≥0)

and

Q(>0)

are two integers and coprime), then print it as

(P x Q-1) mod 1000000007

.

See the sample output for the exact format.

Example


---

## Samples

### Sample Input 1
```
1
2 1
6 3
1 2
2 3
```

### Sample Output 1
```
Case 1:
9
```
